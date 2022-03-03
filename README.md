# apigee-on-aws
 Apigee API Registry deployment on AWS

## API registry concepts

> The Registry API allows teams to track and manage machine-readable descriptions of APIs.

The Registry API is a structured approach to organizing information about APIs. Machine-readable API specs are key, but we also want to track APIs that lack specs, and we also want to have a way to store API-related metadata that doesn’t fit well in specs.  

The Registry API (protocol documentation) presents a simple resource hierarchy for API information. All **APIs** are tracked in a container called a **project**. APIs contain **versions**, and versions contain **specs**.  

**Specs** can be of any format, and spec formats are specified with a mime_type field in the spec record.  

**Metadata** can be associated with APIs, versions, and specs using maps of key-value pairs attached to these resources, and larger metadata can be stored in artifacts associated with projects, APIs, versions, and specs. Artifacts are binary blobs with associated mime_type values that can optionally refer to Protocol Buffer message types.  

## About the service

The Registry API is a gRPC service that closely follows the guidelines in the Google API Improvement Proposals. This includes following standards for pagination, reading across collections, filtering for all collections, optional partial responses, resource revisions for specs, and support for generated client libraries and HTTP transcoding.  

## Packages (v0.4.4)

- registry-tools (Published on 30 Nov 2021 by Apigee in registry-tools)
- registry-server (Published on 31 Oct 2021 by Apigee in registry-server)
- registry-envoy (Published on 5 Nov 2021 by Apigee in registry-envoy)
- registry-linter (Published on 30 Nov 2021 by Apigee in registry-linter)

## Releases

- [v0.4.4](https://github.com/apigee/registry/tree/v0.4.4)
  - 03/01:  Revision ordering bug fix Latest

- [v0.4.3](https://github.com/apigee/registry/tree/v0.4.3)
  - 02/09:   Add support for recommended_deployment fields and automatically uncompress gzipped artifacts



References
- https://apigee.github.io/registry/
- https://github.com/apigee/registry
