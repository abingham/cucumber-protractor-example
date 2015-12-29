# cucumber-protractor-example
Example of how to use cucumber with protractor.

## Setup and running

First you need to install protractor, cucumber, and the other dependencies:

```
npm install -g protractor cucumber webdriver
npm install 
```

(This assumes you've already installed node, npm, etc.)

Then update webdriver:

```
webdriver-manager update
```

This is only necessary the first time you run.

Next, start the webdriver:

```
webdriver-manager start
```

You also need a webserver for the HTML. One simple option is Python's
builtin `http.server`::

```
python -m http.server
```

Now you can run the tests:

```
protractor cucumberConf.js
```
