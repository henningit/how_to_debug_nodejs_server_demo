# Project to Show How a Nodejs Server can be Debugged

# Install
Open a console (CMD) inside this directory and install the needed module dependencies included in `package.json` from inside the directory

```sh
$ npm install
```

In case you're behind a firewall try

```sh
git config --global http.proxy http://proxy:8080
```

# Run
Start the server

```sh
$ node app.js
```

# Debug
1. Install [node-inspector][]:

	```sh
	$ npm install -g node-inspector
	```
2. Check your nodejs version

	Make sure to use a nodejs version that works together fine with [node-inspector][]. According to my experience the latest version creates issue. But the older version I use [nodejs version 6.3.1][] works fine. Find out the version of nodejs you are using by typing in a console:

	```sh
	$ node --version
	```
	If you want to change to an older version of nodejs then first deinstall nodejs and afterwards install the older version.
3. Start debugging the server by typing

	```sh
	$ node-debug app.js
	```

[node-inspector]: https://github.com/node-inspector/node-inspector 	"Node Inspector"

[nodejs version 6.3.1]: https://nodejs.org/download/release/v6.3.1/
