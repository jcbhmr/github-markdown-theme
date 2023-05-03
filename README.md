# GitHub Markdown theme

📄 The one-stop shop GitHub-style theme for rendered Markdown documents

<div align="center">

![]()

</div>

## Installation

```sh
npm install @jcbhmr/github-markdown-theme
```

⚠️ This is a _CSS package_. That means there's no JavaScript exported. You are
expected to use this either:

1. With a JavaScript bundler that understands `import "./style.css"` or similar.
2. In your HTML using `<link rel="stylesheet">` with a bundler.
3. Directly on your page using a CDN or your own copy of the `.min.css` file.

If you just want to apply a fancy Markdown style to a page returned by a SSR
function like a PHP script or a Deno deploy response, use code like this:

```html
<link rel="stylesheet" href="https://esm.run/@jcbhmr/github-markdown-theme@1" />
```

## Usage

If you're using a bundler like [Vite], you can use `import` statements in your
JavaScript code to auto-bundle the CSS when you run your build step. Be aware
that this library applies things to the `:root` global scope!

```js
import "@jcbhmr/github-markdown-theme";

document.body.innerHTML = `
  <h1>Hello world!</h1>
  <p>Put your awesome page content here!</p>
`
```

Now you can just use plain HTML elements and they will be styled just like a
regular GitHub `README.md` document would appear on a GitHub repository.
