# Wiki
##No empty href, use # instead

* href was the single required attribute for anchors defining a hypertext source link, but is no longer required in HTML5. Omitting this attribute creates a placeholder link.

* The href attribute indicates the link target, either a URL or a URL fragment. A URL fragment is a name preceded by a hash mark (#), which specifies an internal target location (an ID) within the current document. 

* Putting the "#" symbol as the href for something means that it points not to a different URL, but rather to another id or name tag on the same page. However, if there is no id or name then it goes "no where."

* A hashtag - # within a hyperlink specifies an html element id to which the window should be scrolled.

* href="#some-id" would scroll to an element on the current page such as 
```html 
<div id="some-id"> 
```

* href="//site.com/#some-id" would go to site.com and scroll to the id on that page.

###Scroll to Top:

* href="#" doesn't specify an id name, but does have a corresponding location - the top of the page. Clicking an anchor with href="#" will move the scroll position to the top.
A blank href property is actually a hyperlink to the current page. In other words, it will cause a page refresh.

* Browsers render default styles for elements and will change the default style of an anchor tag that doesn't have the href property. Instead, it will be considered like regular text. It even changes the browsers behavior in regards to the element. The status bar (bottom of the screen) will not be displayed when hovering an anchor without the href property. It is most optimal, then, to use a placeholder href value on an anchor to ensure it is treated as a hyperlink.

###Examples
####Recommended
```html
<a href="#">
  Example link
</a>

<a href="#bottomOfPage">Click to go to the bottom of the page</a>
...
...
...
<a id="bottomOfPage"></a>
```
####Not Recommended
```html
<a href="">
  Example link
</a>
```


###Further Reading

[Don't use href to create empty links.](http://paintincode.blogspot.in/2012/03/dont-use-to-create-empty-links.html)

[What is href and why it is used.](http://stackoverflow.com/questions/4855168/what-is-href-and-why-is-it-used)