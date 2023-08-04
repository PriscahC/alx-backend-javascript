# Introduction to Java Scrip

I encountered this error;
-ERROR: npm v9.8.1 is known not to run on Node.js v12.22.12.  This version of npm supports the following node versions: `^14.17.0 || ^16.13.0 || >=18.0.0`. You can find the latest version at https://nodejs.org/.

ERROR:
/usr/lib/node_modules/npm/lib/utils/exit-handler.js:19
  const hasLoadedNpm = npm?.config.loaded
                           ^

SyntaxError: Unexpected token

Resolved by re-installing nodejs and npm;
- curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
If you need another Node.js version, for example 12.x, change the setup_14.x with setup_12.x.
- sudo apt install nodejs
installs Node.js and npm
- node --version
- npm --version
- sudo apt install build-essential
enables to compile native addons from npm by installing the development tools:

