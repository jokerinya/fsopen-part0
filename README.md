# fsopen-part0

> Helsinki University [Full Stack Open Course](https://fullstackopen.com/) Part0

# Exercises

> ## Exercises 0.1.-0.6.

The exercises are submitted via GitHub, and by marking the exercises as done in the [submission application](https://studies.cs.helsinki.fi/stats/courses/fullstackopen).

You can submit all of the exercises into the same repository, or use multiple different repositories. If you submit exercises from different parts into the same repository, name your directories well. If you use a private repository to submit the exercises, add `mluukkai` as a collaborator to it.

One good way to name the directories in your submission repository is as follows:

```bash
part0
part1
    courseinfo
    unicafe
    anecdotes
part2
    courseinfo
    phonebook
    countries
```

So, each part has its own directory, which contains a directory for each exercise set (like the unicafe exercises in part 1).

The exercises are submitted **one part at a time**. When you have submitted the exercises for a part, you can no longer submit any missed exercises for that part.

## 0.1: HTML

Review the basics of HTML by reading this tutorial from Mozilla: [HTML tutorial](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics).

_This exercise is not submitted to GitHub, it's enough to just read the tutorial_

## 0.2: CSS

Review the basics of CSS by reading this tutorial from Mozilla: [CSS tutorial](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics).

_This exercise is not submitted to GitHub, it's enough to just read the tutorial_

## 0.3: HTML forms

Learn about the basics of HTML forms by reading Mozilla's tutorial [Your first form](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form).

_This exercise is not submitted to GitHub, it's enough to just read the tutorial_

## 0.4: New note

In chapter [Loading a page containing JavaScript - review](https://fullstackopen.com/en/part0/fundamentals_of_web_apps#loading-a-page-containing-java-script-review) the chain of events caused by opening the page https://studies.cs.helsinki.fi/exampleapp/notes is depicted as a [sequence diagram](https://www.geeksforgeeks.org/unified-modeling-language-uml-sequence-diagrams/)

The diagram was made using [websequencediagrams](https://www.websequencediagrams.com/) service as follows:

```
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
server-->browser: HTML-code
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
server-->browser: main.css
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js
server-->browser: main.js

note over browser:
browser starts executing js-code
that requests JSON data from server
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
server-->browser: [{ content: "HTML is easy", date: "2019-05-23" }, ...]

note over browser:
browser executes the event handler
that renders notes to display
end note
```

**Create a similar diagram** depicting the situation where the user creates a new note on page https://studies.cs.helsinki.fi/exampleapp/notes when writing something into the text field and clicking the _submit_ button.

If necessary, show operations on the browser or on the server as comments on the diagram.

The diagram does not have to be a sequence diagram. Any sensible way of presenting the events is fine.

All necessary information for doing this, and the next two exercises, can be found from the text of [this part](https://fullstackopen.com/en/part0/fundamentals_of_web_apps#forms-and-http-post). The idea of these exercises is to read the text through once more, and to think through what is going on there. Reading the application [code](https://github.com/mluukkai/example_app) is not necessary, but it is of course possible.

## Solution!

![0.4-New note](0.4-New%20note.png)

## 0.5: Single page app

Create a diagram depicting the situation where the user goes to the single page app version of the notes app at https://studies.cs.helsinki.fi/exampleapp/spa.

## Solution!

![0.5-SPA](0.5-Single%20page%20app.png)

## 0.6: New note SPA

Create a diagram depicting the situation where the user creates a new note using the single page version of the app.

## Solution!

![0.6-New note(SPA)](<0.6-New%20note%20(SPA).png>)

---

This was the last exercise, and it's time to push your answers to GitHub and mark the exercises as done in the [submission application](https://studies.cs.helsinki.fi/stats/courses/fullstackopen).
