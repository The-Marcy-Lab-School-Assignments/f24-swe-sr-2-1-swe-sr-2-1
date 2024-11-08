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

Elements can share `class` attributes of the same value, while each `id` is unique to the element it is attributed to. In a zoo, `class` attributes could be used to represent and to group each of the species, as their could be multiple animals of each. Meanwhile, `id` attributes could be used to assign a unique name to each of the animals.

```html
<h2 class="species brown-bear">Brown Bear</h2>
<h3 class="brown-bear" id="Brother">Brother Bear</h3>
<p class="descriptions">Enjoys being active.</p>
<h3 class="brown-bear" id="Sister">Sister Bear</h3>
<p class="descriptions">Prefers outdoor environments.</p>
```

In this example, there are two `<h3>` elements with the attribute `class="brown-bear"`, but they each have different `<id>` attributes. This is because, although they both represent animals that are brown bears, they each have their own name that distinguishes them from all other animals. The other elements such as the `<p>` and `<h2>` also have classes that represent their relation to other elements. The paragraph is a description of each of the animals, while the second-level heading is the name of species. As the second-level heading is also related to brown bears, it has the second class, brown-bear.

```css
h2 {
    color: black;
}

.brown-bear {
    color: brown;
}

h3[class="brown-bear"] {
    color: tan;
}

#brother {
    font: sans-serif;
}

#sister {
    font: serif;
}

p {
    color: purple;
}
```

This CSS file assigns colors to second-level headings and paragraphs, while also assigning different fonts to the third-level headings using ID selectors: by combining hash symbols with the `id` values, the program references the specific elements with each ID. The file uses a class selector to set all elements of the brown-bear class to the brown color, but also uses an attribute selector to reassign all third-level headings, excluding other elements of the same class, of class brown-bear to the tan color.

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

HTML and CSS can be used to set up the basic layout of a website, assigning its default styles and appearance when the website is first loaded. HTML and CSS are used to create and style static content, which does not need to change dynamically after the page loads. JavaScript and the DOM API can be used to alter a website as it is used for dynamic content that can be manipulated. For example, if a user's input causes a change in the appearance or layout of elements on a website or changes the page they are on, JavaScript and the DOM API can be used to program these changes so the user's actions will have the corresponding, intended impact. Using only JavaScript and the DOM API is not the best practice as HTML is more clearly structured and is faster.
