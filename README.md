# theme-dronecode

Theme for Dronecode Gitbook documentation libraries.

This theme contains adds a horizontal top header/menu bar across the top of a Gitbook (3.x) book. The menu contains links to the main dronecode websites, docs and support pages.


## Install the theme

To install the theme, add the following text to the target book's `book.json`
```json
 "plugins": [
        ...,
        "theme-dronecode@git+https://github.com/dronecode/theme-dronecode.git"
    ],
 ```
 
Optionally, you can also specify a logo that will be displayed on the root index (language-selector) page. For example:
```
    "variables": {
        "logo": "./assets/site/some_logo_full.png"
    },

```