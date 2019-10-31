# CPE 1040 - Introduction to Computer Engineering

## Assignment: micro:bit I/O 1

### 1. Summary

This assignment asks you to use the GPIO pins of the micro:bit to achieve external I/O, that is, I/O with devices/circuits that are not on the micro:bit itself. This is a lab assignment. You will be provided with a micro:bit breakout board to get you focused on programming and circuit building.

### 2. Requirements

#### 2.1 Analog output pin

1. Start with this SparkFun [breakout board hookup guide](https://learn.sparkfun.com/tutorials/microbit-breakout-board-hookup-guide). Build the circuit, using 3 LEDs of different colors. Remember the proper orientation of the LEDs (long leg toward higher voltage). Commit the JavaScript file to your assignment repository. Call it `original.js`. _Notice that you have to disable the on-board LEDs to work with the external pins (see the documentation for the [GPIO edge connector](https://tech.microbit.org/hardware/edgeconnector/)._
2. Modify the program to do something interesting with the 3 LEDs. Commit the modified JavaScript file to your assignment repository. Call it `new-program.js`.
3. **(Bonus)** Add more analog output LEDs and write a new program to drive them in an interesting way. Commit the modified JavaScript file to your assignment repository. Call it `more-leds.js`.

#### 2.2 Digital input pin

1. Keeping at least one analog output pin, open a digital input pin and hook it up to a TTL input button on the workstation. Light the external LED when you detect a 1 on the input button (that is, the button is _pressed_). Commit the modified JavaScript file to your assignment repository. Call it `digital-in.js`. Do you need a [_pullup resistor_](https://www.google.com/search?q=pullup+pulldown+resistor&oq=pullup+pull)?
2. **(Bonus)** Try to drive one of the internal LEDs **and** the external LED on the analog output pin **at the same time**. Commit the modified JavaScript file to your assignment repository. Call it `on-board-and-external-out.js`.

#### 2.3 Videos of operation

1. For each programming file, record a short video of the LED operation. Upload to [Imgur](https://imgur.com/).

2. **(Bonus)** Make one video out of the different clips and upload to [Imgur](https://imgur.com/).

### 3. Criteira for micro:bit JS programs

#### 3.1 Requirements
1. The file should have a name and the `.js` file extension.
2. A project [description](#description) should be included in this [README](README.md) file, and a leading comment in the JS file.

#### 3.2 Code quality
1. The program should have proper indentation.
2. Every block of code should contain inline comments, briefly describing its purpose and functionality.	
3. The program should have good structure, with asynchronous and synchronous code blocks properly differentiated. **Note:** You cannot have more than one `forever` loop.
4. Variables should be named in either of the following styles:
   1. `variable_name_of_underscore_delimited_lower_case_words`, or
   2. `variableNameInCamelCase`

#### 3.3 JavaScript
1. Variables should be declared with [full static data types](https://makecode.microbit.org/javascript/types).	
2. Programmatic functionality should be encapsulated in [functions](https://makecode.microbit.org/javascript/functions), and, optionally for **bonus** points, [classes](https://makecode.microbit.org/javascript/classes).	
3. Functions in JavaScript are [1st class objects](https://developer.mozilla.org/en-US/docs/Glossary/First-class_Function). All event constructs like `onButtonPressed` and `onGesture` take functions as arguments.	
4. A maximum variety of JS language constructs (loops, conditionals, various operators, encapsulations, event handling, etc) should be used.

#### 3.4 micro:bit			
1. Use of buttons	and/or guestures.
2. Sensible display update.
3. Non-trivial functionality.	
4. Control complexity.

## Resources

### micro:bit 

1. micro:bit [lessons](https://makecode.microbit.org/lessons).
2. micro:bit [ideas](https://microbit.org/ideas/).
3. A list of some more [advanced projects](https://www.itpro.co.uk/desktop-hardware/26289/13-top-bbc-micro-bit-projects).
4. The assembled micro:bit resources at the [awesome micro:bit list](https://github.com/carlosperate/awesome-microbit).
5. micro:bit [reference](https://makecode.microbit.org/reference), and specifically the [pins](https://makecode.microbit.org/reference/pins) section.
6. The technical documentation for the micro:bit [GPIO edge connector](https://tech.microbit.org/hardware/edgeconnector/).

### Github

1. Github Tutorial for Beginners ([webpage](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)).
2. Github Basics for Mac and Windows ([video](https://www.youtube.com/watch?v=0fKg7e37bQE)).
3. git & Github Crash Course for Beginners ([video](https://www.youtube.com/watch?v=SWYqp7iY_Tc)).
4. Introduction to Github for Beginners ([video](https://www.youtube.com/watch?v=fQLK8Ib_SKk)).
5. About `git` ([webpage](https://git-scm.com/about)).
6. `git` [documentation](https://git-scm.com/doc) (webpage, book, videos, reference manual).
7. [Github markdown cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

### JavaScript

1. Technically, the language which is used side-by-side with Blocks in the Makecode environment is a subset of [TypeScript](https://makecode.com/language), which itself is a superset of JavaScript (technically, [ECMAScript](https://www.ecma-international.org/ecma-262/10.0/index.html#Title)), with some JS features not implemented in Makecode.
2. The limited [JavaScript mini-tutorial](https://makecode.microbit.org/javascript) in Makecode. Make sure you read it but that can't be your only reference.
3. Official [TypeScript documentation]():
   1. TypeScript in 5 min [tutorial](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html). _**Highly recommended!** You will need to [download](https://www.typescriptlang.org/index.html#download-links) and install an integrated development envinronment (IDE). The two that I recommend are Visual Studio Code from Microsoft and WebStorm from JetBrains._
   2. The full documentation and reference is under _Handbook_. Bear in mind that you are drinking from the hose. Don't be surprised if not everything is presented in a strictly incremental manner.
   3. The Microsoft TypeScript page on [Github](https://github.com/microsoft/TypeScript), including the [TypeScript language sepecification](https://github.com/microsoft/TypeScript/blob/master/doc/spec.md).
4. In-browser TypeScript [playground](https://www.typescriptlang.org/play/index.html). Note that micro:bit specific code will not run, but you can still play. _Start making the distinction between a generic multi-purpose programming language (TypeScript) and functionality (packages, libraries, objects, etc.) that is specific to a particular device (micro:bit), though written in the same programming language._
5. A pretty good and very palatable JS tutorial with in-browser coding, by [Codecademy](https://www.codecademy.com/learn/introduction-to-javascript).
6. Extensive and detailed [JS tutorial](https://javascript.info/), with some advanced material thrown in. _**I like this one!**_
7. The most authoritative JS resource on the Web, including tutorials and reference, by [Mozilla](https://developer.mozilla.org/en-US/docs/Web/JavaScript).

---

### Description

TODO: Your project description, in your own words. _Clarity and grammatical correctness are required._
