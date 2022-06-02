# OpenTDF

## Protect Your Data. Control Your Keys. Build Your Future.

The OpenTDF project is
an open set of standards, libraries, and services
that allow you to enable zero-trust protection
across your ecosystem
to ensure complete data protection
and access control.

## Getting started

To quickly set up your own local OpenTDF cluster, refer to
[our quickstart guide](https://github.com/opentdf/opentdf/tree/main/quickstart).


## Repositories of Note

* Guides and Samples
  * [opentdf](https://github.com/opentdf/opentdf): Introduction to OpenTDF, our implementation of it, examples, and instructions of how to get going and how these all fit together in your projects

* Specification
  * [spec](https://github.com/opentdf/spec): TDF Schema and Protocol Specification. A high-level view of TDF.  

* Services
  * [backend](https://github.com/opentdf/backend): Microservices to support ABAC for Key Access and data storage.
  * [frontend](https://github.com/opentdf/frontend): A Web front end for ABAC

* Client Libraries and Software
  * [client-cpp](https://github.com/opentdf/client-cpp): A native TDF and nanoTDF implementation
  * [client-web](https://github.com/opentdf/client-web): A nanoTDF implementation in JavaScript for web clients and NodeJS.

## Releases

4.15.22 | OpenTDF 0.9.0
* Initial OpenTDF Release
* Quickstart
* Client Libraries: C++, web
* ABAC 

### Services

  * **Attributes**: manages attributes with rules used in ABAC ([container image](https://github.com/opentdf/backend/pkgs/container/attributes), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fattributes))
  * **Claims**: reads the attributes that have been assigned to an entity ([container image](https://github.com/opentdf/backend/pkgs/container/claims), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fclaims))
  * **Entitlements**: manages assignment of attributes to entities ([container image](https://github.com/opentdf/backend/pkgs/container/entitlements), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fentitlements))
  * **Kas**: access control of the key using ABAC ([container image](https://github.com/opentdf/backend/pkgs/container/kas), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fkas))
  * **Storage**: provides temporary credentials to upload a file to a S3 service ([helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fstorage))

### Client Libraries

  * Python [opentdf](https://pypi.org/project/opentdf/)
  * C++ [opentdf-client](https://conan.io/center/opentdf-client)
  * Javascript [@opentdf/client](https://github.com/opentdf/client-web/packages/1152758)
  * Node-based CLI [@opentdf/cli](https://github.com/opentdf/client-web/packages/1158071)

### Extras
  * **Keycloak**: custom build of our preferred identity provider ([container image](https://github.com/opentdf/backend/pkgs/container/keycloak))
  * **Keycloak Multi-arch Base**: we build a custom base image off of the upstream Keycloak image and Keycloak Helm chart - it is identical to the upstream image, just built for both arm64 and amd64 ([container image](https://github.com/opentdf/backend/pkgs/container/keycloak-multiarch-base))
