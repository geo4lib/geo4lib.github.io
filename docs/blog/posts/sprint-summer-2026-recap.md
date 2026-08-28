# Geo4Lib Summer Sprint 2026 Recap

From August 17-21, 2026, the Geo4Lib community held a Summer Community Sprint. Our collaborative work centered on OpenGeoMetadata, including new tools for discovering and viewing OGM records, as well as managing our shared metadata and code repositories.

Beyond those projects, the sprint provided time for participants to make progress on their own work. Daily standups gave us a chance to check in, share ideas, troubleshoot problems, and see what everyone else was working on.

The week included activities across OpenGeoMetadata, GeoBlacklight, georeferencing, metadata cleanup, and data processing. Much of this work addressed a common challenge for geospatial libraries: how to build useful, sustainable services without requiring every institution to solve the same technical problems independently.

## Building Shared OpenGeoMetadata Infrastructure

### OGM API and Discovery

Ownership of the [OGM API](https://github.com/OpenGeoMetadata/ogm-api) and [OGM Discovery](https://github.com/OpenGeoMetadata/ogm-discovery) repositories was formally transferred from Eric Larson's personal GitHub account to the OpenGeoMetadata organization. The API provides access to records from OpenGeoMetadata repositories, while the Discovery app offers a lightweight search interface that can run on GitHub Pages.

We also published a draft proposal for an [OGM API Mirror Network](http://opengeometadata.org/ogm-api-mirror-network/), through which institutions could collaboratively host copies of the API.

Moving these projects into the OpenGeoMetadata organization is part of our effort toward treating them as shared community infrastructure rather than tools maintained by individual developers.

### OGM Viewer

Development also continued on the [OGM Viewer](https://github.com/OpenGeoMetadata/ogm-viewer), a tool for displaying and interacting with OGM metadata and hosted resources. A few of the newer features include:

* tabs for multiple types of views
* a globe-based map view for browsing resources
* user facing error messages for layers that cannot be previewed

### OGM Repository Maintenance

We established a better way to handle records that have been withdrawn from OpenGeoMetadata repositories. Rather than simply deleting metadata when a resource is removed, the new approach is to maintain a `withdrawn.json` file within the repository that lists the identifiers to be retired. This file serves as a record trail and can be used directly to delete or unpublish those items from a search index.

## GeoBlacklight

GeoBlacklight 6 is currently under development and available as an alpha release. Sprint work included:

* integrating the OGM Viewer
* redesigning widgets that show relationships between records
* updating the GeoBlacklight Sidecar Image Plugin to be compatibile with GeoBlacklight versions 4-6

## Local Projects

Participants also used the week as dedicated time for projects at their own institutions.

### Search portal administration

* cleaning up metadata
* planning the addition of scanned maps to a GeoBlacklight site
* testing GeoBlacklight upgrades
* improving geosearch interfaces, including map views based on centroids and bounding box searches

### Georeferencing

* using Allmaps for georeferencing and for adding bounding boxes to map metadata  
* investigating an issue with control points crossing the antimeridian and reporting it to the Allmaps project  
* testing how well AI tools can identify smaller features on scanned maps to serve as control points, such as monuments or public squares

### Cloud Optimized GeoTIFFs (COGS)

* Batch creating COGs
* Testing image bands and transparency with various online viewers
 
---------

Overall, the balance of collaborative and independent work made for a relaxed but productive summer sprint, allowing participants to focus on projects that often get sidelined during the regular work week. We also spent some time looking beyond the sprint and developed a list of discussion topics for Geo4Lib meetings during the coming year.

We plan to host another sprint during the winter season. Until then, join us at upcoming monthly meetings or reach out on Slack.
