[Previous](Architecture.md) | [Table of contents](README.md) | [Next](Quality.md)
***
# **Interface (Accessibility)**
Interfaces allow diversified resources within and across the organization to seamlessly communicate, discover and exchange data. Interfaces are realized in the form of services and follow standards. Interfaces enable data users to have easy and efficient ways of discovering and accessing data and associated services through the exploitation of standard protocols and the harmonizing of search and data retrieval processes

Question (YC): what is the expected granularity of a recommendation ? Each time a pointer to an existing CEOS document or more fine-grained ?

## Data Discovery

| **ID** | **Recommendations** |
| :---- | :---- |
| **DISC\#1** | Collection and granule discovery interfaces should comply with the [CEOS STAC Collection and Granule Discovery Best Practices](https://github.com/ceos-org/stac-collection-and-granule-discovery-best-practices/tree/v1.0.0) (preferred) or [CEOS OpenSearch Best Practices](https://ceos.org/document_management/Working_Groups/WGISS/Documents/WGISS%20Best%20Practices/CEOS%20OpenSearch%20Best%20Practice.pdf). |
| **DISC\#2** | Service and tool discovery interfaces should comply with [CEOS Service Discovery Best Practice](https://ceos.org/document_management/Working_Groups/WGISS/Documents/WGISS%20Best%20Practices/CEOS-Service-Discovery-Best-Practices_V1.1.pdf). |
| **DISC\#3** | Collection and granule metadata obtained via the discovery interfaces should advertise the existence of the corresponding file-level online data access and subfile or pixel-based access services and endpoints (e.g. OGC WCS, WMTS, WCPS, OGC API Maps, OGC API Tiles, etc.). |
| **DISC\#4** | Collection and granule metadata obtained via the discovery interfaces should advertise the existence of the corresponding authentication endpoint for access to the data (if any). |
| **DISC\#5** | Resource metadata including keywords should link each keyword to its HTTP URI and to the appropriate thesaurus (i.e. controlled vocabularies). |
| **DISC\#6** | Keywords from controlled vocabularies that allow lookup of keyword information via [Linked Data principles](https://en.wikipedia.org/wiki/Linked_data), e.g. HTTP URI dereferencing or SPARQL interfaces are preferred. The use of GCMD controlled keywords is encouraged.|
| **DISC\#7** | Resource metadata shall include the Persistent Identifier (e.g. DOI) of the corresponding resource (if available).   See also [CEOS Persistent Identifier Best Practices](https://ceos.org/document_management/Working_Groups/WGISS/Documents/WGISS%20Best%20Practices/CEOS%20Persistent%20Identifier%20Best%20Practice.pdf).|

## Data Access
| **ID** | **Recommendations** |
| :---- | :---- |
| **DACC\#1** |  Granule data stored in the cloud should be accessible via the S3 (Simple Storage Service) and HTTP(S) protocols. |
| **DACC\#2** |  Data access should support file-level access and subfile or pixel-based access.|
| **DACC\#3** |  Data download interfaces over HTTP should support [`Range Requests`](https://en.wikipedia.org/wiki/Byte_serving) to allow clients to request a portion of a file.  Typical use case: access to a portion of a [Cloud-Optimized GeoTIFF (COG)](https://en.wikipedia.org/wiki/GeoTIFF) file.|
| **DACC\#4** |  |
| **DACC\#5** |  |



***
[Previous](Architecture.md) | [Table of contents](README.md) | [Next](Quality.md)
