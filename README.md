![alt text](https://github.com/eclipse/editdor/blob/master/logo/1585_ediTDor_logo.png "ediTDor logo")

A tool for simply designing W3C Thing Descriptions and Thing Models

Find the ediTDor here to try it out: 

https://eclipse.github.io/editdor/

## Building the App
There are two ways this app can be built. One way would be for using it as a standalone application, the 
other one for using it embedded into a production environment.
The available environment variables are:
``` bash
REACT_APP_IS_STANDALONE={flag} # true or false
REACT_APP_HOST={hostname} # default: localhost
REACT_APP_PORT={port} # default: 8080
```

If the REACT_APP_IS_STANDALONE environment variable is set to true, REACT_APP_HOST and REACT_APP_PORT are going to be
used for building the UIs target. Otherwise "/" is used.
The package.json already contains build options for this (build, build-standalone).

## About this project

The goal of this project is the easy creation of W3C Thing Description instances and Thing Models by providing a platform-independent ediTDor tool. The following features are addressed in this project

- Creating a new Thing Description / ThingModel from scratch
- Rendering a Thing Description / Thing Model
- Editing the Thing Description / Thing Model
- Validating the Thing Description / ThingModel
- Exporting the Thing Description / ThingModel from the visual representation into JSON-LD
- Reading/writing/observing exposed properties value exposed by a proxy


## Technologies
- React
- TailwindCSS

## Contribution guide
Any contribution to this project is welcome. If you want to report a bug or have a question, please check the [issue list](https://github.com/eclipse/editdor/issues) or create a new issue. Many thanks. 

## License
* [Eclipse Public License v. 2.0](http://www.eclipse.org/legal/epl-2.0)
  
## Prerequisites
* [NodeJS](https://nodejs.org/), use the LTS release


## Start Locally
`yarn dev` starts a local development server on Port 3000 (http://localhost:3000)

## Build
`yarn install` install all the dependencies listed within package.json

`yarn build` builds the project for deployment

## Implemented Features: 
* JSON Editor with JSON Schema support for TD (Autocompletion, JSON Schema Validation)
* Add Property, Action, Event by wizard
* Render TD to be more human readable
* Validate JSON Syntax and JSON Schema for TD (JSONLD and Additional Validation for nested TM will be implemented in the future)

## Additional implemented Features in the fork of editdor: 

* Read/write the value of your properties using the read/write buttons next to the properties name.
