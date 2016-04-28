# Separator line with CSS

Using CSS pseudo elements are a great way to extend your web page look and feel with nice additions, like adding separator/decorator lines in between DOM elements, or simply addding a line before and after a header title.

You can add a decorator line next to a textual innerHTML, like for 'H1' element's text content by simply 
  * using empty pseudo before and after contents indicated by: 'content': ""
  * setting an inline-block 'display' attributes to visualize them
  * setting a 'width' per your choice for the lines
  * and of course as these elements are empty meaning they do not have a dimension (nor height or width), we must add one of the horizontal borders to them, like 'border-bottom'
  * to make the border middle aligned to the original HTML element, we must also set 'vertical-align' attribute to middle

To prevent the lines flowing together with the text content, we can add some spacing by setting margins to the before and after presudo elements, to the right and left sides accordingly.

This is the full CSS below, which decorates a header element with some nice line along its right and left sides:

```css
h1 {
  text-align: center;
}
h1:before, h1:after {
  content: "";
  display: inline-block;
  width: 10%;
  border-bottom: 1px solid;
  vertical-align: middle;

}
h1:before {
  margin-right: 5px;
}
h1:after {
  margin-left: 5px;
}
```

Credit goes to [stackoverflow question](http://stackoverflow.com/questions/23584120/line-before-and-after-title-over-image), which shows a bit more complex version pulling and stretching the lines by setting negative margins.
