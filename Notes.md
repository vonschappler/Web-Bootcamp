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

It's also possible to see those void elements declared as

```html
<hr />
<!-- or -->
<hr />
```

<details>
<summary>Example of use:</summary>

> <p>This is a pargraph, with an <code>hr</code> element below it</p>
> <hr>
> <p>This is a pargraph, with an <code>br</code> element below it</p>
> <br>
> <p>This is a pargraph, placed after the <code>br</code> element.</p>

</details>
<hr>
<br>
