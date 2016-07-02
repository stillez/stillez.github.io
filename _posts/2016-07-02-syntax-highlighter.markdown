---
layout: post
title:  "Syntax Highlighter"
date:   2016-07-02 01:27:00 +0700
---

comming theme: Peacock contract, juicy

```php
<?php

namespace Illuminate\Container;

use Closure;
use ArrayAccess;

/**
 * Theme: Juicy
 * Juicy.
 *
 * Copyright (c) 2014 Dayle Rees
 */
class Container implements ArrayAccess
{
    /**
     * An array of the types that have been resolved.
     *
     * @var array
     */
    protected $resolved = array();

    /**
     * Determine if a given type is shared.
     *
     * @param  string  $abstract
     * @return bool
     */
    public function isShared($abstract)
    {
        if (isset($this->bindings[$abstract]['shared']))
        {
            $shared = $this->bindings[$abstract]['shared'];
        }
        else
        {
            $shared = false;
        }
        return isset($this->instances[$abstract]) || $shared === true;
    }
}
```

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>StillEz</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="style.css">
    <script src="jsscript.js"></script>
  </head>
  <body>
    <div class="container-fluid">
      <header>
        <h1 class="page-header">It's really a Page Header</h1>
      </header>

      <main>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod <strong>tempor</strong> incididunt ut labore et dolore magna aliqua. Ut <a href="blah.html">enim</a> ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        </p
      </main>

      <footer>
          Copy right of Someone
      </footer>
    </div>
  </body>
</html>
```

```css
.class {
    background-image: url(background.jpg);
    margin: 0;
    padding: 0;
    font-family: 'Open Sans', sans-serif;
}

#id {
    content: 'Awesome!';
}

h1, h2, h3, h4, h5, h6 {
    font-weight: bold;
}

a {
    text-decoration: none;
    color: #fff;
    transition: all .25s ease;
}

a:hover {
    color: rgb(0, 0, 0);
}
```

```javascript
$(document).ready(function() {
  $('.class').on('click', function() {
    $('#id').fadeToggle();
    console.log('StillEz');
  });
});
```