# `hmt-digital`: digital services of the Homer Multitext project

This git repository customizes the generic `cs2` servlet to provide digital services for the Homer Multitext project.



## Versions ##

The master branch always has the most recent published version (currently, version 1.0 series).

The most recent published version is always installed at <http://www.homermultitext.org/hmt-digital>.

The HMT project also runs a current development  branch on
a test server at <http://beta.hpcc.uh.edu/tomcat/hmt-digital>.


### Version numbering ###

The left-most digit identifies a major version, defined as a version that either dramatically changes functionality, or requires a change in configuration. The second digit from the left identifies an upgrade that adds some functionality to the main version, but does not require a change in configuration. The third digit identifies a version with changes that do not alter the underlying functionality but might change appearance or presentation.


## Installation and usage##

`hmt-digital` can be installed on
any machine that can run a servlet container and the gradle build system, and that has access to a SPARQL endpoint with HMT data.



### Prerequisites ###

- gradle: <http://www.gradle.org/>
- a version 1.1 SPARQL endpoint serving HMT project data (your own, or a publicly visible one such as <http://beta.hpcc.uh.edu:3030/>)
- a clone of `cs2`: <https://github.com/cite-architecture/cs2>


### Usage ###

1. In the file `customconf.gradle`, give the absolute path to this directory for the property `overlaySource`, and copy `customconf.gradle` to the `customcts` directory of `cs2`.
2. In `cs2`'s `customcts` directory, run `gradle installSource`

You can now use generic `gretty` tasks in `customcts` (e.g., `gretty appRun` to run the servlet or `gretty war` to build a `.war` file).

See the documentation for `cs2` for more details.
