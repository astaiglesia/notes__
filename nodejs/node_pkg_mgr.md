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