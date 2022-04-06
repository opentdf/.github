# openTDF

## Protect Your Data. Control Your Keys. Build Your Future.

The openTDF project is
an open set of proposed standards, libraries, and services
that allow you to enable Zero Trust protection
across your ecosystem
to ensure complete data protection
and access control.

## Getting started

To quickly set up your own local openTDF cluster, refer to
[our quickstart guide](https://github.com/opentdf/documentation/tree/main/quickstart).

## Releases
### Services
  * **Attributes**: manages attributes with rules used in ABAC ([container image](https://github.com/opentdf/backend/pkgs/container/attributes), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fattributes))
  * **Claims**: reads the attributes that have been assigned to an entity, provides claims JSON blobs to an identity provider ([container image](https://github.com/opentdf/backend/pkgs/container/claims), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fclaims))
  * **Entitlements**: manages assignment of attributes to entities ([container image](https://github.com/opentdf/backend/pkgs/container/entitlements), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fentitlements))
  * **Kas**: access control of the key using ABAC ([container image](https://github.com/opentdf/backend/pkgs/container/kas), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fkas))
  * **Keycloak**: Keycloak is our Identity Provider (IdP) software ([container image](https://github.com/opentdf/backend/pkgs/container/keycloak)))
    * **Keycloak Multi-arch Base**: we build a custom base image off of the upstream Keycloak image and Keycloak Helm chart - it is identical to the upstream image, just built for both arm64 and amd64 ([container image](https://github.com/opentdf/backend/pkgs/container/keycloak-multiarch-base))
  * **Keycloak Bootstrap**: we use a Python wrapper around Keycloak's REST API to automatically configure Keycloak for Virtru's needs ([container image](https://github.com/opentdf/backend/pkgs/container/keycloak-bootstrap), [helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fkeycloak-bootstrap))
  * **Python Base**: TODO not sure how to describe ([container image](https://github.com/opentdf/backend/pkgs/container/python-base))
  * **Storage**: provides temporary credentials to upload a file to a S3 service ([helm chart](https://github.com/opentdf/backend/pkgs/container/charts%2Fstorage))

### SDKs
  * Python [opentdf](https://pypi.org/project/opentdf/)
  * C++ [opentdf-client](https://conan.io/center/opentdf-client)
  * Javascript [@opentdf/client](https://github.com/opentdf/client-web/packages/1152758)
  * Node-based CLI [@opentdf/cli](https://github.com/opentdf/client-web/packages/1158071)


## Repositories of Note

* Services
  * [backend](https://github.com/opentdf/backend): Microservices to support ABAC for Key Access and data storage.
  * [frontend](https://github.com/opentdf/frontend): A Web front end for ABAC
* Guides and Samples
  * [documentation](https://github.com/opentdf/documentation): Documentation of how to get going and how these all fit together in your projects
* Client Librareis and Software
  * [client-cpp](https://github.com/opentdf/): A native TDF3 and nanoTDF implementation
  * [client-web](https://github.com/opentdf/): A nanoTDF (TDF3 coming soon) implmentation in JavaScript for web clients and NodeJS.
  * [client-python](https://github.com/opentdf/): Python library (wrapper for `client-cpp`)
