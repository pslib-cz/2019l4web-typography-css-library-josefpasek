# Blog Typography Style Implementation

## Implementation

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">

    <!--Style link-->
    <link rel="stylesheet" type="text/css" href="./style/blog_typography_format.css">

    <!--Font Import-->
    <link href="https://fonts.googleapis.com/css?family=Nunito+Sans:400,600,700,800,900&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Work+Sans&display=swap" rel="stylesheet">
    <title>My Blog</title>
</head>
```

## Usage
CSS file is based on styling HTML tags. However there are few components that are initialized by class.
Entire blog post needs to be wrapped in the **article** tag.
**Article** tag can wrap following components:
* uo/ol
* blockquote
* p, b, i
* h2, h3, h4, h5, h6 (tag **h1** is part of header)

```html 
<article>
    <h2>Heading</h2>
    <p>Paragraph Text</p>
    <p>More Paragraph Text...</p>
    <h2>List</h2>
    <ul>
        <li>List Item 1</li>
        <li>List Item 2</li>
        <li>List Item 3</li>
    </ul>
</article>
```

## Components
### Header

```html
<header>
        <img src="./.../your_header.img" alt="Image Description" />
        <h1>Heading</h1>
        <div class="info">
            <p><b>Author of Post</b><br><span class="date">X. Month XXXX</span><span
                    class="time">How long does it take to read you post</span></p>
        </div>
    </header>
```

### Image in Post

Images that are part of post in the **article** tag are wrapped in **figure** tag.

```html
<article>
<figure><img src="./.../article_img.jpg" alt="Description" />
                <figcaption>
                    Random Photo | by John Decker
                </figcaption>
            </figure>
</article>
```

### Footer
```html
<footer>
        <p>Made by <a href="#">Your Name</a> | XXXX</p>
    </footer>
```