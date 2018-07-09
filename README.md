#Packages

##Node
WTF is Node?
It's a Javascript Engine that can run as an standalone program in the terminal and servers, Download it from https://nodejs.org/en/download/

##NPM
WTF is **NPM**?
it's the Node Package Manager
```
npm init
```

##Mocha
WTF is **Mocha**?
it's a Test-driven develoment FrameWork that implements Behavior-driven development

```
npm install mocha --save-dev
```

##Chai
WTF is **Chai**?, it's an Assertion library.

```
npm install chai --save-dev
```

##Karma
WTF is **Karma**? is Test launcher that can run browser tests
```
npm install  karma karma-chrome-launcher karma-mocha karma-chai --save-dev
```

#Configurations

Generate default config for **Karma**
```
karma init
```

Open the generated **karma.conf.js** , change 'Chrome' for 'ChromeHeadless'.
```
browsers: ['ChromeHeadless'],
```

And add 'chai' to Frameworks list
```
frameworks: ['mocha', 'chai'],
```

Update **package.json** with:
```
"scripts": {
    "test": "karma start --single-run"
}
```