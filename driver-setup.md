# Setting up a driver

Running selenium automation tests locally requires a browser (safari, firefox, chrome, internet explorer, phantomjs,
etc) and sometimes a browser plugin or external shim binary. You will need to complete one or more of the below
installations depending on which browser/s you want to automate.

## Using phantomjs and ghostdriver

By far the quickest way to get a test to run locally is by installing phantomjs.

Mac folks will find that "brew install phantomjs" works quite well to install phantomjs. Just make sure the installation
is somewhere on your $PATH environment variable.

## Using Firefox

All that is necessary in order to use Firefox is that you've got an appropriate version ([Version 35](https://ftp.mozilla.org/pub/firefox/releases/35.0/)) of the Firefox browser for the
version of selenium-webdriver that `nemo` is currently using. Sometimes, you may need to forego a Firefox update in order
to ensure that your `nemo` test environment continues to work.

## Using Chrome

To automate the Chrome browser, you will need the chromedriver binary visible in your computers `$PATH`

Find the latest here:
http://chromedriver.storage.googleapis.com/index.html

For OS X, if you're using [Homebrew](http://brew.sh/), there's a [Homebrew formula](http://brewformulas.org/Chromedriver),
which makes installation much easier.  To install, it's simply `brew install chromedriver`.

## Using Safari

As of this edit, there is an issue where the latest selenium-webdriver client supports Safari, but does not support Chrome or
Firefox. Until this situation is resolved, and unless automating Safari is a REQUIREMENT, avoid it.

## Other drivers

There are other "drivers", like Appium or ios-driver, which can be used to automate iOS/Android simulators and devices.
That setup is covered elsewhere.


