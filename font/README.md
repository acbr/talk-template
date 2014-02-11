Grunt: The Build Tool for Javascript
====================================

Rafael Guedes

*rguedes@avenuecode.com*

Avenue Code - 2014

---

## Agenda

 - Overview
  - Usage
  - Installation
  - Setup
 - Grunt syntax
  - Sample Gruntfile
 - Demo Session
 - Conclusion
  - Assignment

----

## Prerequisites

- Node
- Node Package Manager (NPM)

---

## Overview

tl;dr
> in one word: automation

----

## Usage

 - JS/CSS Lint
 - Uglifying
 - Minifying
 - Concat static files
 - Hot deploy
 - Dev/Test Server

----

## Instalation

```
npm install -g grunt-cli
npm install grunt --save-dev
```
*.. and that's it :)*

***

#### package.json

```
"devDependencies": {
    "grunt": "~0.4.1",
...
```

----

## Setup

 1. Configure existing tasks
 2. Load needed plugins
 3. Create own tasks
 4. Define aliases and combine tasks

---

## Grunt syntax

> All configuration code is done inside Gruntfile.js located at project root

----

## Creating tasks


```
grunt.registerTask(taskName, [description, ] taskFunction)
```

Ex:
```javascript
module.exports = function(grunt) {
  grunt.registerTask('foo', 'My "foo" task.', function(a, b) {
    grunt.log.writeln(this.name, a, b);
  });
}
```

```
$ grunt foo
  logs: "foo", undefined, undefined

$ grunt foo foo:bar
  logs: "foo", "bar", undefined

$ grunt foo:bar:baz
  logs: "foo", "bar", "baz"
```

----

## Configuring tasks

```
grunt.initConfig({
  jshint: {
    foo: {
      src: ['app/js/a.js', 'src/aa.js']
    },
  },
  concat: {
    options: {
      src: ['src/bb.js', 'src/bbb.js'],
      dest: 'dest/b.js',
    },
  },
  uglify : require('path/to/my/settings'),
  ...
```

----

## Configuring Tasks (cont)

```
...
watch: {
    options: {
      interrupt: true
    },
    files: [
      'app/js/**/*.js',
      // Exclude minified files
      '!app/js/min/*'
    ],
    tasks: [
      'jshint:foo', 'uglify', 'notify:uglify', 'concat',
      'notify:concat', 'jdd', 'notify:jdd'
    ]
  }
});
...
```

----

## Configuring Tasks (cont)

```
...

grunt.loadNpmTasks('grunt-contrib-uglify');
grunt.loadNpmTasks('grunt-contrib-watch');
grunt.loadNpmTasks('grunt-notify');

grunt.registerTask('default', ['jshint:foo', uglify', 'concat', 'watch']);
...
```

Remind: packages *must* be declared in package.json

---

## Demo Session

---

## Conclusion

 - Powerful build tool
 - High level of customization
 - Leads to productivity improvements

----

## Assignment

Create a task (you are free to set its name) with following rules:

 1. Watch for changes on you source code
  1. In case of .css change, launch a CSS lint task
  2. In case of .js change, launch a JS lint task
 3. Run uglify & minify tasks and move the result file(s) to /min/
 4. Notify the user that the flow is done


**The task should FAIL if a lint rule is broken.**

Submit the code on your Github account

---

## Thank you!

Questions?