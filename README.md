# Snapslides

Read the README in slide form: https://tmke8.github.io/snapslides/

### Template

```html
<!DOCTYPE html>
<html lang="en">
<meta charset="utf-8">
<title>Your title</title>
<link rel="stylesheet" href="snapslides.css">

<!-- begin syntax highlighting -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/atom-one-light.min.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/highlight.min.js"></script>
<script>hljs.highlightAll();</script>
<!-- end syntax highlighting -->

<style>
  :root {
    --running-title: 'Your running title';
  }
</style>

<!-- uncomment the following to get the "dev" view -->
<!-- <body class="dev"> -->

<article tabindex="1" id="viewport">
  <section class="alt-style">
    <h1>Your title</h1>
    <p>Johnson Smith, January 2000
  </section>

  <section>
    <h3>Slide heading</h3>
    <ul>
      <li>Some content
    </ul>
  </section>
</article>

<script>
  // this is needed for compatibility with Firefox
  document.getElementById("viewport").focus();
  // set the total number of slides
  document.querySelector(':root').style.setProperty(
    "--total-slide-num",
    `'${document.getElementById("viewport").childElementCount.toString()}'`);
</script>
```
