## Talk template

<img src="img/logo.jpg" />

Tiago Garcia @ [Avenue Code](http://www.avenuecode.com)

*tgarcia@avenuecode.com* <!-- .element: class="feature" -->

Feb 11th, 2014

---

## Agenda

 - The template
  - Installing
  - Working
  - Deploying
 - Your talk
  - Organization
  - The DO's
  - The DONT's
  - Tips

----

## Agenda

 - Contributing
 - Learn more
 - Conclusion
 - Assignment

---

## Prerequisites

- Markdown
- Reveal.js
- Grunt

---

## The template

1. The Avenue Code talk template is a responsive, web-based talk template.
1. This template is based on [Reveal.JS](http://lab.hakim.se/reveal-js).
1. All you need to do is to write your content in [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).
1. There are some [Grunt](http://gruntjs.com) jobs to automatize the build process.
1. It has <span class="feature">automatic code highlighting</span>, guessing the programming language you used.
1. Once it is described in <span class="feature">README.md</span>, the talk contents will also be available as the repository description which is a common format for tutorials.

----

## Setting up your repo

1. Sign in on GitHub
1. Fork the repository <https://github.com/acbr/talk-template>
1. Rename it to match your talk name (ex: <span class="feature">talk-design-patterns</span>)
1. Clone this repository
1. Navigate to its folder on the terminal

----

## Building and running

1. Install [Node.js](http://nodejs.org/)
1. Install [Grunt](http://gruntjs.com/getting-started#installing-the-cli)
1. On the repo folder, install the npm dependencies
```sh
$ npm install
```
1. Build it, serve it and monitor source files for changes
```sh
$ grunt
```
1. Open <http://localhost:8000> to view your talk

----

## Working

1. Open up <span class="feature">config.json</span> and fill your talk data such as title, author, email, date and description.
1. Open up <span class="feature">src/README.md</span> file and write your talk in plain <span class="feature">Markdown</span>.
1. In order to separate slides horizontally, use 3 dashes (---).
1. In order to separate slides vertically, use 4 dashes (----).
1. In order to call out attention, use the css class <span class="feature">feature</span>:
```
*WARNING* <!-- .element: class="feature" -->
```
```
<span class="feature">WARNING</span>
```
1. For every change, grunt will rebuild your talk and all you need to do is to refresh your page.

----

## Deploying

1. Make sure your build is not breaking.
  - You should see <span class="feature">Done, without errors.</span> in the terminal.
1. <span class="feature">git add</span>, <span class="feature">git commit</span> and <span class="feature">git push</span> to <span class="feature">gh-pages</span> branch.
1. You should see your talk in an address like:
  - http://<span class="feature">your-github-username</span>.github.io/<span class="feature">your-repo-name</span>
  - Ex: <http://acbr.github.io/talk-template>

---

## Your talk

 - Should last no more than 50 minutes, leave up to 10 minutes for questions.
 - Should not be too deep neither too superficial.
 - Give at least 3 reference links to be followed for further studies.
 - Give a challenge that would be solved using ideas that were covered on the talk.
 - It is ok to go a little bit far (forcing the attendee to do some research), but that should be optional.

----

## Organization

 - 1st slide: the cover, featuring your talk name, your name, the lecture date and AC logo.
 - 2nd slide: the agenda, in topics.
 - 3nd slide: the prerequisites of your talk.
 - From 4th slide on: your content
  - When content from the same topic doesn't fit on a slide -> grow it <span class="feature">VERTICALLY</span> by adding a slide below (----).
  - When you finish a topic and will start a different one -> grow it <span class="feature">HORIZONTALLY</span> by adding a slide to the right (---).
 - The 3 last slides: Conclusion, Learn more (with the reference links) and Challenge.

----

## The DO's

1. <span class="feature">BE BALANCED BETWEEN THEORY AND PRACTICE</span>. Your target is keeping the subject interesting for everybody.
1. <span class="feature">BE CONSISTENT</span>. Please watch some good screencasts in order to learn how to use your voice and conduct the talk.
1. <span class="feature">BE POLITE</span>. Don't use slangs neither bad words.
1. <span class="feature">BE OBJECTIVE</span>. Don't overexplain in such way you could cause confusion to your attendees.
1. <span class="feature">KEEP THE FOCUS</span>. Off-topic discussions are ok, but only if it doesn't disturb the natural flow of your content.
1. <span class="feature">BE PREPARED</span>. If you are going to use examples or live coding, make sure you have them all prepared beforehand.
1. <span class="feature">TRAIN</span> your full talk at least once before your talk.

----

## The DONT's

1. <span class="feature">DO NEVER SHOW PRIVATE CODE FROM THE CLIENT</span>. This is CRITICAL and can cause serious problems.
1. <span class="feature">DON'T BE ARROGANT</span>. Be humble and don't focus the talk on yourself.
1. <span class="feature">DON'T GENERALIZE</span>, specially stuff that you are not sure about.
1. <span class="feature">DON'T MAKE UP DATA</span>. Base yourself on trustable references.
1. <span class="feature">DON'T BE BORING</span>. Just be yourself. It is ok to joke around, but don't exaggerate.

----

## Tips

 - <span class="feature">ENJOY</span> your experience by creating the talk, because you will surely learn MUCH MORE than your attendees.
 - <span class="feature">BRING WATER</span> to drink while you present. You will certainly need it!
 - <span class="feature">BE OPEN</span> to receive questions and even criticism. You will learn a lot from them.
 - <span class="feature">ALWAYS</span> be polite when talking to your audience. This will always open doors for you.
 - People might come to you with questions and more complex cases after your talk. Consider it as a gift, it means you represent something good for them!

---

## Contributing

Should you wish to contribute, please be welcome to!

1. Fork this repository
1. Create a feature branch for your contribution
```sh
git checkout -b my-new-feature
```
1. Commit your changes
```sh
git commit -am 'Add some feature'
```
1. Push to the branch
```sh
git push origin my-new-feature
```
1. Create a Pull Request

---

## Conclusion

- This talk template rocks!
- Your life should be easier now.

---

## Learn more

1. [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
1. [Reveal.JS](https://github.com/hakimel/reveal.js)
1. [Grunt](http://gruntjs.com)

---

## Challenge

1. Make your awesome talk based on this template.
1. Push it to a gh-pages branch on your GitHub account.
1. Share the URL with the world!