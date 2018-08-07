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
 
Optionally, you can also specify a number of other features:

1. The logo that will be displayed on the root index (language-selector) page. For example:
   ```
    "variables": {
        "logo": "./assets/site/some_logo_full.png"
    },

   ```
   
1. The logo and url for top left of menu bar. The logo must specify a file location for both large and small versions (though these can be same):
   ```
   "pluginsConfig": { 
    
        
        "theme-dronecode": {

            "logo": {
                "logo_large": "../assets/site/logo_large.png",
                "logo_small": "gitbook-plugin-theme-dronecode/images/dronecode_top_bar_logo_small.png",
                "url": "https://www.dronecode.org/"
            }

        }
    } 
   ```
1. The logo and url for top left of menu bar (defaults to dronecode logo).
   The logo must specify a file location for both large and small versions (though these can be same).
   The images should be transparent.
   ```
   "pluginsConfig": { 
    
        
        "theme-dronecode": {

            "logo": {
                "logo_large": "../assets/site/logo_large.png",
                "logo_small": "../assets/site/logo_small.png",
                "url": "https://www.dronecode.org/"
            }

        }
    } 
   ```
1. The menu items (defaults to dronecode standard links) 
   The menu is an array of items (displayed left-to-right with big text, small text, and URL)
   ```
   "pluginsConfig": { 
    
        
        "theme-dronecode": {

            "menu": [

                  {
                    "url": "http://px4.io/",
                    "text": "PX4 BIG",
                    "text_small" : "PX4"
                  },
                  {
                    "url": "https://www.dronecode.org/documentation/",
                    "text": "Documentation",
                    "text_small" : "Docs"
                  },
                  {
                    "url": "http://discuss.px4.io/",
                    "text": "Support",
                    "text_small" : "Help"
                  }
            ]

        }
    } 
   ```
