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

Tips/Conventions:

- It's not a good practice to have more than a `h1` tag.
- Avoid skipping levels of headings

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
<!-- or -->
<hr />
<!-- or -->
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

Tips/Conventions:

- Do not break a single paragraph into multiple paragraphs. Make use of `<br />` when it's necessary to make a single paragraph to have multiple lines.
- It's also possible to see those void elements declared as `<hr/>` or `<hr>`, which is perfectly fine, but not recommended.
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
>   <li>Item A</li>
>   <ul>
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

Tips/Conventions:

- The `alt` attribute stands for `alternative text` which displays a text when the image source is not loaded correctly.
- Remember also to always ADD the `alt` for your `img` elements, because it helps imparied vision users to have the best experience when acessing your webite. This would then make the HMTL element to be defined as:

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

