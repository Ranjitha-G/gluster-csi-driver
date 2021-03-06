# Gluster CSI driver Release Process

- [Gluster CSI driver Release Process](#gluster-csi-driver-release-process)
  - [Introduction](#introduction)
  - [Versioning](#versioning)
  - [Tagging repositories](#tagging-repositories)
  - [Release process](#release-process)

## Introduction

This document provides details about Gluster CSI driver releases.

## Versioning

The Gluster CSI driver project uses
[semantic versioning](http://semver.org/)
for all releases.
Semantic versions are comprised of three
fields in the form:

```MAJOR.MINOR.PATCH```

For examples: `1.0.0`, `1.0.0-rc.2`.

Semantic versioning is used since the version
number is able to convey clear information about
how a new version relates to the previous version.
For example, semantic versioning can also provide
assurances to allow users to know when they must
upgrade compared with when they might want to upgrade:

- When `PATCH` increases, the new release contains important **security fixes**,
general bug fixes  and an upgrade is recommended.

 The patch field can contain extra details after the number.
 Dashes denote pre-release versions.`1.0.0-rc.2` in the example
 denotes the second release candidate for release `1.0.0`.

- When `MINOR` increases, the new release adds **new features**
and it must be backward compatible.

- When `MAJOR` increases, the new release adds **new features,
  bug fixes, or both** and which *changes the behavior from
  the previous release* (may be backward incompatible).

## Tagging repositories

The tag name (`$tag` in the previous example) must conform
to the [versioning](#versioning) requirements (e.g. `1.0.0-rc2`).

## Release process

The Release Owner must follow the following process, which is
designed to ensure clarity, quality, stability, and auditability
of each release:

- Raise an issue and assign to themselves.

[new issue in this repository](https://github.com/gluster/gluster-csi-driver/issues/new)

  This issue is used to track the progress of the release with maximum visibility.

- Paste the release checklist into the issue.

  This is useful for tracking so that the stage of the release is visible
  to all interested parties.

- Once all steps are complete, close the issue.
