# Awesome Cloud-Native Buildpacks

This is the repository for a collection of [Cloud-Native Buildpacks](https://buildpacks.io/), all outlined with some quick feature annotations.

## [Heroku](https://devcenter.heroku.com/)

`heroku/buildpacks:18` ([source](https://github.com/heroku/pack-images))

### Provides buildpacks for:

- [Java](https://github.com/heroku/heroku-buildpack-java)
    (Maven,
    [Gradle](https://github.com/heroku/heroku-buildpack-gradle),
    [Clojure](https://github.com/heroku/heroku-buildpack-clojure))

- [Ruby](https://github.com/heroku/heroku-buildpack-ruby)

- [NodeJS](https://github.com/heroku/nodejs-engine-buildpack)
    ([npm](https://github.com/heroku/nodejs-npm-buildpack/),
    [yarn](https://github.com/heroku/nodejs-yarn-buildpack))

- [Python](https://github.com/heroku/heroku-buildpack-python)
    (via [cnb-shim](https://github.com/heroku/cnb-shim))

- [Scala](https://github.com/heroku/heroku-buildpack-scala)

- [PHP](https://github.com/heroku/heroku-buildpack-php/)
    (via [cnb-shim](https://github.com/heroku/cnb-shim))

- [Golang](https://github.com/heroku/heroku-buildpack-go)
    (via [cnb-shim](https://github.com/heroku/cnb-shim))

Provides `Procfile` launcher support with the [Procfile buildpack](https://github.com/heroku/procfile-cnb)

*Existing heroku buildpacks can be implicitly converted to CNBs by applying [heroku's CNB shim](https://github.com/heroku/cnb-shim).*

## [Paketo](https://paketo.io/docs/)

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

## [Google](https://github.com/GoogleCloudPlatform/buildpacks)

`gcr.io/buildpacks/builder`

### Provides [Generic](https://github.com/GoogleCloudPlatform/buildpacks#generic-builder-and-buildpacks) builders for:

- Golang
- Node
- Python
- Java
- .NET

Also provides support to build [Google Cloud Functions](https://github.com/GoogleCloudPlatform/buildpacks#building-a-function)
