## Maven Conventions

This document defines some conventions that Maven recommends projects
adopt. This is especially important if you intend to distribute your
project publicly.

## Artifact Naming

This section outlines the naming conventions used in the Maven project
object model (POM). This document is an attempt to try and unify the
many various ways projects name the artifacts that they publish for
general consumption by the Java developer community (regardless of
whether they are using Maven).

The first thing you will do when creating a project is to select a group
ID and an artifact ID. If you are building a project to be part of a
larger product that is already using Maven, you should attempt to follow
any patterns already established by other projects for consistency.

These identifiers should be comprised of *lowercase* letters, digits,
and hyphens only.

In general you should select a group ID that describes the entire
product, and artifact IDs that are the basis of filenames for each item
you distribute. The artifact ID may or may not overlap the group ID.

For example:

    maven : maven-core
    maven : wagon-api

As previously mentioned, the artifact ID should be the basis of the
filename for the project, as by default Maven will use that and the
version to assemble the filename. Having the version as part of the
filename is strongly recommended to ensure that the version can be
determined at a glance without having to check a possibly non-existant
manifest, or compare file sizes with the official releases.

Following these guidelines are particularly encouraged when distributing
via the Maven Repository, to ensure that it can easily fit alongside
other projects and reduce the risk of conflicts and confusion.

## Directory Structure

Maven encourages a common directory structure for a project. For more
information on this please refer to our [Introduction to the standard
directory
structure](./guides/introduction/introduction-to-the-standard-directory-layout.html).

