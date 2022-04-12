# Quiz 4 - we came; we built; we interacted

This is the last `quiz`... you've made it through:

- Quiz 1: `setup and soundbeats`
	- do you remember your first template clone into robots?
  - what about your reaction to `how do I make an emotion with code`? 
  - or changing `just one thing`?

- Quiz 2: `classy robot family`
	- do you know where your `classy` children are?
	- what about their parents? 
	- do you remember how similar `OOP` is when we looked at `processing.py` vs `p5.js`?

- Quiz 3: `message in a bottle`
  - you are no longer limited to `one file - one location`!
  - smile! There will be a surprize sent to your `GPS` next week!
  - interacting digitally across space and time (in just a few lines..)

---

## Let's look back

Our notes from last class (_THE_ [`last class`](last-class.md)) might be helpful to reference while answering the `Quiz 4` questions.

Here we go! Just answer in this `readme.md` file - you can even do it online, remember? (grab a copy of the repo first though!). 

>
> You do not need to write long answers. In fact, keep them short, keep them clear. 
>
> Point-form, jot-notes, paraphrasing, snippets, links.
>

---

### Week 01

1. setup
   - What is a repo and why do we use them?
   > A Github Repositiory is a collection of files and various versions of a project.
   > These files are pushed from local onto the cloud for storage, and potential reroll
2. version control.
   - Why do we use version control? How did you manage making use of this? Be specific.
   > Version control keeps track of changes in case of need for referral.
   > This means in case a current file is corrupt, it can be rerolled, or to simply compare versions.
3. processing
   - Why is processing similar across _at least_ three languages (Java, Python, JavaScript)? What might be the point of this?
   > Processing uses Java and Python, and used to have a JavaScript port.
   > Java and Python are Object Oriented, wjile JavaScript can imitate it.
   > Since Processing can be considered a "simpler" version while sharing syntactical features, it is a good beginner learning tool.

---

### Week 02

1. IDEs
   - What IDEs did you use over the last 3.5 months?
   > Processing, PyCharm, Visual Studio Code, Replit
   > These are the IDEs that _I_ used
2. UI & UI Elements
   - Give me a specific example of where you considered UI in any of your course content submissions?
   > For Lab 4, I used a UI to get feedback from user's clicks, and then to display response
3. JSON
   - What _exactly_ is JSON? Decide how you want to answer this.
   > It stands for _JavaScript Object Notation_
   > JSON is data format used to transmit data between web apps and servers.
   > It uses `name : data` pairs
4. CLI & GUI
   - Give me at least 3 ways we used GitHub and explain the difference between local and remote copies of a repo.
   > We used GitHub to store repo versions (single and multiple contributors), to host webpages (for AR), and to allow Heroku to access code to run
   > Local refers to the repo being stored directly on the user's computer, remote means it could be stored on another person's computer
5. debug
   - What magical number-letter combo helps us debug in the browser? (What is a cross-origin error?) How can I display console content?
   > F12
   > A CORS error occurs when CORS is disabled/blocked. This prevents cross-domain resource sharing due to security reasons.
   > Console content can be printed (in JS) with `console.log("message");`. Syntax varies with languages.

---

### Week 03

1. Browsers, extensions
   - Interaction with the browser through extensions required at least 2 things. Tell me what you think they are. There is a correct answer, and I talked about it in a January video.
   > Permissions and requirements: Written in `manifest.json`.
   > This file is essential to the extension as it holds critical information.
2. DOM, selectors, elements
   - How are these related? 
   > DOM selectors are used within the document to select elements with JavaScript.
   > Can be used like this: `thing.function(selector)`.
   > Selector Examples: `p`, `#id`, `.class`.
3. JavaScript OOP
   - Show me 2 specific ways you used an OOP style in your course content submissions. Where did I use OOP in my p5.js updates?
   > In Processing from the robot family, objects inheritied from parents.
   ```python
   class Bot2(Bot):
    def __init__(self, si, sh, gen, col, name):
        super(Bot2, self).__init__(si, sh, gen, name)
        self.col = col
        self.st = grey
   ```
   > In Node JS while packaging data in JSON format
   ```js
    let data = {
    "x": x,
    "y": y
  };
   ```
   > In P5.js, was used in:
   ```javascript
   function _inherits(subClass, superClass) {
            if (typeof superClass !== 'function' && superClass !== null) {
              throw new TypeError('Super expression must either be null or a function');
            }

            subClass.prototype = Object.create(superClass && superClass.prototype, {
              constructor: {
                value: subClass,
                writable: true,
                configurable: true
              }
            });
            if (superClass) setPrototypeOf(subClass, superClass);
          }

          module.exports = _inherits;
        }
   ```
   > and also elsewhere

---

### Week 04

1. Python
   - Show me where you completed the `try these` instructions from [Feb 3](https://github.com/robots-make-art-too/EECS_1720/tree/main/General-Content/Content_by_Week/Week04/Week04-live_code)
   > `constantFactor` affects the radius of the circles
   > `circleSize` is the radius of the circle
   > Yes, the shapes can be modified by changing `constantFactor`
   > The shapes grow over time and recycle, so no, it makes little visual difference
   > Relocate the smallest shape by changing the first two arguments in
   ```java
      ellipse(width/2,height, circleSize, circleSize)
   ```

   > Changing that value in lerp colour will affect the gradient colour distances. Changing a float to an integer here will effectively make it a solid colour
   > Use `lerpColor` on a diagonal vector
   > Will need to use multiple shapes stacked seamlessly to give the illusion of multiple gradients on one shape. This can be done through `beginShape`, and using a `for` loop to change which gradient is applied to the current shape.
   > If replicated correctly, there should be no notable differences.
2. Describe and list common attributes of any object-oriented programming language.
   > Encapsulation: Bundling data into one object or unit (classes).
   > Abstraction: Classes can have private and public identifiers for the scope limit.
   > Inheritance: Child objects can inherit features of its parent (classes)
   > Polymorphism: Child objects can modify its class while still inheriting features from parents

---

### Week 05

1. Python OOP
   - Write a python class for a `classy robot` that has the following: a name, an age, and can start and stop dancing when you clap. You can do it in under 10 lines (it can be pseudo-code like).
   ```python
   class classyRobot(object):
      def __init__(self, name, age):
         self.name = name
         self.age = age
      def clap (self):
         self.dance = not self.dance
   ```
2. APIs
   - What API did you connect with in Lab 2? Briefly explain how you integrated interactivity within your code. 
   > I used the Discord Bot API. The bot is able to respond to messages by users within the server based on the "wake-up token" followed by a command, `$`.

---

### Week 06

1. server-client
   - Give me an example of an interaction done `client-side` and an interaction done `server-side`.
   > Client side displays data it receives from the server to the user.
   > Server side communicates between clients and decides what data to send each client
2. local hosting
   - what is the difference between dragging an index.html file into your browser and opening an index.html file using localhost? Do you remember the number equivalent to localhost? 
   > They are treated similarly, except in certain cases, like Cross-Origin Resource Sharing (not allowed in Chrome for the file alone).
   > Localhost: `127.0.0.1:8000/`

---

### Week 07

1. GitHub pages
   - What is a `deployment` in this context? What is a branch and why are they used for contributing to repos? 
   > Deployment used by Heroku to host the GitHub code on its server
   > Branches allow multiple version to exist on the same level (for comparisons and merges)
2. Augmented Reality
   - What makes AR possible? What is needed in a code context?
   > Camera data is needed in order to project something onto it and to react to changes
   > Location data is needed to orient and position augmented objects
   > The object to augment

---

### Week 08

1. aesthetics
   - Give me a specific example of where you considered aesthetic design in any of your course content?
   > Lab 4 draws a Rainbow onto the screen procedurally, and will interactively respond to user
2. APIs for extending integration
   - Identify where in _your_ code, for Quiz 1, Quiz 2, Quiz 3, Lab 1, Lab 2, Lab 3 that either you used an API or where you _could_ integrate an API (it could be that we added API access in the lecture example and you used the same - still identify this).
   > Quiz 1 calls from external source in the html for the beats
   > Quiz 2 is solely focused on inheritance, which is part of OOP. Could use API if importing from external source code 

---

### Week 09

1. OOP elements & interactive JavaScript
   - How did we interact with webpage elements using code?
   > Dealt with JS and HTML thorugh DOM. Can modify elements of the page (HTML) with JS
2. integrating multi-code & external content
   - What kind of event-based interactions are possible in web-based applications?
   > Mouse-click, Key-press/Keystroke, Button-press are the common ones. 

---

### Week 10

1. Levels of location - local to geo
   - How did we instantiate multiple geo-locations and dynamic object loading in our AR code?
   > Using latitude and logitude
2. app hosting
   - What is important about constructing an app? How does this relate to its `environment`?
   > App needs to be run in an environment. There are many hosting environments provided online
   > The hosting environment is responsible for handling app functions

---

### Week 11

1. interaction along the virtuality-reality continuum
   - Why are `id`'s important for interaction?
   > ID attribute is unique to an element and can be used to select it. Interactive apps may use this to determine which elements to change when an event is triggered.
2. Tell me about 2 WEB-APIs and how you could integrate them into any of your course content submissions? Give me a line or two of code.
> Barcode Detection API: `qr_code`
```javascript
  barcodeDetector.detect(imageEl)
    .then(barcodes => {
      barcodes.forEach(barcode => console.log(barcode.rawData));
    })
    .catch(err => {
      console.log(err);
    })
```
> Streams API: `Request`
```javascript
   const fetchResponsePromise = fetch(resource [, init])
```

---

### Week 12

1. tracking
   - Briefly describe how the complexity changes between image, facial, and hand, tracking? 
   > Detecting an image usually requires pixels of a target image to match pixels from camera
   > Detecting a face requires there be prominent features present that represent a face
   > Detecting and tracking a hand requires the program to be able to distinguish different hand positions (which vary wildly)
2. OOP, ECS, DOM
   - What are these acronyms? How are they related?
   > Object Oriented Programming, Entity Component System, Document Object Model
   > ECS prioritises composition over inheritance (compared to OOP), DOM is for web documents
3. How do you register a component in A-Frame, and show me how to relate this component to data flow, API, and useage. 
> Register component with `AFRAME. registerComponent()`
```javascript
   AFRAME.registerComponent('message', {
   init: function () {
      //stuff
   }
   });
```
> Components must be registered before they are used. Data can flow between components. API can also provide data and improve data flow.

---

## That's all!

(did you ever watch the movie trailer embedded somewhere in your Quiz 3 readme.md [files](https://github.com/robots-make-art-too/Quiz_3-message-in-a-bottle)?)

### Do you want a bonus? 

Do one, some, or all, of the following before the end of April:

Publish an A-Frame component.
- <https://www.npmjs.com/package/angle>

Publish your browser extension. 
- [microsoft](https://docs.microsoft.com/en-us/microsoft-edge/extensions-chromium/publish/create-dev-account)
- [chrome](https://developer.chrome.com/docs/extensions/)
- [firefox](https://addons.mozilla.org/en-CA/developers/)

Release a version of your Bot.
- <https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository>


---

Psst: Every 100 days _another_ `100 days of code` starts ... 
> 5ZOO5ZGA77yB5aSq5aSa6Zeu6aKYIPCfmII=