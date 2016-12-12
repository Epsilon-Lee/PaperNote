Setup and Running
-----------------

As prerequisites, this project requires Node.js and NPM to be installed, along with the TypeScript compiler (1.8+).
If you don't already have TypeScript installed as a global NPM package, then run this command:

`npm install -g typescript`

Now start by cloning this Git repository:

`git clone https://github.com/hzxie/PaperNote.git`

... and running the following command from the project root directory:

`npm install`

At this point, you can build and launch the application with:

`npm start`

Development Notes
-----------------

The type definition files used by this project are managed by the "typings" TypeScript Definition Manager,
version 1.0 or higher.  It is not necessary to have "typings" installed just to run this application.  However,
if you want to develop on your own fork, and have the ability to update the type definitions, then you'll need
to install "typings" as a global NPM module:

`npm install -g typings`

The type definitions are committed to source control, as the `typings.json` file and the `typings` subdirectory.
To get the latest type definitions, delete that file and subdirectory and replace them by running these 
commands:

```
typings install dt~core-js --save --global
typings install dt~electron/github-electron --save --global
typings install dt~jasmine --save --global
typings install dt~node --save --global
```