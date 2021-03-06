### ESLINT Configuration
Our [ESLint configuration](https://github.com/teamhacksmiths/project-resources/blob/master/configuration/.eslintrc) uses the eslint-config-airbnb configuration file, the babel-eslint parser and has several small configuration tweaks that we have determined work well for us and our projects.

Please download the [.eslintrc file](https://github.com/teamhacksmiths/project-resources/blob/master/configuration/.eslintrc) and put it in the root directory of your project to get started.

#### Configuration Tweaks
[eol-last](https://github.com/eslint/eslint/blob/master/docs/rules/eol-last.md): This plugin forces a new line at the end of a non-empty file.

[func-names](http://eslint.org/docs/rules/func-names) Forces that you add a function name after the function declaration.  In the case below, the function should be written as:
```
Foo.prototype.bar = function bar() {

};
```

versus
```
Foo.prototype.bar = function() {

};
```

The reason to do so is to ensure that the function has a name in the stack trace.

[comma-dangle](http://eslint.org/docs/rules/comma-dangle). With this rule enabled, we warn when there are extra dangling commas.  This is the main rule we disagree with when it comes to AirBnb's style guide.
