## HTML

### Zen Coding
Zen coding will increase your HTML writing speed using an abbreviation syntax similar to css selectors.
```html
<!-- div#container>ul>li*3 will output -->
<div id="container">
    <ul>
        <li></li>
        <li></li>
        <li></li>
    </ul>
</div>
````

### Layout Structures
Name your content by HTML structural elements. 
* Never name your content after the visual appearance but after its description. (e.g. prefer "sidebar-container" than "left-container")
* Add suffix “-container” for clarity to the primary parent element.
* ~~Add container name prefix on subcontent (e.g. header-container > header-title)~~ No need to add the container name as prefix because using less, yu can nest you class in the contaner class, which make more sense.

```html
<body>
    <div id="container">
        <div id="header-container">
            <div class="logo">...</div>
            <div>...</div>
        </div>
        <div id="content-container">...</div>
        <div id="sidebar-container">...</div>
    </div>
</body>
```

### HTML Attributes Naming
* Name your id, class after the elements description and not about the visual elements, use `.external-link` instead of `.red-link` => what if you change the color of the link?
* Use hyphen to name your attribute and class.

```html
<div>
    <div id="header-container">
        <div id="header-title" class="title">...</div>
    </div>
</div>
```



## CSS

### Convention
* Never use #id in your css files. Only class selectors are authorized in a css file. 
* To keep your HTML/CSS clean, name your class as your id. `<div class="header-title" id="header-title"></div>`
* Minimize the depth of your css selector `.article-list ul li h1.title` can be replaced by `.article-list .title`
* CSS Lint your css before pushing live

### Less
* Use Less.css to write your css: http://lesscss.org/. This will improve and structure better your stylesheet files.
* Use the lessprefixer file: http://lessprefixer.com/ It will add the vendor prefixer (webkit, firefox, etc...) to increase the compatibility cross-browser.

### Resources
* Read http://smacss.com/book/

***

## Javascript

* Please use Douglas Crockford javascript convention: http://javascript.crockford.com/code.html
* JSLint your javascript. This tool maintained by Douglas Crockford respects its code convention.
* Always put semicolons
* Use DocBlock comment above variable and function declarations, use inline comment inside function to describe algorithm.

```javascript
/**
 * This is the foo function
 */
foo = function() {
    // this is an inline comment
    var baz = 'bar';   
    return baz;
};
```

* If you need to create an alias of `this`: use `self`

```javascript
var foo = {
  baz: 'Hello World',
  bar: function() {
    var self = this;
    var st = setTimeout(function(){
      return self.baz;
    }, 1000);
  }  
};
```

### Jquery
* Please write jquery plugin following the structure shown at http://jqueryboilerplate.com/


