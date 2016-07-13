# XIB 2 NIB

Sometime it can be handy to use an already defined user interface and load it e.g. from your Swift based playground. It is not enought to simply add your XIB files as a Resource to your playground, since the Swift playground needs compiled resources to make it instantly visible in a live preview. For compiling a XIB to a NIB file you need to use the 'ibtool':

```sh
ibtool --compile CompiledView.nib RawView.xib
```

'ibtool' comes installed with your XCode, so can be simply run from your shell, terminal environment.

