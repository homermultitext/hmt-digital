# hmt-digital 1.1.0: digital services of the Homer Multitext project

This git repository is for customizations of the generic `citeservlet` to 
provide digital services for the Homer Multitext project.   

## Versions ##

The master branch always has the most recent published version (currently, version 1.0 series).  

The most recent published version is always installed at <http://www.homermultitext.org/hmt-digital>.

The HMT project also runs a current development  branch on
a test server at <http://beta.hpcc.uh.edu/tomcat/hmt-digital>.


### Version numbering ###

The left-most digit identifies a major version, defined as a version that either dramatically changes functionality, or requires a change in configuration. The second digit from the left identifies an upgrade that adds some functionality to the main version, but does not require a change in configuration. The third digit identifies a version with changes that do not alter the underlying functionality but might change appearance or presentation.


## Installation and usage##

The HMT project team is beginning development of a virtual machine to run `hmt-digital` (<https://github.com/homermultitext/hmt-digital-vm>).  It is also possible to install the system on
any machine that can run a servlet container, a SPARQL endpoint, and the gradle build system.



### Prerequisites ###

- gradle: <http://www.gradle.org/>
- a SPARQL endpoint serving HMT project data (your own, or a publicly visible one such as <http://beta.hpcc.uh.edu:3030/>)
- a clone of `citeservet`: <https://github.com/cite-architecture/citeservlet>


### Usage ###

In your clone of `citeservlet`, set the value of `customDir` to the `hmt` directory of this repository.   You can then use the generic `gradle war` or `gradle jettyRunWar` tasks within `citeservlet`.

See the documentation in `citeservlet` for more details on how you can configure and customize it.


### `citeservlet` configurations ##

The `confs` dir includes configuration files for running HMT Digital locally, or for installing on HMT project systems.
