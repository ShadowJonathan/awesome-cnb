# Awesome Cloud-Native Buildpacks

This is the repository for a collection of [Cloud-Native Buildpacks](https://buildpacks.io/), all outlined with some quick feature annotations.

## [Heroku Buildpacks](https://devcenter.heroku.com/)

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

## [Paketo Buildpacks](https://paketo.io/)

(A **CloudFoundry Project** applying learnings from **CloudFoundry Buildpacks**)

#### Builders:

([source](https://github.com/paketo-buildpacks/builder))

`gcr.io/paketo-buildpacks/builder:full-cf`<br>
(`ubuntu:bionic`-based [paketo stack](https://github.com/paketo-buildpacks/stacks) with common C libraries and utilities.)

`gcr.io/paketo-buildpacks/builder:base`  
(`ubuntu:bionic`-based [paketo stack](https://github.com/paketo-buildpacks/stacks) **without** many C libraries.)  

`gcr.io/paketo-buildpacks/builder:tiny`  
(`ubuntu:bionic`-based [paketo stack](https://github.com/paketo-buildpacks/stacks). Ideal for most Go apps)

### Provides buildpacks for:

- [Golang](https://github.com/paketo-buildpacks/go)
- [.NET Core](https://github.com/paketo-buildpacks/dotnet-core)
- [NodeJS](https://github.com/paketo-buildpacks/nodejs)
- [Java](https://github.com/paketo-buildpacks/java)
- [Scala (SBT)](https://github.com/paketo-buildpacks/sbt)
- [PHP](https://github.com/paketo-buildpacks/php)
- [NGINX](https://github.com/paketo-buildpacks/nginx)

Provides `Procfile` launcher support with the [Procfile Paketo Buildpack](https://github.com/paketo-buildpacks/procfile)  

## [Google Cloud Buildpacks](https://github.com/GoogleCloudPlatform/buildpacks)

`gcr.io/buildpacks/builder`

### Provides [Generic](https://github.com/GoogleCloudPlatform/buildpacks#generic-builder-and-buildpacks) builders for:

- Golang
- Node
- Python
- Java
- .NET

Also provides support to build [Google Cloud Functions](https://github.com/GoogleCloudPlatform/buildpacks#building-a-function)

