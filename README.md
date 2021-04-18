# gl-icons-assets
[![version](https://img.shields.io/npm/v/gl-icons-assets)](https://www.npmjs.com/package/gl-icons-assets) 
[![downloads](https://img.shields.io/npm/types/gl-icons-assets)](https://www.npmjs.com/package/gl-icons-assets) 
[![downloads](https://img.shields.io/npm/dw/gl-icons-assets)](https://www.npmjs.com/package/gl-icons-assets)

### What is this repository for? ###
This package (**g**laucio**l**eonardo-**assets**-**icons**) is a Common icons to be used on web applications.<br>

## Table of contents ##
0. Dependencies-peer:<br>
   
1. Configurations:<br>
   1.1. [ Configuring assets ](#configuring-assets)<br>
   1.2. [ Configuring external links / urls from anchors ](#external-links-anchors)<br>
   1.3. [ Configuring side menu ](#configuraing-side-menu)<br>

<a name="configuring-assets"></a>
### Configuring assets ###
Inside the `angular.json` you need including the following information:
```
{
    "glob": "**/*",
    "input": "node_modules/gl-icons-assets/assets",
    "output": "/assets"
}
```
The output assets could be another path according to your setup.

Here is how the assets `angular.json` should be:
```
{
  ...
  "projects": {
    "lessons-learned-angular": {
      ...
      "architect": {
        "build": {
          "builder": "@angular-devkit/build-angular:browser",
          "options": {
            ...
            "assets": [
              ...,
              {
                "glob": "**/*",
                "input": "node_modules/gl-icons-assets/assets",
                "output": "/assets"
              },
              ...
            ],
            ...
          },
          ...
        },
        ...
      }
    }},
  ...
}

```
