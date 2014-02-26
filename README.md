# hmtdigital: digital services of the Homer Multitext project

This git repository is for customizations of the generic `citeservlet` to 
provide digital services for the Homer Multitext project.   


## Prerequisites ##

- gradle: <http://www.gradle.org/>
- a SPARQL endpoint serving HMT project data (your own, or a publicly visible one such as <http://beta.hpcc.uh.edu:3030/ds/>)
- a clone of `citeservet`: <https://github.com/cite-architecture/citeservlet>


## Usage ##

In your clone of `citeservlet`, set the value of `customDir` to the `hmt` directory of this repository.   You can then use the generic `gradle war` or `gradle jettyRunWar` tasks within `citeservlet`.

See the documentation in `citeservlet` for more details on how you can configure and customize it.
<<<<<<< HEAD

### `citeservlet` configurations ##

The `confs` dir includes configuration files for running HMT Digital locally, or for installing on HMT project systems.
=======
>>>>>>> 5503c46fa2934038923b599e3d488c9f9b822a01
