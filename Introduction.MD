<!--To view the preview in Vscode use ctrl + shift + v -->
<!--For headers Use a "#" sign with space for H1 heading.
For H2 use 2 "##" sign with space-->
This is Mardown Overview sheet.
For complete info on Markdwon see,
-  [John Gruber's original spec](http://daringfireball.net/projects/markdown/)
-  [Github-flavored Markdown info page](http://github.github.com/github-flavored-markdown/)
 
# Sections <!-- omit in toc -->
<!-- How to link implicit sections in links -->
- [Headers](#headers)
- [Lists](#lists)
- [Quotes](#quotes)
- [Formatting](#formatting)
- [Block](#block)
- [Links](#links)
- [Images](#images)
- [Tables](#tables)
- [Custom HTML](#custom-html)
- [Custom CSS](#custom-css)

---
<!--"---" / "***"/ "___"used for inserting a horizontal rule--> 

## Headers
```
  # H1 
  ## H2 
  ### H3 
  #### H4 
  ##### H5 
  ###### H6
  Another way to to headers
  H1 
  =

  H2 
  -
```
# H1 <!-- omit in toc -->
## H2 <!-- omit in toc -->
### H3 <!-- omit in toc -->
#### H4 <!-- omit in toc -->
##### H5 <!-- omit in toc -->
###### H6 <!-- omit in toc -->
<!-- " omit in toc " this is to prevent it being included in table of contents -->
Another way is to do Headers is

H1 <!-- omit in toc -->
= 
<!-- "=" below for h1/ "-" for h2 -->
H2 <!-- omit in toc -->
-

--- 

## Lists
```
  - Bullet 1
  * Bullet another type
    * Sub bullet type
  + k

  Ordered lists using a number prefix

  1. item 1
  2. item 2
```
- Bullet 1
* Bullet another type
  * Sub bullet type
+ k

Ordered lists using a number prefix

1. item 1
2. item 2

---
<!--"-"/"*" will create a single bullet point giev space after and write-->
<!-- you have to give an 2 trailing spaces after the line to make them seperate or they'll continue -->
Something
continued

Not continued  
seperated by line

---

## Quotes
<!--Use ">" For making text appear different-->
```
  > This is for highliting or making a note
  > ## You can combine Headers and Quotes
  > #### Another one
```

> This is for highliting or making a note
> ## You can combine Headers and Quotes
> #### Another one

---
## Formatting
<!--"*" for italic-->
<!--"**" for Bold-->
```
  *Italic*

  **Bold**

  **_Combined_**

  ~~Striked~~

  They can be _used_ in a sentence too __like__ this. 
```
*Italic*

**Bold**

**_Combined_**

~~Striked~~


They can be _used_ in a sentence too __like__ this. 
<!-- And "_" can be used in place of "*". -->

---

## Block 
    Two tab spaces
    can create this type of thing
    useful for mentioning something


    Or like this text between back ticks
    
    ```
    Text
    ```
```
Another block
```

**For code snippets:**   
We can also do this type of thing for code blocks. 
<!-- 
  ```language 
  code
  ```
  -->
    Javascript
    ```javascript
    var num = 0;
    var num2 = 0;
    ``` 
    HTML
    ```html 
    <div>
        <p>This is an html example</p>
    </div>
    ```


Javascript

```javascript
var num = 0;
var num2 = 0;
``` 

HTML

```html 
<div>
    <p>This is an html example</p>
</div>
```
---

## Links
You can also link a file within the repo as we did with image.
``` 
  <https://www.google.com>  

  [Google](https://www.google.com "Google Homepage")
  "This defines the titlke so if you hover over link you can see the title"

  [1]:(https://www.google.com)
  [Google][1]
```
<!-- A link -->
<https://www.google.com>  

<!-- A link in a sentence -->
[Google](https://www.google.com "Google Homepage")

<!-- Create reference to use multiple times -->
[1]:(https://www.google.com)
[Google][1]

For Implicit links we can use name of headers as a id since this converted to HTML so names becomes id with all lower-case space replaced by "-"(hyphens).

Ex '# Header' becomes `<h1 id="header">Header</h1>`
<!-- `write between them to highlight also for code` -->

Ex 'Header Info' becomes header-info 

- [Headers](#headers) <!-- omit in toc -->
---

## Images
This is same as links just include ! before "[" .  
Also you have to have your picture in same repo.
```
  ![Panda](/red-panda.jpg)
```
![Panda](/red-panda.jpg "Red Panda")

Can also do referencing

```
  [1]:(/red-panda.jpg)
  ![Panda][1]
```
---

##  Tables
```
  | Header 1 | Header 2 | Header 3 |
  | -------- | -------- | -------- |
  |   R1 C1  |   R1 C2  |   R1 C3  | 
```

| Header 1 | Header 2 | Header 3 |
| -------  | -------- | -------- |
|   R1 C1  |   R1 C2  |   R1 C3  | 
|   R2 C1  |   R2 C2  |   R2 C3  | 
|   R3 C1  |   R3 C2  |   R3 C3  | 

For alignment of text in a column use colons " : ". Default **left alignment**.  Colons on each side = **center alignment**.  And a right colon = **right alignment**.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| *zebra stripes* | `are neat`      |    **$1** |

Inline MarkDown can also be used.

---

## Custom HTML

Since MarkDown gets converted to HTML, you can add raw HTML directly to your MarkDown.

```html 
<p>Sample HTML Div</p>
```

<p>Sample HTML Div</p>

---

## Custom CSS

You can also add custom CSS to your MarkDown to add additional styling to your document. You can also include CSS by including a style tag.

```html
<style> 
    body {background-color: #6A68DE;
    color: Black;
    font-size: 1.05rem;}
    a{ color: #FFEC51; }
</style>
```
----