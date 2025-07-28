---
date: 2025-07-28
---

# Recap of the Geo4Lib Community Sprint, Summer 2025

The Geo4Lib community came together on July 21, 2025, for a week-long virtual sprint focused on application development, metadata, documentation, and community governance across multiple open-source projects. We held daily standups and structured the sprint as a choose-your-own-adventure style event, allowing contributors to dive into areas aligned with their interests.

<!-- more -->

## Projects & tasks

### OpenGeoMetadata (OGM) Aardvark Viewer

We began developing a static viewer capable of rendering records from OGM Aardvark JSON. It supports several web service and data formats, including WMS & TMS layers, GeoJSONs, and Cloud-Optimized GeoTIFFs (COGs).

- [Preview the viewer and load sample records](http://opengeometadata.org/ogm-viewer/)
- [GitHub Repository](https://github.com/OpenGeoMetadata/ogm-viewer)

### OGM Aardvark field obligations

We did a thorough review of OGM Aardvark fields to determine:

- Which fields should be mandatory for community standards
- Which are recommended to optimize search and citations
- Which are required in the GeoBlacklight application

This effort produced updated guidance and a new sortable table to clarify field obligations.

[Explore the updated documentation](https://opengeometadata.org/ogm-aardvark/)

### OGM API

A new FastAPI-based metadata endpoint is beginning to take shape. During the sprint, we drafted the technical specifications and held discussions around potential hosting strategies.

If you are interested in contributing or providing feedback, [check out the draft spec in this Google Doc](https://docs.google.com/document/d/12by56JqAJh6Htt3kZNOFX6qtOk3Tp9uGtxEpz2xnSJ8/edit?tab=t.tgbh7bmsp4yh#heading=h.ptdpkd8xdnlz). Comments and questions are encouraged!

### GeoBlacklight v4.5.0 release

We completed the upgrade to support Rails 8 and Blacklight v7.41.0. We also fixed the [CI failures in the GeoBlacklight build by replacing the default IIIF viewer](https://github.com/geoblacklight/geoblacklight/issues/1675).

[View the v4.5.0 release on GitHub](https://github.com/geoblacklight/geoblacklight/releases/tag/v4.5.0)

### OpenIndexMaps version converter

We released a new script that converts GeoJSON files adhering to the OpenIndexMaps specification version 0.0.0 to version 1.0.0.

[Try out the v0-v1-converter](https://github.com/OpenIndexMaps/v0-v1-converter)


### OpenGeoMetadata issue triage

We addressed a few long-standing issues in the OpenGeoMetadata project board.

- [Adding a new IIIF annotation reference URI to OGM documentation](https://github.com/OpenGeoMetadata/metadata-issues/issues/64)
- [Exploring how to display multiple COGs per record](https://github.com/OpenGeoMetadata/metadata-issues/issues/66)
- Fixing broken links and the [broken search function](https://github.com/OpenGeoMetadata/opengeometadata.github.io/issues/118) on the OpenGeoMetadata website


### Geo4Lib website & governance

For the Geo4Lib Commmunity overall, we finalized several governance decisions, launched a new community website, and created an initial list of monthly meeting topics for the upcoming year.

## Reflections

The one-week format proved to be just the right length this time. It was brief enough for participants to get approval or carve out time to attend, yet long enough to make progress.  Having a wide range of tasks to choose from, including both bigger projects and smaller one-off items, gave people the flexibility to contribute in whatever way made sense for them. 

It was also the first sprint to not revolve primarily around the GeoBlacklight software. While we did ship a minor release, much of the focus was on other projects, like OpenGeoMetadata, OpenIndexMaps, and even the creation of a brand-new application: the OGM Viewer.

We plan to host another sprint during the winter season. Until then, join us at upcoming monthly meetings or reach out on Slack!
