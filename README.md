# Awesome Cloud-Native Buildpacks

This is the repository for a collection of [Cloud-Native Buildpacks](https://buildpacks.io/), all outlined with some quick feature annotations.

## [Heroku](https://devcenter.heroku.com/)

`heroku/buildpacks:18`

### Provides builders for:

- Java (Maven, Gradle, Clojure)
- Ruby
- Python
- Scala
- PHP
- Golang
- NodeJS (npm, yarn)

Provides `Procfile` launcher support.

##  [Paketo](https://paketo.io/docs/)

(Formerly known as **CloudFoundry Buildpacks**)

`gcr.io/paketo-buildpacks/builder:full-cf`
<br>
(provides full support + native extensions)

`gcr.io/paketo-buildpacks/builder:base`
<br>
(Provides support for Java, NodeJS and Golang)

`gcr.io/paketo-buildpacks/builder:tiny`
<br>
(Provides minimal support for Golang)

### `full-cf` provides builders for:

- Golang (mod, dep)
- .NET (core, core ASP)
- NodeJS (npm, yarn)
- Java
  - Tomcat
  - Executable Jar
  - Gradle
  - Spring Boot
  - Maven
  - SBT
  - Bellsoft Liberica
  - JMX
- Scala (SBT)
- PHP

Provides `Procfile` launcher support.
