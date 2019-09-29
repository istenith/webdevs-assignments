# #0
Abhay is assigned a task to design FAQs(Frequently Asked Questions) webpage for
his school, it would be nice if you help him with this task.

Abhay being a long-time C++ programmer,
likes well-structured code. He wishes that code is structured such that the Question
and its Answers lie in the same group. This is what he came up with.
```html
<div class="faq">
	<p class="question">
		This is a question
	</p>
	<p class="answer">
		This is an answer
	</p>
</div>
```
He advocates to use `class` over `id` as there are going to be many `faq`, `question` and `answer`.

See `class` vs `id` HTML.

However he is way behind schedule, he needs your help to get back on it.

As he is going to maintain the website afterward there are **best practices** you should follow which will make it easy for him.
- variable names
	- relateable

Let's get started.

Your 0th task is to make this page functional, as you can see the above-mentioned code is not complete.

Todo
- Add basic HTML structure
- Add **title** to the page

# #1
As per requirements, users should be able to easily questions from answers.

An easy way to do that would be to give them different colors.

Add the required embedded `CSS` to achieve this, using the style tag.

**To study**

- HTML
	- style tag
- CSS
	- selectors
	- `color`

# #2
Let's face it, the page looks ugly.

A part of it is due to fonts, default fonts are not so beautiful.
Embed fonts of your choice from a [CDN]() like [Google Fonts](https://fonts.google.com).
Questions, being the main focus, can be made bold.

**To study**
- Embedding fonts HTML
- CSS
	- `font-family`
	- `font-weight`

# #3
Abhay is lazy. He doesn't like that he has to add `Q.` at the start and `?` at the end of every question. So he has to write 
```html
<p class="question">
	Q. My real question?
</p>
```
Find a way that he has to only write
```html
<p class="question">
	My real question
</p>
```
and `Q.` and `?` are added automatically.

Being lazy he also doesn't like that he has to capitalize the first letter of question/answer**(not after the full stop)** but his teacher needs him for proper English.

**To study**
- Pseudo-elements CSS
	- `after`
	- `before`
	- `content`
- Pseudo Classes
	- `first-letter`

# #4
There a lot of questions in the world and a lot of answers.
> Everything has a reason, you just have to be smart and persistent enough to find it.

There are going to be many questions on Abhay's page too.
So that users of this page don't get overwhelmed, Abhay has come up with an idea
that answers can be made transparent to some extent (not invisible) until users,
hovers over answer to reveal it fully.


Abhay is now concerned that, it is too much to maintain HTML and CSS in the same file.
Comment out the style tag and move styles you added to an external `.css` file,
and link that in your HTML.

**To study**
- CSS
	- Pseudo-classes
		- `hover`
	- Colors and Backgrounds
		- `opacity`
- HTML
	- Linking External CSS file

# #5
Dimming answers isn't cutting it, on further surveys, he found that FAQs page
still looks very huge and that is overwhelming users.

You have to provide a solution such that only questions are visible initially,
with answers consuming no space,
and once the user clicks a question only then should its answer become visible.

**To study**
- JavaScript
	- Selecting elements by class
	- loops
			- `forEach` or `for`
	- Adding Event listeners
	- Selecting Children
	- adding, removing, toggling classes
- CSS
	- `height`

# #6
Now answers become visible when the respected question is clicked, but users still
have to hover to increase the opacity of the answer. This is a bug! and

> Bug for one, feature for another.

Abhay notices that answers have **keywords**, that are important points of an answer,
he marks them by wrapping in `strong` tag as
```html
<strong> important phrase </strong>
```

When the user clicks the question he/she should be able to view these keywords in full opacity,
when the user hovers over the answer then the whole answer should get full opacity.

# #polishing
Everything pops into existence! Add some transitions to make things a bit smoother.
Answers should grow gradually, colors transition smoothly.

Search for transition times that are smooth but don't make the system feel too slow.

**To study**
- CSS
	- `transition`

# #bonus
Try to do this without JavaScript

**To study**
- Checkbox HTML
- Sibling selectors CSS


---
[Go to all assignments](../assignment_list.md)
