# Qlik Sense Extension: Reload and Replace a published app

Simple extension, that 
 * allows a developer to refresh an already published app with a new design from a copy of this app (standard process)
 * allows to reload the app without going through script editor (using QRS API - also works when app is already published)
 
## Virtual Proxy Setup

It is necessary to setup a virtual proxy first, so that the extension can authorize against it. 

## Data Connection to the App Folder

If you plan to use the option *Keep data + script of target app* you need to create and define a data connection, that points to the 
Qlik Sense shared app folder. This is needed, because the local app will be BINARY loaded with the data model of the target app 
before replacing its design+data. After this is done, the source app's data will be reverted to the data you had when you clicked 
the button. 

![screenshot](https://github.com/ChristofSchwarz/pics/raw/master/cbkeepdata.png "screenshot")


