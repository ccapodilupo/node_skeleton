
# Node Skeleton

Use this as a starting point for an app (Handlebars Express)

## Install

* **Terminal into server** - run command: ssh <user>@bos1dnodel01.bos1.vrtx.com
* **Make project** - run command: mkdir /apps/project/<yourapp>
* **Go to project** - run command: cd /apps/project/<yourapp>
* **Get files from Subversion** - run command: svn export --force http://svn.vrtx.com/svn/webdev/node_skeleton/trunk .
* **Install modules** - run command: npm install	
* **Modify README.md** - change this file with your app's description, etc
* **Modify main server file** - change the filename of node_skeleton.js to yourApp.js and modify the configs in that file
  * fielstoragepath
  * port
  * app.locals
* **Modify env.json file** - Add additional dbconnections as necessary for your app
   
## Things to Note
* notice the svn-ignore.txt file - keep existing contents (node_modules and env.json) and add anything that you don't want in subversion. Run the following command from your checked out, or working, directory: svn propset svn:ignore -RF svn–ignore.txt .
* always use npm install --save --save-exact **AND** npm uninstall --save
* put static files in /public - the skeleton has a mapping so that the web server will serve things in  rooturl/static/
* reloadify - this reloads the browser when views change - if you don't want it remove the refreences to it in code and npm uninstall reloadify --save

```
Have fun!
```
