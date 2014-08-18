
# Installation Process

The installation process assumes that you have already setup nodejs and npm.  Please google for installing nodejs for your platform (mac osx, pc, linux).

Outline:

* Install Yeoman/KeystoneJS Generators
* Run KeystoneJS Generator with HBS Engine Enabled
* Checkout/Clone Uno-KeystoneJS Theme to directory


## Install Yeoman/KeystoneJS Generators

Creating a KeystoneJS project require more than just trying to `npm install keystonejs` which would only install the core cms library and not all the necessary project components such as Models, Routes, and Configurations.  Instead KeystoneJS supports a Yeoman-Generator which enables a methodology for managing scaffolding with an interactive interface.

### Getting Started with the Generators

First install the Yeoman-Generator

```bash

# install yeoman
npm install -g yeoman

# now install the keystonejs specific generator
npm install -g yeoman-generator

```

## Run KeystoneJS Generator with HBS Engine Enabled

Using the KeystoneJS Yeoman Generator is fairly striaght forward, but for those not familiar with how yeoman facilitates interactive scaffolding generation watch the embedded screencast.

*embed screencast*

## Checkout / Clone Uno-Keystone Theme

Once the generator has completed, you will need to update the included `keystone.js` which acts as the manifest/boostrap file for your keystone project.  Within this file are the path configurations for where public-static assets and template files exist.
