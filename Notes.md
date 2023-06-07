# Personal notes taken

## Section_01:

### How does the internet work:

The internet is a "giant" wire, which allows computers to connect each other.

There as computers known as Servers and the ones knwon as clients.

Process of communication between client and servers

1.  Client (requests to access google.com, for example) > ISP > DNS (sends the ip address of google servers) > Client
2.  Client (uses the ip) > Server (sends files) > Client

### How website works

Basically a website is composed by 3 different files:

1. **HTML file**: stores the content of the site
2. **CSS file**: stores the appearance of the site
3. **JavaScript file**: stores the functionality of the site

Those 3 files together, is what will make webistes nowadays.

<hr>

## Section_02:

### What is HTML?:

The first websites were made with pure HMTL.

HTML stands for HyperText Markup Language

- HyperText:<br>
  Pieces of text (hyperlinks) which link to other documents on the website
- Markup Language:<br>
  Markings (known as html tags) which creates elements on the HTML file.

HMTL tags are mostly composed of 3 parts:

- Opening tag (for example `<h1>`)
- Content (for example "Hello world!")
- Closing tag (for example `</h1>`)

Those 3 parts compose what is known as an HTML element

<hr>
<br>

### HTML headings:

Below we have the code for all the HTML headings, from the top to the bottom level:

```html
<h1>Hello world from h1</h1>
<h2>Hello world from h2</h2>
<h3>Hello world from h3</h3>
<h4>Hello world from h4</h4>
<h5>Hello world from h5</h5>
<h6>Hello world from h6</h6>
```

<details>
<summary>Example of use:</summary>

> <h1>Hello world from h1</h1>
> <h2>Hello world from h2</h2>
> <h3>Hello world from h3</h3>
> <h4>Hello world from h4</h4>
> <h5>Hello world from h5</h5>
> <h6>Hello world from h6</h6>

</details>

<br>
There is no `h7` and below. The code above would render something like this, to the browser:

> Tips/Conventions:
>
> - It's not a good practice to have more than a `h1` tag.
> - Avoid skipping levels of headings

Not following these tips won't break your site, but will keep it consistent in following international convetions for this tag.

<hr>
<br>

### HTML paragragh:

Below we have the code for HTML paragraphs:

```html
<p>A simple paragraph in line 1</p>
<p>A simple paragraph in line 2</p>
```

<details>
<summary>Example of use:</summary>

> <p>A simple paragraph in line 1</p>
> <p>A simple paragraph in line 2</p>

</details>
<hr>
<br>

### HTML void elements:

A void element is a HTML element which forbids you to add content between the opening and closign tags, because void elements **DO NOT HAVE CLOSING TAGS**.

Below we have the code for two HTML void elements:

```html
<hr />
<!-- and -->
<br />
```

<details>
<summary>Example of use:</summary>

> <p>This is a pargraph, with an <code>hr</code> element below it</p>
> <hr>
> <p>This is a pargraph, with an <code>br</code> element below it</p>
> <br>
> <p>This is a pargraph, placed after the <code>br</code> element.</p>

</details>

> Tips/Conventions:
>
> - Do not break a single paragraph into multiple paragraphs. Make use of `<br />` when it's necessary to make a single paragraph to have multiple lines.
> - It's also possible to see those void elements declared as `<hr/>` or `<hr>`, which is perfectly fine, but not recommended.

<hr>

## Section_03:

### HTML listings:

- Unordered lists (order of the items do not matter):
  Below there is the code for using unordered lists:

```html
<ul>
  <li>Item A</li>
  <li>Item B</li>
  <li>Item C</li>
</ul>
```

- Ordered lists (order of the items do matter):
  Below there is the code for using unordered lists:

```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```

<details>
<summary>Example of use:</summary>

> <p>Unordered list</p>
> <ul>
>  <li>Item A</li>
>  <li>Item B</li>
> <li>Item C</li>
> </ul>
> <hr>
> <p>Ordered list</p>
> <ol>
>  <li>Item 1</li>
> <li>Item 2</li>
> <li>Item 3</li>
> </ol>

</details>
<hr>
<br>

### HTML nesting:

It's possible to nest lists inside other lists.

```html
<ul>
  <li>Item A</li>
  <ul>
    <li>Subitem A-A</li>
    <li>Subitem A-B</li>
  </ul>
  <li>Item B</li>
  <ol>
    <li>Subitem B.1</li>
    <li>Subitem B.2</li>
  </ol>
</ul>
```

<details>
<summary>Example of use:</summary>

> <ul>
> <li>Item A</li>
> <ul>
> <li>Subitem A-A</li>
> <li>Subitem A-B</li>
> </ul>
> <li>Item B</li>
> <ol>
> <li>Subitem B.1</li>
> <li>Subitem B.2</li>
> </ol>
> </ul>

</details>
<hr>
<br>

### HTML element atrributes and anchors:

Elements can contain attributes. The way of specifying attributes in HTML files is displayed below:

```html
<tag attribute1="value1" attribute2="value2">Content</tag>
```

There are some atrributes which are specific to certain elements and global elements which can be used on any elements. For more information about those, check the [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)

Anchor are elements used to create hyperlinks, by making use of the `<a>` opening tag and the `</a>` closing tag, with the special `href` attribute, which specifies where should the hyperlink should redirect the user, as seen below:

```html
<a href="any-site-or-page">Text to be displayed</a>
```

<details>
<summary>Example of use:</summary>

The element <code>`<a href='https://google.com'>Visit google</a>`</code> would display this result in a HMTL file, and it would redirect us to `https://google.com` when clicked on the blue text displayed.

> <a href='https://google.com'>Visit google</a>

</details>
<hr>
<br>

### HTML images:

Image elements are elements used to display images, by making use of the `<img />`, without a closing tag, with the special `src`, which specifies the image to be displayed and , as seen below:

```html
<img src="image-file-or-url" />
```

<details>
<summary>Example of use:</summary>

> <img src='https://picsum.photos/200' />

</details>

> Tips/Conventions:
>
> - The `alt` attribute stands for `alternative text` which displays a text when the image source is not loaded correctly.
> - Remember also to always ADD the `alt` for your `img` elements, because it helps imparied vision users to have the best experience when acessing your webite. This would then make the HMTL element to be defined as:

```html
<img src="image-file-or-url" alt="description-of-the-image" />
```

<hr>
<br>

## Section_04:

### Computer file paths:

File paths are ways of navigating between files and folders on a computer.

File paths can be absolute or relative paths.

- Absolute paths are also known as the complete path to a folder or file

```ps
#Example of a absolute file path
C:/Apps/MyApp/run.exe
```

- Relative paths are more useful for webdevelopers and they are relatively of a file being currently used. Those paths are usually shorter.

```ps
#Example of a relative file path to the folder Apps
./MyApp/run.exe
```

Using `../` means `go up a level in the folder structure` while `./` means `stay on the same folder level`.

<details>
<summary>Example of use:</summary>
To understand better, assume the current folder structure:

```
.
├───User
│   ├───MyImages
└───Apss
    ├───rsc
    │   └───file.rsc
    └───MyApp
        ├───run.exe
        └───public
```

- To access the file `run.exe` inside MyApp, relatively to `MyApp` folder, the path would be:

```ps
./run.exe
```

- To access the file `file.rsc` inside rsc, relatively to `MyApp` folder, the path would be:

```ps
../rsc/file.rsc
```

</details>

<hr>
<br>

### Multi-page webistes:

In order to have multi-page websites, there are two basic pre-requisites which need to be satisfied:

1. The folder structure of the site must contain various `*.html` files, such (as an example), `index.html`, `contact.html` and `about.html`
2. The files should make relationship between each other, using anchor tags, where the `href` attribute links to the relative path from the origin HTML file to the destiny HMTL file.
<hr>
<br>

### HTML boilerplate:

HTML boilerplate is the starting code for any html file. This boilerplate has the following structure:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1>Hello world!</h1>
  </body>
</html>
```

Important concepts about this boilerplate:

- Everything between `<head>` and `</head>` won't be displayed. This section includes important information abou the site, helping it to be rendered correctly.
- `<meta charset="UTF-8">` sets the charset type in which the website was written. This makes it easier for the website to render all special symbols used. If the site was not made using `utf-8`, be sure to specify the correct charset.
- `<meta http-equiv="X-UA-Compatible" content="IE=edge">` adds compatibliity on your website, making it visible on older browsers.
- `<meta name="viewport" content="width=device-width, initial-scale=1.0">` specifies how the site should be rendered relatively as default on various devices.
- `<title>Document</title>` specifies the title of the current html file, usually displayed on the top of the browser window or tab where the site is rendered.
- Everything between `<body>` and `</body>` decribes which elements the website contains.

> Tips/Conventions:
>
> - The `lang` helps screen reader applications to match the correct language of the contents in the website, so make sure to always add it to your files..

<hr>
<br>

## Section_05:

### What is CSS?

CSS stands for Cascade Style Sheets and this name makes reference to how the styles defined are applied - from the most general to the most specific rule. Although it's juse one one among many styling languages for websites, but it's the most common and most used by web developers.

<hr>
<br>

### How to add CSS?

There are 3 ways of adding CSS to an html file:

- Inline - the rule(s) are added as an attribute of the element itself (the global `style` attribute) and those rules are apllied ONLY to the element where the css was added:

```html
<tag style="property_1: value_1; ...; property_n: value_n;"></tag>
```

<details>
<summary>Example of use:</summary>

The code:

```html
<p style="background: white; color: red">
  This is a paragraph with red text in a white background
</p>
```

would display the result below:

<img src='https://media.discordapp.net/attachments/500413717561868288/1111572163259011112/image.png' alt='preview 01'>

</details>

<br>

- Internal - the rule(s) are added as a style html element (using the `<style>` and `</style>` tags) into the page and the rules are applied ONLY into the page this style was added:

```html
<style>
  selector {
    property_1: value_1;
    ...
    property_n: value_n;
  }
</style>
```

This block of code is usually added inside the head element of the html file.

<details>
<summary>Example of use:</summary>

The code:

```html
<style>
  p {
    background: gray;
    color: blue;
  }
</style>
<p>This is a paragraph with blue text in a gray background</p>
```

would display the result below:

<img src='https://media.discordapp.net/attachments/500413717561868288/1111572554386247741/image.png' alt='preview 02'>

</details>

<br>

- External - the rule(s) are added as an external file, which can be re-used in different pages, by using the `<link>` tag, being the most used cases when creating a multi-page website:

```css
/* create a file with the name style.css*/
selector {
  property_1: value_1;
  ...
  property_n: value_n;
}
```

```html
<!-- add this line to head block in the html files where the styles need to be applied-->
<link rel="stylesheet" href="url/to/style.css" />
```

<details>
<summary>Example of use:</summary>
The codes:

```css
/* style.css */
p {
  background: white;
  color: black;
}
```

and

```html
<link rel="stylesheet" href="./style.css" />
<p>This is a paragraph with white text in a black background</p>
```

would display the result below:

<img src='https://media.discordapp.net/attachments/500413717561868288/1111572769679872071/image.png' alt='preview 03'>

</details>

<hr>
<br>

### CSS selectors:

CSS selector is the part of any css rule that points to the element which the rules should be applied.

- Element selector:
  element selectors are the simplest ones and they target all elements which match the selected tag.

```css
element {
  property_1: value_1;
  ...
  property_n: value_n;
}
```

<details>
<summary>Example of use:</summary>
The codes:

```css
h2 {
  color: red;
}
```

and

```html
<h2>Red</h2>
<h2>Green</h2>
<h2>Blue</h2>
```

will return the following result:

<img src='https://media.discordapp.net/attachments/500413717561868288/1111591997271195730/image.png' alt='preview 04'>

</details>
<br>

- Class selector: class selectors are the ones which "group" elements which should have the same stile to them. Classes are always defined using the attribute `class` when declaring the html element and called inside the css using a `.` followed by the name of the "group".

On HTML:

```html
<element1 class="group-name">element1 content</element1>
<element2 class="group-name">element2 content</element2>
```

then on CSS:

```css
.group-name: {
  property_1: value_1;
  ...
  property_n: value_n;
}
```

<details>
<summary>Example of use:</summary>
The codes:

```css
h2 {
  color: red;
}

.green-heading {
  color: green;
}
```

and

```html
<h2>Red</h2>
<h2 class="green-heading">Green</h2>
<h2 class="green-heading">Blue</h2>
```

will return the following result:

<img src='https://media.discordapp.net/attachments/500413717561868288/1111702745037152257/image.png' alt='preview 06'>

</details>
<br>

- ID selector: id selectors are the ones which specify a single element with a unique id. Elements ids are defined by using the attribute `id` when declaring the html element and called inside the css using a `#` followed by the name of the "id".

HTML ids have to be unique, because those are the identifiers of elements on the same an id card is used to identify a unique person.

On HTML:

```html
<element1 id="unique_identifier_1"> element1 content </element1>
```

then on CSS:

```css
#unique_identifier_1: {
  property_1: value_1;
  ...
  property_n: value_n;
}
```

<details>
<summary>Example of use:</summary>
The codes:

```css
h2 {
  color: red;
}

.green-heading {
  color: green;
}

#blue-heading {
  color: blue;
}
```

and

```html
<h2>Red</h2>
<h2 class="green-heading">Green</h2>
<h2 id="blue-heading" class="green-heading">Blue</h2>
```

will return the following result:

<img src='https://media.discordapp.net/attachments/500413717561868288/1111704808190132334/image.png' alt='preview 07'>

</details>
<br>

- Attribute selector: attribute selectors are the ones which elements based on a specific attribute or the attribute value they have. This is created in the css by using the sintax below:

On HTML:

```html
<element attribute="value"> element content1 </element>
<element attribute="value"> element content2 </element>
```

then on CSS:

```css
element[atrribute="value"]: {
  property_1: value_1;
  ...
  property_n: value_n;
}
```

<details>
<summary>Example of use:</summary>
The codes:

```css
h2 {
  color: red;
}

.green-heading {
  color: green;
}

#blue-heading {
  color: blue;
}

h2[setUnderline='true'] {
  text-decoration: underline;
}
```

and

```html
<h2 setUnderline="true">Red</h2>
<h2 class="green-heading">Green</h2>
<h2 id="blue-heading" class="green-heading" setUnderline="true">Blue</h2>
```

will return the following result:

<img src='https://media.discordapp.net/attachments/500413717561868288/1111713351798628362/image.png' alt='preview 08'>

</details>
<br>

- Universal selector: the universal selector selects everything on the HTML file and apply the rules defined such as below:

```css
* {
  property1: value1;
  ...
  property2: value2;
}
```

<details>
<summary>Example of use:</summary>
The codes:

```css
* {
  background: lightblue;
}

h2 {
  color: red;
}

.green-heading {
  color: green;
}

#blue-heading {
  color: blue;
}

h2[setUnderline='true'] {
  text-decoration: underline;
}
```

and

```html
<h2 setUnderline="true">Red</h2>
<h2 class="green-heading">Green</h2>
<h2 id="blue-heading" class="green-heading" setUnderline="true">Blue</h2>
```

will return the following result:

<img src='https://media.discordapp.net/attachments/500413717561868288/1111717061501132940/image.png' alt='preview 09'>

</details>

<hr>
<br>

## Section_06:

### Color properties:

- Named colors - colors where the name is used to set a color property
- RGB colors - colors where the color is represented in a matrix of 3 values (red, green and blue). Each value stars on 0 and ends on 255, as for example rgb(200, 30, 20)
- Hex colors - colors where the color is represented by a HEX code as for example #FF73AB

<details>
<summary>Example of use:</summary>

```css
/* Named colors */
h1 {
  background-color: blue;
  color: red;
}

/* RGB colors */
h2 {
  background-color: rgb(0, 255, 0);
  color: rgb(255, 0, 0);
}

/* HEX colors  */
h3 {
  background-color: #00ff00;
  color: #ff0000;
}
```

</details>

<hr>
<br>

### Font properties:

- **color** - changes the color of the text
- **font-weight** - changes the boldiness of the text
- **font-size** - changes the size of the text
- **font-family** - changes the typeface of the text

<details>
<summary>Example of use:</summary>

```css
h1 {
  color: blue;
  font-weight: bold;
  font-size: 20px;
  font-family: sans-serif;
  text-align: center;
}
```

</details>

> Tips/Conventions:
>
> - Font size meanings:
> <table>
>  <thead>
>    <th align=center>1px</th>
>    <th align=center>1pt</th>
>    <th align=center>1em</th>
>    <th align=center>1rem</th>
>  </thead>
>  <tbody>
>    <tr>
>      <td colspan=2 align=center>static sizing</td>
>      <td colspan=2 align=center>relative sizing</td>
>     </tr>
>     <tr>
>       <td>1/96 of an inch</td>
>       <td>1/72 of an inch</td>
>       <td>
>         100% of the width of the letter "m"<br>
>         compared relatively to the parent element
>       </td>
>       <td>
>         100% of the width of the letter "m"<br>
>         compared relatively to the html/root element
>       </td>
>     </tr>
>   </tbody>
> </table>
>
> - Whenever defining a font-family, always remember to add a generic typeface that matches the selected fontface, so websites can be rendered normaly in cases where a specific fontface is not found on the user's computer.
> - Fonts which names are formed by multiple words, the name inside quatation marks, such as:
>
> ```css
> h1 {
>   font-family: 'Times New Roman', serif;
> }
> ```

<hr>
<br>

### Box-model:

Each element in HTML exists inside a box. This box is defined basically by 5 properties:

1. **Width**: how "thick" the box is
2. **Height**: how "tall" the box is
3. **Padding**: the internal margin inside of the box
4. **Border**: the contour of the box around the composite sum of measures given by `width + height + padding`
5. **Margin**: the external marding to separate one box from the other

Using CSS, the box model would like something similar to:

```css
h1 {
  width: 200px;
  height: 200px;
  padding: 20px;
  border: 10px solid black;
  margin: 20px;
}
```

The code above, creats a square h1 element, with the total of 300px on each side.

> Tips/Conventions:
>
> - To define a border, it's required 3 arguments: the thickness of the border in pixels, the style of the border and the color of the border
> - It's possible to further customize a border, by adding definitions to each side after the main boder definition. In CSS it would look like to:
>
> ```css
> h1 {
>   border: 10px solid black;
>   border-top: 0;
>   border-right: 10px;
>   border-bottom: 20px;
>   border-left: 30px;
> }
> ```
>
> - The code above can be also written on a different way, as displayed below:
>
> ```css
> h1 {
>   border: 10px solid black;
>   border-width: 0px 10px 20px 30px;
> }
> ```
>
> - It's possible to use border width also in two different ways:
>
> ```css
> h1 {
>   border-width: 10px 20px;
> /*
>   this specifies the value of the top and bottom borders to 10px
>   and left and right to 20px
> */
> }
> h2 {
>   border-width: 10px 20px 40px
> }
> /*
>   this specifies the value of the top to 10px
>   the left and right to 20px
>   and the bottom to 40 px
> */
> ```
>
> - Padding and margin properties also can be set on the same way as done with ``border-width``, when using multple values to define them.

<hr>
<br>

## Section_07:

### CSS Cascade:

A single element can have multiple styles applied to it. When there are conflicting CSS rules, a "cascade" rule is used to define the hierarchy of which will be the final rule to be rendered on screen.

- First hierarchy rule:
  - **Position**: the rules are applied based on their position in the overall CSS definition, being the last one to be read by the browser the rule to be rendered on scree.

- Second hierarchy rule: 
  - **Specificity**: the styles are applied in order of specificty
    1. Elements
    1. Classes
    1. Ids 
  
  This means that rules applied to Ids will get rendred above classes, while classes will be rendered above elements

- Third hierarchy rule:
  - **Type of the CSS rule**: the styles by their definition type
    1. External CSS file
    2. Internal CSS definition
    3. Inline CSS definition
    
  This means that what will be rendered on screen will be the the last rule in the order 