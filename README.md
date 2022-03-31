# Site-refactor

## Description 

Horiseon's website needed refactoring into a format using semantic html. The website also needed accessibility fixes. This required changed to both the index.html and the style.css.

Html tags that did not have semantic purpose were converted into semantic html tags in order to better define the different sections according to the webpages layout. This included necessary changes in the style.css file to maintain styles on the page. 

The project's accessibility issues included fixes to link functionality, alternate texts in images and including a informative title.

[Horiseon](https://sambalogna.github.io/site-refactor/)
[Horiseon](./assets/images/horiseon.PNG)

## Table of Contents

* [Languages](#Languages)
* [Important Code Snippets](#CodeSnippets)


## Languages
This project utilizes both HTML and CSS. 

## CodeSnippets

**Example Changes** \
The following provide examples of the overall semantic overhaul of the websites html and fixes to accessibility.

Before: No ID class for nav link
```html
<div class="search-engine-optimization">
```
After: lack of ID class causes accessibility issues.
```html
 <div id="search-engine-optimization" class="search-engine-optimization">
```

Before:
```html
<img src="./assets/images/search-engine-optimization.jpg" class="float-left" />
```
After: alternative text added
```html
<img src="./assets/images/search-engine-optimization.jpg" alt="search-engine-optimization" class="float-left" />
```

Before:
```html
<div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
```
After: header and nav used for semantic purpose
```html
<header>
        <h1>Hori<span class="seo">seo</span>n</h1>
        <nav>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </nav>
    </header>
```