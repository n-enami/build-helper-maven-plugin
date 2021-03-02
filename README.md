# MojoHaus Build Helper Maven Plugin
 
[![The MIT License](https://img.shields.io/github/license/mojohaus/build-helper-maven-plugin.svg?label=License)](https://opensource.org/licenses/MIT)
[![Maven Central](https://img.shields.io/maven-central/v/org.codehaus.mojo/build-helper-maven-plugin.svg?label=Maven%20Central)](http://search.maven.org/#search%7Cga%7C1%7Cbuild-helper-maven-plugin)
[![Main](https://github.com/mojohaus/build-helper-maven-plugin/workflows/Main/badge.svg?branch=master)](https://github.com/mojohaus/build-helper-maven-plugin/actions?query=workflow%3AMain+branch%3Amaster)
[![JDKBuilds](https://github.com/mojohaus/build-helper-maven-plugin/workflows/JDKBuilds/badge.svg?branch=master)](https://github.com/mojohaus/build-helper-maven-plugin/actions?query=workflow%3AJDKBuilds+branch%3Amaster)

This is the [build-helper-maven-plugin](http://www.mojohaus.org/build-helper-maven-plugin/) contains
serveral goals to support you in different kinds of task, like parsing version information,
add supplemental source/test folders to a Maven project or attach supplemental artifacts.

More details can be found on the [goals overview page](http://www.mojohaus.org/build-helper-maven-plugin/).

## Releasing

* Make sure `gpg-agent` is running.
* Execute `mvn -B release:prepare release:perform`

For publishing the site do the following:

```
cd target/checkout
mvn verify site site:stage scm-publish:publish-scm
```
