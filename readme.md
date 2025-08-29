## Create Readme

You have to create a `Readme.md` file. and write down following questions. Dont Try to copy paste from AI Tools. Just write what you know about these. If you don't know , then search , learn , understand and then write.

### 6. Answer the following questions clearly:

1. What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?

Answer: getElementById: Selects a single element by its unique id. Returns only one element.

getElementsByClassName: Selects all elements with the same class name. Returns an HTMLCollection.

querySelector: Selects the first element that matches a CSS selector.

querySelectorAll: Selects all elements that match a CSS selector and returns a NodeList.

2. How do you **create and insert a new element into the DOM**?

Answer:  To create a new element we use document.createElement().
We can set text or attributes, then insert it into the DOM using methods like appendChild(), append(), or prepend().

const newDiv = document.createElement("div");
newDiv.textContent = "Hello, I am a new element!";
document.body.appendChild(newDiv);



3. What is **Event Bubbling** and how does it work?

Answer: Event bubbling means when an event happens on an element, it first runs on that element and then propagates upward to its parent, grandparent, and so on until the document root.
For example, clicking on a button also triggers the click events of its parent containers unless stopped.

4. What is **Event Delegation** in JavaScript? Why is it useful?

Answer: Event delegation is a technique where a single event listener is added to a parent element to handle events on its child elements.
This is possible because of event bubbling.

Why it is useful?

Saves memory and improves performance (fewer event listeners).

Makes it easier to handle dynamically added elements.

5. What is the difference between **preventDefault() and stopPropagation()** methods?

Answer: preventDefault() → Stops the default behavior of an element (e.g., prevent a link from navigating or stop a form from submitting).

stopPropagation() → Stops the event from propagating to parent elements (prevents bubbling or capturing).