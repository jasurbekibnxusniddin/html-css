

# What are Tags and Attributes?

Tags and attributes are the basis of HTML.

They work together but perform different functions – it is worth investing 2 minutes in differentiating the two.

## What Are HTML Tags?
Tags are used to mark up the start of an HTML element and they are usually enclosed in angle brackets. An example of a tag is: `<h1>`

Most tags must be opened `<h1>` and closed`</h1>` in order to function.

## What are HTML Attributes?
Attributes contain additional pieces of information. Attributes take the form of an opening tag and additional info is placed inside.

An example of an attribute is:

```html
<img src="mydog.jpg" alt="A photo of my dog.">
```

In this instance, the image source (`src`) and the alt text (`alt`) are attributes of the `<img>` tag.

## Golden Rules To Remember

* The vast majority of tags must be opened (`<tag>`) and closed (`</tag>`) with the element information such as a title or text resting between the tags.
* When using multiple tags, the tags must be closed in the order in which they were opened. For example:

```html
<strong><em>This is really important!</em></strong>
```

# Editors
Now that we’ve gotten the basic theory out of the way. It’s time to learn how to build our first website.

First off, we must ensure that we have the right tools. Most important, we need an HTML editor.

There are many choices on the market. Here are a handful of the most popular:

## Sublime Text 3

However, for this tutorial, we will use the Sublime Text 3 as it is free and also offers cross-platform support for Windows, Mac, and Linux users.

![alt text](images/image.png)
Sublime Text 3 has a mini-preview window on the right.

![alt text](images/image-1.png)

# Creating Your First HTML Webpage
First off, you need to open your HTML editor, where you will find a clean white page on which to write your code.

From there you need to layout your page with the following tags.

# Basic Construction of an HTML Page
These tags should be placed underneath each other at the top of every HTML page that you create.

`<!DOCTYPE html>` — This tag specifies the language you will write on the page. In this case, the language is HTML 5.

`<html>` — This tag signals that from here on we are going to write in HTML code.

`<head>` — This is where all the metadata for the page goes — stuff mostly meant for search engines and other computer programs.

`<body>` — This is where the content of the page goes.

![alt text](images/image-2.png) *This is how your average HTML page is structured visually.*


## Further Tags
Inside the `<head>` tag, there is one tag that is always included: `<title>`, but there are others that are just as important:

**`<title>`**
This is where we insert the page name as it will appear at the top of the browser window or tab.

**`<meta>`** This is where information about the document is stored: character encoding, name (page context), description.

Let’s try out a basic `<head>` section:

```html
<head> 
    <title>My First Webpage</title> 
    <meta charset="UTF-8"> 
    <meta name="description" content="This field contains information about your page. It is usually around two sentences long.">. 
    <meta name="author" content="Conor Sheils"> 
</header>
```

## Adding Content
Next, we will make `<body>` tag.

The HTML `<body>` is where we add the content which is designed for viewing by human eyes.

This includes text, images, tables, forms and everything else that we see on the internet each day.

### How to Add HTML Headings To Your Web Page
In HTML, headings are written in the following elements:


```
<h1>
    <h2>
        <h3>
            <h4>
                <h5>
                    <h6>
```
As you might have guessed `<h1>` and `<h2>` should be used for the most important titles, while the remaining tags should be used for sub-headings and less important text.

Search engine bots use this order when deciphering which information is most important on a page.

**Creating Your Heading**

Let’s try it out. On a new line in the HTML editor, type:
```html
<h1>Welcome to My Page</h1>
```

## How To Add Text In HTML

Adding text to our HTML page is simple using an element opened with the tag `<p>` which creates a new paragraph. We place all of our regular text inside the element `<p>`.

When we write text in HTML, we also have a number of other elements we can use to control the text or make it appear in a certain way.

**Other Key Elements**

*They are as follows:*
| Element   | Meaning             | Purpose                                   |
|-----------|---------------------|-------------------------------------------|
| `<b>`     | Bold                | Highlight important information           |
| `<strong>`| Strong              | Similarly to bold, to highlight key text  |
| `<i>`     | Italic              | To denote text                            |
| `<em>`    | Emphasized Text     | Usually used as image captions            |
| `<mark>`  | Marked Text         | Highlight the background of the text      |
| `<small>` | Small Text          | To shrink the text                        |
| `<strike>`| Striked Out Text    | To place a horizontal line across the text|
| `<u>`     | Underlined Text     | Used for links or text highlights         |
| `<ins>`   | Inserted Text       | Displayed with an underline to show inserted text |
| `<sub>`   | Subscript Text      | Typographical stylistic choice            |
| `<sup>`   | Superscript Text    | Another typographical presentation style  |

These tags must be opened and closed around the text in question.

Let’s try it out. On a new line in the HTML editor, type the following HTML code:

```html
<p> Welcome to <em>my</em> brand new website. This site will be my <strong>new<strong> home on the web. </p>
```

## How To Add Links In HTML
As you may have noticed, the internet is made up of lots of links.

Almost everything you click on while surfing the web is a link takes you to another page within the website you are visiting or to an external site.

Links are included in an attribute opened by the `<a>` tag. This element is the first that we’ve met which uses an attribute and so it looks different to previously mentioned tags.

**The Anchor Tag**

The `<a>` (or anchor) opening tag is written in the format:

```html
<a href="https://blogging.com/how-to-start-a-blog/">Your Link Text Here </a>
```

The first part of the attribute points to the page that will open once the link is clicked.

Meanwhile, the second part of the attribute contains the text which will be displayed to a visitor in order to entice them to click on that link.

If you are building your own website then you will most likely host all of your pages on professional web hosting. In this case, internal links on your website will`<a href=”mylinkedpage.html”>Linktle Here</a>`.

**Let’s Create An Anchor Tag**
Let’s try it out. Make a duplicate of the code from your current index.html page. Copy / paste it into a new window in your HTML editor.

Save this new page as “page2.html” and ensure that it is saved in the same folder as your index.html page.

On page2.html add the following code:

```html
<a href="http://www.google.com">Google</a>
```
This will create a link to Google on page 2. Hit save and return to your index.html page.

On a new line on index.html add the following code:

```html
<a href="*folder(s)*/page2.html">Page2</a>
```

Ensure the folder path to the file (page2.html) is correct. Hit save and preview index.html in your browser.

If everything is correct then you will see a link which will take you to your second page. On the second page, there will be a link that will take you to google.com.

## How To Add Images In HTML To Your Website
In today’s modern digital world, images are everything. The `<img>` tag has everything you need to display images on your site. Much like the `<a>` anchor element, `<img>` also contains an attribute.

The attribute features information for your computer regarding the source, height, width and alt text of the image.

Styling and Formats:
![alt text](images/image-3.png)

*You can check the file type of an image by right-clicking the item and selecting ‘Properties’.*

You can also define borders and other styles around the image using the class attribute. However, we shall cover this in a later tutorial.

The file types generally used for image files online are: .jpg, .png, and (less and less) .gif.

Alt text is important to ensure that your site is ranked correctly on search sites and also for visually impaired visitors to your site.

The `<img>` tag normally is written as follows:

```html
<img src="yourimage.jpg" alt="Describe the image" height="X" width="X">
```
Let’s try it out.

Create Your Own Image With An Alt Text

Save an image (.jpg, .png, .gif format) of your choice in the same folder where you’ve saved index.html and page2.html. Call this image “testpic.jpg.”

On a new line in your HTML editor enter the following code:

```html
<img src="testpic.jpg" alt="This is a test image" height="42" width="42">
```
Hit save and preview the index.html page in your browser.

## How To Make an HTML List
In web design, there are 3 different types of lists which you may wish to add to your site.

### Ordered List
The first is an `<ol>`: This is an ordered list of contents. For example:

1. An item
1. Another item
1. Another goes here.

Inside the `<ol>` tag we list each item on the list inside `<li>` `</li>` tags.

For example:

```html
<ol> 
    <li> n item </li> 
    <li> nother item </li> 
    <li> nother goes here </li> 
</ol>
```

### Unordered List

The second type of list that you may wish to include is an `<ul>` unordered list. This is better known as a bullet point list and contains no numbers.

An example of this is:

```html
<ul>
    <li> This is </li>
    <li> An Unordered </li>
    <li> List </li>
</ul>
```
### Definition List
Finally, you may wish to include a definition list `<dl>` on your page. An example of a `<dl>` list is as follows:

HTML
Hypertext markup language is a programming language used to create web pages and is rendered by a web browser.
The code used for the above is as follows:

```html
<dl>
    <dt>Item</dt>
    <dd>The definition goes here</dd>
</dl>
```
Let’s try it out. Open index.html and on a new line, enter the following HTML:

```html
<p>This website will have the following benefits for my business:</p> 

<ul> 
    <li> Increased traffic </li>  
    <li> Global Reach</li> 
    <li> Promotional Opportunities</li> 
</ul>
```
Now hit save and check out the results in your browser. If everything worked out then it will display a bullet-pointed table displaying the information above.

## How To Add Tables In HTML
![alt text](images/image-4.png)

Tables can be styled in various ways – Codepen.io offers live previews to keep track of changes.
Another way to keep your website looking neat and orderly is through the use of a table.

### What Does a Table Consist Of?
When drawing a table we must open an element with the `<table>` opening tag. Inside this tag, we structure the table using the table rows, `<tr>`, and cells, `<td>`.

Read more: https://html.com/#ixzz8uf6A548f
An example of an HTML table is as follows:
```html
<table> 
    <tr> 
        <td>Row 1 - Column 1</td> 
        <td>Row 1 - Colunm 2 </td> 
        <td>Row 1 - Column 3 </td> 
    </tr> 
    <tr> 
        <td>Row 2 - Column 1</td> 
        <td>Row 2 - Column 2</td> 
        <td>Row 2 - Column 3</td> 
    </tr> 
</table>
```
This will produce a 2-row table with 3 cells in each row.

Tables can get quite complicated, so be sure to check out our special HTML tables tutorial.

### Table Tags
However, watch out for these tags so that you can recognize them and use them as your skills develop.

Here are the tables tags presented in a table – pun totally intended.
| Table Tag    | Meaning          | Location              |
|--------------|------------------|-----------------------|
| `<thead>`    | Table Head       | Top of the table      |
| `<tbody>`    | Table Body       | Content of the table  |
| `<tfoot>`    | Table Foot       | Bottom of the table   |
| `<colgroup>` | Column Group     | Within the table      |
| `<th>`       | Table Header     | Data cell for the table header |

Let’s Make a Table
Go to a new line on the index.html page within your text editor. Enter the following HTML code:


```html
<table> 
    <tr> 
        <td> Row 1 - Column 1 </td> 
        <td> Row 1 - Column 2 </td> 
    </tr> 
    <tr> 
        <td> Row 2 - Column 1 </td> 
        <td> Row 2 - Column 2 </td> 
    </tr> 
</table>
```
Hit save and preview it in your browser.

Congratulations: You did it!

# How To Close an HTML Document
You’ve reached the end of our absolute beginners HTML tutorial.

The final step we need to complete is to close the <body> and <html> tags at the end of each page using the following HTML code:

```html
</body>
</html>
```

## Troubleshooting
In case things didn’t work out as intended, simply check your HTML code against the examples below.

Index.html troubleshooting code:
```html
<!DOCTYPE html>

<html>
    
    <head>
        <title>My First Webpage</title>
        <meta charset="UTF-8">
        <meta name="description" content="This is my first website. Itincludes lots of information about my life.">
   </head>
    
    <body>
        <h1>Welcome to my webpage</h1>
        
        <p>Welcome to <em>my</em> brand new website.</p>
        <p>This site will be my <strong>new</strong> home on the web.</p>
        
        <a href="/page2.html">Page2</a>
        
        <img src="testpic.jpg" alt="This is a test image" height="42" width="42">
        
        <p>This website will have the following benefits for my business:</p>
        
        <ul>
            <li>Increased traffic </li>
            <li>Global Reach</li>
            <li>Promotional Opportunities</li>
        </ul>
        
        <table>
            <tr>
                <td>Row 1 - Column 1</td>
                <td>Row 1 - Column 2 </td>
            </tr>
            <tr>
                <td>Row 2 - Column 1</td>
                <td>Row 2 - Column 2</td>
            </tr>
        </table>
    </body>

</html>
```

page2.html troubleshooting code:

```html
<!DOCTYPE html> 
<html> 

    <head> 
        <title>My First Webpage</title> 
        <meta charset="UTF-8"> 
        <meta name="description" content="This is my first website. It includes lots of information about my life."> 
    </head> 
    
    <body>  
        <h1>Welcome to my webpage</h1> 
        
        <p>Welcome to <em>my</em> brand new website.</p> 
        <p>This site will be my <strong>new<strong> home on the web.</p> 
        
        <a href="http://www.google.com">Google</a> 
    </body> 

</html>
```