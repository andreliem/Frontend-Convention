### Layout Structures
Name your content by HTML structural elements. Add suffix “-container” for clarity. Also name the parent container "container"
```html
<body>
    <div id="container">
        <div id="header-container">...</div>
        <div id="content-container">...</div>
        <div id="sidebar-container">...</div>
    </div>
</body>
```


### HTML/CSS Naming
* Name your id, class after the elements description and not about the visual elements, use `.external-link` instead of `.red-link` => what if you change the color of the link?

* Use hyphen to name your attribute and class.
```html
<div>
    <div id="header-container">...</div>
    <div id="header-title" class="header-title">...</div>
</div>
```


### CSS Coding style
* Never use #id in your css files. Only class otherwise Css Lint won’t like it. To keep it clean, name your class the same as your id, or use smartly parents, children selectors. 



### Javascript Coding style
* variables and function names are written in camelCase. 
