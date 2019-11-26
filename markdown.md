![markdown logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

# Markdown

Markdown is a lightweight markup language. It is much like HTML in some respects but is much simpler than HTML. We all know how difficult HTML is to learn :)

Therefore, due to its simplicity, it makes it an ideal choice to do some quick code documentation

Github has support for markdown and many repositories contain a readme file which is written in markdown

The markdown files end with "md"

There are different kinds of markdown but most popular are the basic markdown and the flavored markdown

## Basic Syntax

The basic syntax is very simple. Follow along and you will know it all in 5-15 minutes

### Characters
The following characters are used in the markup and therefore need to be escape with \\ if need be to represent them:
- \# pound
- \- hyphen
- \` backtick (accent grave)
- \> greater than
- \\ backslash
- \. dot
- \+ plus
- \_ underscore
- \! exclamation mark
- \{\}\[\]\(\) any container characters

### Headers

To make a header, the line of text should start with \# pound

One \# is for biggest header and six \# to get smallest header size

\# h1

\## h2

\### h3

\#### h4

\##### h5

\###### h6

# h1
## h2
### h3
#### h4
##### h5
###### h6

### Emphasis

Bold and italic emphasis can be added to the text

The text must be surrounded by asterix \*

One \* for *italic* 

Two \*\* for **bold**

Three \*\*\* for ***bold and italic***

### Blockquotes

Blockquotes can be expressed using the greater than \> character

\> sometimes i wonder what came first,

\> chicken or the egg

> "sometimes i wonder what came first,
> chicken or the egg"

### Lists

Lists can be ordered or unordered.

For **ordered** list, the line must start with any number and dot :

1\. one

1\. two

4 spaces \- two a

4 spaces \- two b

1\. three

1\. four

1. one
1. two
    1. two a
    1. two b, innerlist are made with indentation
1. three
1. four

For **unordered** list, the line must start with hyphen \- :

\- a

\- b

4 spaces \- b a

4 spaces \- b b

\- c

\- d

- a
- b
    - b a
    - b b
- c
- d

### Image

The image format is :
\!\[alt\]\(url\)
![random picture](https://picsum.photos/200/300)
### Link

The link format is :
\[text\]\(url\)
[random picture](https://picsum.photos/200/300)

## Flavored Syntax

The flavored markdown is just a superset of the basic markdown. Just a few more markup options.


### Tables

Tables are made up of \| and \-

column1\|column2\|column3

\---------\|\---------\|\-----------

a     \| b    \|    c

name      |wins|losses
----------|----|-
gabby jay |0   |999
bald bull |50  |4
mike tyson|9999|0
Lil Mac   |????|????

### Code Blocks

Three backticks \(\`\`\`\) begin and ends a code block

```javascript
function hello(){
    console.log("hello world")
}
```

### Task List
\- \[x\] completed

\- \[ \] incomplete

- [x] completed
- [ ] incomplete

©️ Paul Caron, aka ChillPill
