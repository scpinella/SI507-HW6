# JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give.

**To complete and submit this assignment, you should:**

* Fork (and clone) this repository
* Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <u>each</u> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours.

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment
* List everyone's names and uniqnames who have worked on this assignment with you, **including your own name, but make sure YOUR name is first and bold**
* **Samantha Pinella (spinella)**


## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **This is just an example question.**

This is what an example answer should look like. If you want to include some code, which you probably don't have to do, you can, like this:

```js
Some JavaScript code
```

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**

A code comment is statement explaining or organizing the code. It is indicated by ```//``` at the beginning of the text in JavaScript.


* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**

The JavaScript in this assignment is part of an .html file. The .html file can be opened with a browser (the default on my computer is chrome). The browser knows which code is JavaScript and not html because it is inside a ```<script> </script>``` box. In my version of chrome, you can look at the console by using rightclick + Inspect and then navigating to the console window.

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**

`console.log(text)` will print your text in the console. This is useful for debugging because it won't affect how the page is viewed by visitors and is less annoying than a pop up box.

`alert(text)` will print your text in a pop up box. This is a good place to put really important information.

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**

You need to comment out line 13 which says ```alert("hello");```. To instead have code that gives the current date and time, insert ```alert(new Date());``` in line 14.

* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**

You just have to replace the string "A name" in `document.querySelector('h1').innerHTML = "A name";` with your own name in quotes.

* **What does the word `document` represent in this code? Explain briefly.**

The DOM (document object model) represents the structure of the page. Thus `document` is what JavaScript calls this object, so you use document.<something> to access elements (or methods) of the page.  


* **What is happening in line 12 (
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**

This query counts the number of elements that are in any list. It just looks for items with the <li> (list) tag.

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**

The background would be white, I removed the line ```body.style.background = "#CCEE00";``` and that made the background white.


* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**

It's because the paragraph tag ```<p>``` was restyled:

```p{
	background-color: #b3b3b3;
	border: 3px solid #FFFFFF;
	padding: 3%;
	font-size: 1.1em;
	line-height: 1.5;
}
```
You can change the background color by changing ```#b3b3b3``` and the border color by changing ```#FFFFFF```. I changed the border color to `#00ccff`.

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**

The page already has the feature that if you copy "University of Michigan", the text "Go Blue" appears at the bottom of the page. There is a comment in the file explaining how this is done. I wrote a function called copyFunction2 which is defined the same way as copyFunction except with "O, Canada" in place of "Go Blue!". Then where McGill University appears on the page, I linked it to copyFunction2: ```<li oncopy = "copyFunction2()">McGill University</li>```.

* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```
**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```
The function handleClick will create a pop-box with that says 'hello' when it is called. Then in the code for the page, the tag <button> creates a clickable button; `onclick=handleClick()` instructs the page to execute handleClick when the button is clicked. The button says Wow on it because the text ```Wow``` is inside the button tag.



* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**

This is now added, the button is next to the Wow button.



### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**


* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**

It's because these colors were set in the style part of the code:
```
		<style type="text/css">
    .error{
        color: red;
    }
    .good {
        color: blue;
    }		
```
And then later when there is an error, the result is pointed back to this style where you see ```class = "error"``` in the line ```$("#result").html('<p class="error">Not valid!</p>').show().fadeOut(10000);``` and similar for when the input is valid.


* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**

I first googled 'regex variable' and learned that 'regex' means 'regular expression'. That made it easier to look up what is a regular expression; I learned that it is sequence of characters to look for in a search. So then the line `var regex = /^[a-zA-Z]+$/;` is saying that the regular expression is all letters, upper and lower case. This will be how JavaScript tests that the input is only one word.

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**

Python needs tabs/indentations to identify blocks of code while JavaScript uses brackets. An if statement in JavaScript will look like
```
if(thing == other thing){
	when true do this
} else { otherwise do this
}
```
.

* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**

It controls how long the text is on the page. I changed it to 1000000000 and the text stayed a long time (unsure how long, I didn't wait for it to fade).

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```
$(document).ready(function(){
    $("form").submit(function(event){
```

From the reading, I think the syntax ```function(){}``` is a way of executing a nameless function. Then ```(document).ready(function(){})``` is specifying something to execute when the page loads. The word ```"form"``` points to the line ```<form action="" method="post" id="users">``` and sets up another nameless function to execute when text has been submitted in the textbox.



* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
	* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.
