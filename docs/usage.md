# How to use `Atom.css`

There are 2 main ways:

## Clone

- Clone:
  ```sh
  git clone https://github.com/NightNovaNN/Atom-CSS.git
  cd Atom-CSS
  ```
- Make File: Make `index.html` or something, if needed include syntax highlights and CSS/JS file:

  - In <head>:

    ```html
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.10.0/styles/github-dark.min.css"
    />
    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.10.0/highlight.min.js"></script>

    <!-- Include CSS -->
    <link rel="stylesheet" href="atom.css" />
    ```

  - In <body>:
    ```html
    <script src="atom.js"></script>
    ```

- Use it!

## Browser

- Make file: `index.html` with:
  - In head:
    ```html
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.10.0/styles/github-dark.min.css"
    />
    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.10.0/highlight.min.js"></script>
    <link
      rel="stylesheet"
      href="https://nightnovann.github.io/Atom-CSS-Host/atom.css"
    />
    <script src="https://nightnovann.github.io/Atom-CSS-Host/atom.js"></script>
    ```
- Use!

---
