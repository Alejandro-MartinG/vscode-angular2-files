# VS Code Angular Files

This extension allows **quickly scaffold angular 2 file templates** in VS Code project.

> Inspired by angular-cli (https://github.com/angular/angular-cli)

![](https://github.com/qwert789/vscode-angular2-files/raw/master/images/add-files.gif)

## Changelog

### 1.3.10
* Fix .angular-cli.json was automatically included in every non cli project
* Fix add module declarations to *.module.ts  instead of *.module.js

### 1.3.9
* Multiple enhancements and performance improvements
* Added support for .angular-cli.json flexible file generation

```json
    "defaults": {
        "styleExt": "css",
        "component": {
            "spec": true,
            "inlineStyle": false,
            "inlineTemplate": false,
            "flat": false,
            "changeDetection": "Default",
            "viewEncapsulation": "Emulated"
        },
        "class": {
            "spec": false
        }, 
        "directive": {
            "flat": true,
            "spec": true
        },
        "guard": {
            "flat": true,
            "spec": true
        },
        "interface": {
            "prefix": ""
        },
        "module": {
            "flat": false,
            "spec": false
        },
        "pipe": {
            "flat": true,
            "spec": true
        },
        "service": {
            "flat": true,
            "spec": true
        }
    }
```

### 1.3.8
* Fixed support for custom app structure

### 1.3.7
* It's just angular
* Module style ext fix - thanks to Sam Lin

### 1.3.6
* Fix incorrect extension in component generation

### 1.3.5
* CPU usage improvements 

### 1.3.4

* Support for non angular-cli file-structure, code should reside in 'app' folder by default 
* Fixed import declarations to incorrect module
* Added route class generat template
 
### 1.3.2

* Angular-Files now supports angular-cli.json and you can use custom prefixes, different style extensions.
* Note: if you not using angular-cli it is possible to add angular-cli.json to customize file generatiion.

### 1.3.1

* Fixed serivces was incorrectly imported to module declarations

### 1.3.0

* Fixed import declarations to closest module

### 1.1.0

* **angular-cli** removed due to slowness
* **app.module** added automatic import of dependencies

### 1.0.0
* Integrated angular-cli for file generation 


## Features

Right click on a file or a folder in your current project. 
You can find multiple options been added to the context menu:

Menu Options  |
---           | 
New Component |
New Directive | 
New Pipe      |
New Service   | 
New Module    |

Menu Options  |
---           | 
New Class     | 
New Interface |
New Enum      | 

** Override default configuration like app prefix and style:
** Create a angular-cli.json (can be used without angular-cli):

```json
{
   "apps":[
      {
         "root":"src",
         "prefix":"app"
      }
   ],
   "defaults":{
      "styleExt":"css"
   }
}
```

**The naming of the files as well as the (boilerplate) snippets are based on the [official Angular Style Guide](https://angular.io/docs/ts/latest/guide/style-guide.html)**

## Installation

1. Install Visual Studio Code 1.5.0 or higher
2. Launch Code
3. From the command palette `Ctrl`-`Shift`-`P` (Windows, Linux) or `Cmd`-`Shift`-`P` (OSX)
4. Select `Install Extension`
5. Type `angular files` and press enter
6. Reload Visual Studio Code

# Disclaimer

**Important:** This extension due to the nature of it's purpose will create
files on your hard drive and if necessary create the respective folder structure.
While it should not override any files during this process, I'm not giving any guarantees
or take any responsibility in case of lost data. 

# License

MIT
