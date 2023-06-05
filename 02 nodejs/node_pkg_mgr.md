# NPM: The Node Package Manager
uses command line interface

module vs package
> module: 
  file that contains some code that is exported

> package: 
  collection of modules packaged together

<br>


## Initialize and populate an NPM Package
`npm init`
`npm i <pkgname>`
`npm i -D <pkgname>`

package.json prop notes
> main: entry point of the node js program

*note that technically... any application utilizing npm and a package.json is an npm package - even if its not publically published on npm*


<br>
<hr>

## `npm ci` __vs__   `npm install`

In short, the main differences between using npm install and npm ci are:

- The project must have an existing package-lock.json or npm-shrinkwrap.json.
- If dependencies in the package lock do not match those in package.json, npm ci will exit with an error, instead of updating the package lock.
- npm ci can only install entire projects at a time: individual dependencies cannot be added with this command.
- If a node_modules is already present, it will be automatically removed before npm ci begins its install.
- It will never write to package.json or any of the package-locks: installs are essentially frozen.

> Essentially, npm install reads package.json to create a list of dependencies and uses package-lock.json to inform which versions of these dependencies to install. If a dependency is not in package-lock.json it will be added by npm install.

### `npm ci => Clean Install`
> **for use in automated environments** — such as test platforms, continuous integration, and deployment — or, any situation where you want to make sure you're doing a clean install of your dependencies.

It installs dependencies directly from package-lock.json and uses package.json only to validate that there are no mismatched versions. If any dependencies are missing or have incompatible versions, it will throw an error.

Use npm install to add new dependencies, and to update dependencies on a project. Usually, you would use it during development after pulling changes that update the list of dependencies but it may be a good idea to use npm ci in this case.

Use npm ci if you need a deterministic, repeatable build. For example during continuous integration, automated jobs, etc. and when installing dependencies for the first time, instead of npm install.

npm install
Installs a package and all its dependencies.
Dependencies are driven by npm-shrinkwrap.json and package-lock.json (in that order).
without arguments: installs dependencies of a local module.
Can install global packages.
Will install any missing dependencies in node_modules.
It may write to package.json or package-lock.json.
When used with an argument (npm i packagename) it may write to package.json to add or update the dependency.
when used without arguments, (npm i) it may write to package-lock.json to lock down the version of some dependencies if they are not already in this file.
npm ci
Requires at least npm v5.7.1.
Requires package-lock.json or npm-shrinkwrap.json to be present.
Throws an error if dependencies from these two files don't match package.json.
Removes node_modules and install all dependencies at once.
It never writes to package.json or package-lock.json.


<br>
<br>
<hr>

## node_modules

**never modify the node modules content**

> the dependency tree

node modules includes the dependencies of our dependencies 

- the bad rep of node_modules was from the early versions of npm when dependency duplicates were needed (e.g. multiple deps have common deps)


<br>
<hr>


## Semantic Versioning
syntax: MAJOR.MINOR.PATCH

MAJOR: incompatible API changes are made (new logic, new deps)
MINOR: adding backwards compatible functionality 
PATCH: for backwards compatible bug fixes

> ^ carat pre-fixed version (e.g. ^0.21.1) : indicates to npm that any version from the same major version may be used (i.e. its NOT a MAJOR UPDATE)

*if the major version <1, then the minor version is treated like a major version*

> ~ tilde pre-fixed versions (e.g. ~4.16.0) : indicates to npm that any patch versions may be used (same major + minor) (i.e. 4.16.xx are all valid)

<br>
<hr>

## package-lock.json and Versioning
- helps us collaborate better amongst a team of devs
- makes sure everyone is working with the same dependency environment
- always include the packaage-lock.json in your commits

> includes:
> - includes exact dep tree versioning used (down to the minor and patch versions)
> - resolution address
> - integrity check
> - more descriptive pkg.json



## vulnerabilities

`npm audit` : npm reviews installed packages and reports issues
**pay attention to noted vulnerabilities - particularly HIGH vulnerabilities**

`npm audit fix` : auto fixes packages

## nodemon : install -D per project


## LinkedIn Endorsements
[endorse pplz!](https://www.linkedin.com/groups/12121940/)