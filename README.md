# Repackaged and Patched PicoContainer

This repository contains a build file that creates a repackaged picocontainer version
(the package `org.picocontainer` mapped to `saros.repackaged.picocontainer`) which
also contains a few Saros specific patches (see the `src` dir).

We had to repackage the library because the IntelliJ framework also contains a
picocontainer version and we wanted to avoid the issues that arise from having
both versions in the classpath.

## Build

Calling `./gradlew shadowJar` creates the desired jar file in the directory `build/libs`.
