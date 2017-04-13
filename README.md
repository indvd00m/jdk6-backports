# JDK6 backports

Port of some core classes from jdk7+ to jdk6.

Note - this should NOT be permitted to appear in the run-time classpath of 
your library or application, or it may conflict if the annotation is provided
by the virtual machine in which you run it.  Repeat: *do not include in your
application, nor in the transitive dependencies of your application.*

## Using
Add repository to your POM:

```xml
	<repository>
		<id>indvd00m-github-repo</id>
		<url>https://github.com/indvd00m/maven-repo/raw/master/repository</url>
	</repository>
```

Add dependency to your maven project:

```xml
	<dependency>
		<groupId>com.indvd00m</groupId>
		<artifactId>jdk6-backports</artifactId>
		<version>1.0.0-SNAPSHOT</version>
		<scope>provided</scope>
	</dependency>
```

## CI
Maven artifacts are built via Travis: 
[![Build Status](https://travis-ci.org/indvd00m/jdk6-backports.svg?branch=master)](https://travis-ci.org/indvd00m/jdk6-backports)

## Download release

https://github.com/indvd00m/jdk6-backports/releases

## Release notes

### Version 1.0.0
- First release.

## Roadmap

This component is developed as a hobby with no public roadmap or any guarantees of upcoming releases. That said, the following features are planned for upcoming releases:
- ...

## Issue tracking

The issues for this project are tracked on its github.com page. All bug reports and feature requests are appreciated. 

## Building and running tests
```bash
git clone https://github.com/indvd00m/jdk6-backports/
cd jdk6-backports
mvn clean install
```

## Contributions

Contributions are welcome, but there are no guarantees that they are accepted as such. Process for contributing is the following:
- Fork this project
- Create an issue to this project about the contribution (bug or feature) if there is no such issue about it already. Try to keep the scope minimal.
- Develop and test the fix or functionality carefully. Only include minimum amount of code needed to fix the issue.
- Refer to the fixed issue in commit
- Send a pull request for the original project
- Comment on the original issue that you have implemented a fix for it

## License & Author

JDK6 backports is distributed under Apache License 2.0. For license terms, see LICENSE.

JDK6 backports is written by David E. Veliev.
