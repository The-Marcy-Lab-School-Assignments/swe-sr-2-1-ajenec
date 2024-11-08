# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:

- Examples of semantic and non-semantic tags
- The differences between semantic and non-semantic tags
- The benefits of using semantic tags (when possible)

### Response 1

Tags like `<header>` , `<article>` , and `<footer>` are semantic because they specify the role of the content on them. Tags like `<div>` and `<span>` are non-semantic tags because they can structure content without a specific meaning about the content they contain. The difference between semantic and non-semantic tags is that semantic tags describe the content within them. Non-semantic tags only structure content without adding meaning to it. Some benefits of using semantic HTML tags are that they make the code clearer, it's easier to add new elements in the future, and help with accessibility.

## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

### Response 2

Some ways to make your website more accessible are using semantic HTML to help screen readers understand website content, offering alternative versions of the website content, having good color contrast, including keyboard navigation to ensure that the website navigation can be done with keyboard shortcuts, and testing your website on different platforms. It is important for developers to create websites that meet accessibility standards because it ensures that anyone can interact with the website content regardless of any disability. Having a website that meets accessibility standards allows someone with disabilities to have the same user experience as someone who doesn't.

## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;">hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

### Response 3

It could be useful to write inline styles to create quick HTML or for styles that you are using temporary styles. However, putting your styles in a CSS file makes it easier to revise the website and allows future programmers to modify your website.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

- An explanation of the concept of "classes" and "ids" with an analogy.
- An example of the usage using an HTML code block and a CSS code block.
- An explanation of the syntax using the terms: **attribute**, **selector**

### Response 4

Classes are like groups because multiple elements can have the same class. Ids are like names because similar to names, each element can only have one id and each page can have one element with that id.

```html
<!--HTML Example-->
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <h1 class="city" id="myHeader">New York City</h1>
    <h2 class="city">London</h2>
    <h3 class="city">Paris</h3>
  </body>
</html>
```

In the example above, "city" is a **class attribute** and is assigned to other cities. The **id attribute** is only assigned to "myHeader" because we will have one header in this file.

```css
.city {
  background-color: lightblue;
  padding: 20px;
}

#myHeader {
  background-color: black;
  padding: 40px;
}
```

In the example above, the **class selector** (.) comes after the class name to select all elements with the class "city". The **id selector** (#) comes after the id name to target that specific element with the id "myHeader".

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

If you want the content to change on the website based on user interaction you can use **JavaScript** and the **DOM API**. This will allow you to create dynamic behaviors based on user actions, external data, and real-time events, and modify the page content and structure easily. On the other hand, **HTML/CSS** content would be used to create a static page that looks good. The website would still allow the user to interact but, it would be hard to do a site-wide update since the code is hard-coded in the HTML file. You would have to edit each file manually, which isn't practical for large websites.
