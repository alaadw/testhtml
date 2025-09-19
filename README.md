# HTML Learning Commands for Students

This repository contains a comprehensive guide to all essential HTML commands and elements for educational purposes.

## Table of Contents
1. [Basic HTML Structure](#basic-html-structure)
2. [Text Elements](#text-elements)
3. [Heading Elements](#heading-elements)
4. [Links and Navigation](#links-and-navigation)
5. [Images and Media](#images-and-media)
6. [Lists](#lists)
7. [Tables](#tables)
8. [Forms](#forms)
9. [Semantic Elements](#semantic-elements)
10. [Common Attributes](#common-attributes)

## Basic HTML Structure

Every HTML document should have this basic structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
</head>
<body>
    <!-- Your content goes here -->
</body>
</html>
```

### Essential Structure Elements
- `<!DOCTYPE html>` - Declares the document type
- `<html>` - Root element of the page
- `<head>` - Contains metadata about the document
- `<title>` - Sets the page title (shown in browser tab)
- `<meta>` - Provides metadata about the document
- `<body>` - Contains the visible content

## Text Elements

### Basic Text Formatting
```html
<p>This is a paragraph</p>
<br>  <!-- Line break -->
<hr>  <!-- Horizontal rule/line -->

<!-- Text emphasis -->
<strong>Strong/Bold text</strong>
<b>Bold text</b>
<em>Emphasized/Italic text</em>
<i>Italic text</i>
<u>Underlined text</u>
<mark>Highlighted text</mark>
<small>Small text</small>
<del>Deleted text</del>
<ins>Inserted text</ins>
<sub>Subscript</sub>
<sup>Superscript</sup>
```

### Code and Preformatted Text
```html
<code>Inline code</code>
<pre>
Preformatted text
    with preserved spacing
</pre>
<blockquote>This is a quote from another source</blockquote>
```

## Heading Elements

```html
<h1>Main Heading (Largest)</h1>
<h2>Section Heading</h2>
<h3>Subsection Heading</h3>
<h4>Sub-subsection Heading</h4>
<h5>Minor Heading</h5>
<h6>Smallest Heading</h6>
```

## Links and Navigation

```html
<!-- Basic link -->
<a href="https://www.example.com">Link to external site</a>

<!-- Link to another page -->
<a href="page2.html">Link to another page</a>

<!-- Link to section on same page -->
<a href="#section1">Link to section</a>

<!-- Link to email -->
<a href="mailto:someone@example.com">Send Email</a>

<!-- Link to phone -->
<a href="tel:+1234567890">Call us</a>

<!-- Link that opens in new tab -->
<a href="https://www.example.com" target="_blank">Open in new tab</a>
```

## Images and Media

```html
<!-- Basic image -->
<img src="image.jpg" alt="Description of image">

<!-- Image with size -->
<img src="image.jpg" alt="Description" width="300" height="200">

<!-- Figure with caption -->
<figure>
    <img src="image.jpg" alt="Description">
    <figcaption>This is a caption for the image</figcaption>
</figure>

<!-- Audio -->
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support audio.
</audio>

<!-- Video -->
<video controls width="320" height="240">
    <source src="video.mp4" type="video/mp4">
    Your browser does not support video.
</video>
```

## Lists

### Unordered Lists (Bullet Points)
```html
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```

### Ordered Lists (Numbered)
```html
<ol>
    <li>First step</li>
    <li>Second step</li>
    <li>Third step</li>
</ol>
```

### Description Lists
```html
<dl>
    <dt>Term 1</dt>
    <dd>Description of term 1</dd>
    <dt>Term 2</dt>
    <dd>Description of term 2</dd>
</dl>
```

## Tables

```html
<table>
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
            <th>Header 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Row 1, Cell 1</td>
            <td>Row 1, Cell 2</td>
            <td>Row 1, Cell 3</td>
        </tr>
        <tr>
            <td>Row 2, Cell 1</td>
            <td>Row 2, Cell 2</td>
            <td>Row 2, Cell 3</td>
        </tr>
    </tbody>
</table>
```

## Forms

```html
<form action="/submit" method="post">
    <!-- Text input -->
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
    
    <!-- Email input -->
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    
    <!-- Password input -->
    <label for="password">Password:</label>
    <input type="password" id="password" name="password">
    
    <!-- Number input -->
    <label for="age">Age:</label>
    <input type="number" id="age" name="age" min="1" max="120">
    
    <!-- Date input -->
    <label for="birthday">Birthday:</label>
    <input type="date" id="birthday" name="birthday">
    
    <!-- Textarea -->
    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4" cols="50"></textarea>
    
    <!-- Select dropdown -->
    <label for="country">Country:</label>
    <select id="country" name="country">
        <option value="us">United States</option>
        <option value="uk">United Kingdom</option>
        <option value="ca">Canada</option>
    </select>
    
    <!-- Radio buttons -->
    <fieldset>
        <legend>Gender:</legend>
        <input type="radio" id="male" name="gender" value="male">
        <label for="male">Male</label>
        
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label>
    </fieldset>
    
    <!-- Checkboxes -->
    <fieldset>
        <legend>Interests:</legend>
        <input type="checkbox" id="sports" name="interests" value="sports">
        <label for="sports">Sports</label>
        
        <input type="checkbox" id="music" name="interests" value="music">
        <label for="music">Music</label>
    </fieldset>
    
    <!-- Submit button -->
    <button type="submit">Submit</button>
    <button type="reset">Reset</button>
</form>
```

## Semantic Elements

These elements provide meaning to your content:

```html
<header>Page or section header</header>
<nav>Navigation menu</nav>
<main>Main content of the page</main>
<article>Independent piece of content</article>
<section>Section of content</section>
<aside>Side content/sidebar</aside>
<footer>Page or section footer</footer>

<!-- Other semantic elements -->
<time datetime="2023-12-25">December 25, 2023</time>
<address>Contact information</address>
<details>
    <summary>Click to expand</summary>
    <p>Hidden content that can be expanded</p>
</details>
```

## Common Attributes

These attributes can be used with most HTML elements:

### Universal Attributes
- `id="unique-identifier"` - Unique identifier for the element
- `class="class-name"` - CSS class for styling
- `style="color: red;"` - Inline CSS styles
- `title="Tooltip text"` - Tooltip that appears on hover
- `lang="en"` - Language of the element content
- `hidden` - Hides the element

### Data Attributes
```html
<div data-user-id="123" data-role="admin">Custom data</div>
```

### Accessibility Attributes
```html
<img src="image.jpg" alt="Alternative text for screen readers">
<input type="text" aria-label="Search query">
<div role="button" tabindex="0">Custom button</div>
```

## Practice Examples

### Simple Complete Page
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Webpage</title>
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <main>
        <section id="home">
            <h2>Home Section</h2>
            <p>This is the main content of my webpage.</p>
            <img src="welcome.jpg" alt="Welcome image">
        </section>
        
        <section id="about">
            <h2>About Me</h2>
            <p>I am learning HTML!</p>
        </section>
        
        <section id="contact">
            <h2>Contact Form</h2>
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
                
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                
                <button type="submit">Send Message</button>
            </form>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2023 My Website. All rights reserved.</p>
    </footer>
</body>
</html>
```

## Learning Tips

1. **Start with structure**: Always begin with the basic HTML structure
2. **Use semantic elements**: They make your code more meaningful and accessible
3. **Validate your HTML**: Use online validators to check for errors
4. **Practice regularly**: Try building different types of pages
5. **Learn accessibility**: Always include alt text for images and proper labels for forms
6. **Keep it organized**: Use proper indentation and comments

## Next Steps

After mastering these HTML elements, students should learn:
- CSS for styling
- JavaScript for interactivity
- Responsive design principles
- Web accessibility best practices

Happy coding! 🚀
