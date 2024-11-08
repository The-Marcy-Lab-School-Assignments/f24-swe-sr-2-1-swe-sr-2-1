# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:
* Examples of semantic and non-semantic tags
* The differences between semantic and non-semantic tags
* The benefits of using semantic tags (when possible)

Semantic tags means using HTML elements that describe the content they hold. Opposed to generic tags like <div> or <span> like <header>, <article>, and <footer> explain what the content is for. This makes the page easier to understand making the code easier to read. 

## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

Making websites accessible ensures that all users, regardless of their abilities or disabilities, can navigate and interact with content easily. Adding features such as Add alt text helps those who are vision impaired to be able to navigate your website with screen readers describing the images they are seeing. Enabling keyboard navigation can also help with those who have motor disabilities. 

## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;" >hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

Inline styles are best suited for small projects or one-off styling where you don't anticipate making many changes or need quick adjustments. On the other hand, using a separate CSS file is typically preferred for larger project. This approach allows you to keep your HTML content and CSS separate, making your code more organized and easier to maintain.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

* An explanation of the concept of "classes" and "ids" with an analogy.
* An example of the usage using an HTML code block and a CSS code block.
* An explanation of the syntax using the terms: **attribute**, **selector** 

Imagine you have a wardrobe full of clothes. Inside, you have different types of clothing: shirts, pants, jackets. The "class" would be the type of clothing that you are wearing. For example you can have a bunch of different colored shirts they are all shirts so that would be the class. A class would be a shared, reusable label you can apply to multiple items, in this case like many shirts. Now the "ID" would apply to what type of shirt your referring to. Like if it is a special shirt to you, you can use the id and label it something else, such as "lucky-shirt". An ID is a unique label for a single item, like in this case we are singling out our lucky shirt.
CSS for class would be for my example ".shirts" and it would make any change to everything I have under the class shirts. ID would have a #lucky-shirt so that specific shirt would only get changes.
HTML - CLASS
<div class="shirt">purple Shirt</div>
<div class="shirt">cream Shirt</div>
CSS - CLASS
.shirts {
  color: blue;  --> This will apply to all shirts 
  font-size: 16px;
}
HTML - ID
<div id="lucky-shirt">My Favorite Shirt</div>
CSS- ID 
#favorite-shirt {  
color: gold; --> will only apply to favorite shirts
font-weight: bold; 
}

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

No, suing (DOM) and javascript is not the best practice to build an entire website because relying too much on JavaScript for creating and managing content can lead to code that is not easy to maintain. Since using javascript for this you would have to create complex codes that with time would get hard to manage. Where in HTML you are able to have a neater space to see and fix if there is anything wrong pretty easily. HTML Search engines can easily read and index content that’s directly in the HTML, making it easier for your site to show up in search results. Wheres as with using JavaScript after the page loads, search engines may have trouble reading and indexing it. 

