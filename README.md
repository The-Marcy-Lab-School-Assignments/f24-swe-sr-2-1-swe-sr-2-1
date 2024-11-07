# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:
* Examples of semantic and non-semantic tags
* The differences between semantic and non-semantic tags
* The benefits of using semantic tags (when possible)

### Response 1

Semantic elements are elements that clearly describe their meaning. Examples include `article`, `<form>`, and `<table>` which clearly define their contents, Non-semantic tags, such as `<span>` and `<div>`, do not communicate their elements' contents and can be used with different attributes. Semantic tags are beneficial in how they are easier to interpret for developers, making the code more readable, browsers, which helps with Search Engine Optimization, and screen readers, which betters accessibility.

## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

### Response 2

Developers can make their websites more accessible by using `<label>` elements on forms to specify required inputs and by adding alternative text to clarify the contents of images. They can also use the `lang` attribute to specify the primary language of each page and of elements that differ from the primary languages of the pages they are on. Semantic tags can provide structure to pages, clearly labeling the meaning of each part. Developers can also add media tags to adapt navigation, altering display to fit different zoom states and viewport sizes. It is important for developers to create websites that meet accessibility standards so users with disabilities will be able to navigate and interact with the websites without additional difficulties, which would benefit all users in how they'd be able to easily perceive and understand the websites. Accessible websites also tend to have cleaner code, likely making development and maintenance less costly.

## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;" >hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

### Response 3

Inline styles may be useful when testing styles as it could be beneficial to add the styles and see the changes quickly. It is often better to write styles in a separate CSS file because code will be more readable and manageable. Using an external stylesheet allows developers to update multiple elements with a style at the same time, rather than applying updates individually as would happen with inline elements.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

* An explanation of the concept of "classes" and "ids" with an analogy.
* An example of the usage using an HTML code block and a CSS code block.
* An explanation of the syntax using the terms: **attribute**, **selector** 

### Response 4

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

