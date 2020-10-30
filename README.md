## Paragraphs

This is a paragraph. 

Markdown needs an empty line in between paragraphs in order to show them separately. 

## Text decoration

This text is *italic* and this text is **bold**. 
One set of asterisks (*) or underscores (_) makes the content in-between _italic_, two sets make it __bold__.

This is ~~strikethrough~~.


## Headings

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

Or for h1 and h2:

Heading 1
===

Heading 2
---

## Links
Making sure the link is clickable whatever the parser is: 
<https://lillapulay.dev>

Connecting a link to a certain part of the text:
My [portfolio](https://lillapulay.dev).

Title tag upon mouseover:
[CareerFoundry.com](https://careerfoundry.com "This is where I studied Web Development.")

Creating a reference for links that are used e.g. multiple times in a markdown file:
Check out [FreeCodeCamp][1] for a lot of free resources on [Web Development][something].

[1]: https://freecodecamp.org
[something]: https://en.wikipedia.org/wiki/Web_development "Title tag can still be included."

## Images
```
![alt text](link)
```
Here is a cute baby elephant: ![elephant holding a stick](https://jodilmilnerauthor.files.wordpress.com/2014/05/o-smiling-baby-elephant-facebook.jpg "This can still have a tooltip on mouseover")

Or we can reference it just like we did with links.
Here is a beluga:
![beluga][2]

[2]: https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwallsdesk.com%2Fwp-content%2Fuploads%2F2018%2F02%2FBeluga-Whale-HD-Background.jpg&f=1&nofb=1 "And the tooltip"

Link to a different sized version of an image with "nested markdown":

[![](https://unsplash.it/50/50?image/1000)](https://unsplash.it/500/500?image/1000) 

### Styling/sizing
Or with a pinch of HTML included:

[<img src="https://unsplash.it/50/50?image/1000">](https://unsplash.it/500/500?image/1000)

Width and height:

<img src="https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwallsdesk.com%2Fwp-content%2Fuploads%2F2018%2F02%2FBeluga-Whale-HD-Background.jpg&f=1&nofb=1" width="500" height="300" alt="The beluga again!">

Or with CSS (doesn't work on GH):

<img class="babyelly" src="https://jodilmilnerauthor.files.wordpress.com/2014/05/o-smiling-baby-elephant-facebook.jpg">

<style>
  .babyelly {
    width: 150px;
    height: auto;
  }
</style>

## Lists
### Unordered lists: 
(Using *, + or -)
* milk
* bread
* eggs
* flowers
  * tulips
    * red
    * yellow
  * roses


### Ordered lists:
(Not using incremental numbers - so if changing the list items later, it changes the order accordingly)
1. Get pup
1. Hold pup
   1. Lift pup
   
      Careful though!

      ![pup](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdierenkliniekzeist.nl%2Fwp-content%2Fuploads%2F2013%2F10%2Fpup.jpg&f=1&nofb=1)
    1. Pet pup


## Line Breaks
Line 1. <br>
Line 2.

Line 3.

## Horizontal Rules
Line 1 (Put space between this line and the dashes, otherwise it takes it as an h2!)

---

Line 2 Equation signs - didn't work for me :( 

===

## Block Quotes

>“All that is gold does not glitter,
Not all those who wander are lost;
The old that is strong does not wither,
Deep roots are not reached by the frost.

>From the ashes a fire shall be woken,
A light from the shadows shall spring;
Renewed shall be blade that was broken,
The crownless again shall be king.”

```- J.R.R. Tolkien, The Fellowship of the Ring```

## Code Blocks
With indentation:

    var x = "hello";
    const number = 10;

Or with backticks (adding the language is optional):
```js
console.log('Hello there!);
```

### Inline code:

Just like this: `var x = 10;`.

### Deleting/adding a code snippet - using  'diff':
```diff
const x = 20;
- const y = 10;
+ const y = 30;
```

## Tables
Alignment in a column depends on where the colon is in the 2nd line:
* Left
* Right
* Both ends: centered

| Author | Books                         |
| :----: | :---------------------------- |
| J.R.R. | Tolkien The Lord of the Rings |
|  J.K.  | Rowling Harry Potter          |

## GitHub stuff
Checkboxes

* [x] Finish markdown tutorial
* [ ] Add meta tags
* [ ] Update portfolio
  * [ ] Link colors
  * [ ] Logo
* [ ] Update logos

### Referencing issues/PRs:
```
Check out #3!
```
Upon typing the #, a list of issues and PRs in that repo should pop up. The preview shows how it will be displayed upon posting the comment. 
