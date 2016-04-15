# Using Google cloud source with git GUIs

The easisest and recommended way to connect to Google's git repository system is done via the `gcloud` command line interface as it is also written [here](https://cloud.google.com/source-repositories/docs/quickstart). After setting up some config data for gcloud, it can authenticate you via issuing the `gcloud auth login` command. This command pops up a browser window asking you to login via Google, than you may return back to console, and start using the repository with the classical git CLI instructions:

```bash
$ git pull 
$ git branch
$ sh making_some_changes.sh
$ git push -all
```

However sometimes this is not the case that you only want to stick with the CLI git handling when you are developing. You would rather need to use Sourcetree or Github Desktop for light-weight version controlling. So when you want authenticate yourself via your favorite Git GUI to sync and pull/push source code changes from Google hosted repo,  you need to enable custom credentials in "the preferred authentication method" under the Reposity Settings on the cloud console of the Google project you are working on. This will generate a custom downloadable credential, which you can set for your git GUI.

Further description comes soon..

