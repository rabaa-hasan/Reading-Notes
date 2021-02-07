# Markdown
![Markdown](https://th.bing.com/th/id/OIP.QnlzdbGUlNNNlDRWAwnlsQHaEj?w=279&h=180&c=7&o=5&pid=1.7) ‏

Markdown is a way to style text on the web. You control the display of the document; formatting words, adding images, and creating lists are just a few of the things we can do with Markdown. It is just regular text with a few non-alphabetic characters thrown in, like # or *.
### overview of Markdown syntax that you can use anywhere on GitHub:
#### Headers 
We use # for make headings we have 6 headings. 
# This is an <h1> tag 
###### This is an <h6> tag
#### Emphasis
Making format for the text like make it __bold__, _italic_ or combining them.
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_
#### Lists
__Unordered__
* Item 1
* Item 2
  * Item 2a
  * Item 2b
__Ordered__
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
#### Images
![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)
#### Links
http://github.com - automatic!
[GitHub](http://github.com)
#### Blockquotes
As Kanye West said:

> We're living the future so
> the present is our past.
#### GitHub Flavored Markdown
You can use Markdown most places around GitHub:

. Gists
. Comments in Issues and Pull Requests
. Files with the .md or .markdown extension. 

GitHub.com uses its own version of the Markdown syntax that provides an additional set of useful features, many of which make it easier to work with content on GitHub.com.
Syntax highlighting:
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
#### Task Lists
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
#### Tables
You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe |:

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

#### SHA references
Any reference to a commit’s SHA-1 hash will be automatically converted into a link to that commit on GitHub.

16c999e8c71134401a78d4d46435517b2271d6ac
mojombo@16c999e8c71134401a78d4d46435517b2271d6ac
mojombo/github-flavored-markdown@16c999e8c71134401a78d4d46435517b2271d6ac

#### Issue references within a repository
Any number that refers to an Issue or Pull Request will be automatically converted into a link.

#1
mojombo#1
mojombo/github-flavored-markdown#1

#### Username @mentions
Typing an @ symbol, followed by a username, will notify that person to come and view the comment.

#### Automatic linking for URLs
Any URL (like http://www.github.com/) will be automatically converted into a clickable link.

#### Strikethrough
Any word wrapped with two tildes (like ~~this~~) will appear crossed out.

#### Emoji
GitHub supports emoji!
You can add emoji to your writing by typing :EMOJICODE:.

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

Rendered emoji

#### Paragraphs
You can create a new paragraph by leaving a blank line between lines of text.