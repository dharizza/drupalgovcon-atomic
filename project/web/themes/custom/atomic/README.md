## Compiling CSS / JS

The Atomic theme and all it's sub-themes are designed to use `gulp` to compile
SASS and JavaScript. Here's how you can get the ball rolling:

### One-time setup

  1. Install `nvm` if it is not already installed. This helps you manage
     multiple versions of Node JS.

  1. Open the terminal and `cd` into your theme's directory.

  1. Install the Node version `16.x`. You can do this by running
     `./install-node.sh 16.14.2`. You only need to do this once.

  1. The previous step will generate a `.nvmrc` file. To use the correct
     version of node for this project, simply `cd` into your theme's directory
     and run `nvm use`.

  1. Next, we install `gulp`. Gulp will help us compile SASS / JS files. Simply
     run `npm install` and all the right tools and libraries will be installed.

### Compiling CSS / JS

First you have to install `nvm` and `gulp` as per instructions above. Once that
is done, you should be able to run `nvm --version` and `gulp --version` and
see their respective versions without any error.

Now whenever you want to work with SASS / JS, do the following:

  1. Open a terminal window and `cd` into your theme's directory.

  1. Run `nvm use` to make sure that you're using the right version of Node.

  1. Run `gulp watch` and it will watch your SCSS / JS files for changes. As
     and when changes are detected, the respective CSS / JS files will be
     compiled and placed in the `css` and the `js` directories respectively.

You can then test your CSS / JS changes and if you're happy with them, you can
commit them into the version control system.
