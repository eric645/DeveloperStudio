# Developer Studio
==================================================
What you need to build your own Developer Studio
-----------------------------------

In order to build jQuery, you need to have the latest Node.js/npm and git 1.7 or later. Earlier versions might work, but are not supported.

For Windows, you have to download and install [git](https://git-scm.com/downloads) and [Node.js](https://nodejs.org/en/download/).

OS X users should install [Homebrew](http://brew.sh/). Once Homebrew is installed, run `brew install git` to install git,
and `brew install node` to install Node.js.

Linux/BSD users should use their appropriate package managers to install git and Node.js, or build from source
if you swing that way. Easy-peasy.


How to build your own Developer Studio
----------------------------

Clone a copy of the main Developer Studio git repo by running:

```bash
git clone git://github.com/eric645/DeveloperStudio.git
```

Enter the developer studio directory and run the build script:
```bash
cd "DeveloperStudio" && npm run build
```
The built version of jQuery will be put in the `dist/` subdirectory, along with the minified copy and associated map file.

If you want to create custom build or help with Developer Studio, it would be better to install [grunt command line interface](www.gruntjs.com) as a global package:

```
npm install -g grunt-cli
```
Make sure you have `grunt` installed by testing:
```
grunt -V
```

Now by running the `grunt` command, in the jquery directory, you can build a full version of jQuery, just like with an `npm run build` command:
```
grunt
```
