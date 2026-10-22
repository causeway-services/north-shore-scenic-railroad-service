# North Shore Window

<!-- 561-group-standards:badges:start -->
[![Causeway Services](https://img.shields.io/badge/561%20Group-Causeway%20Services-115e69)](https://github.com/causeway-services)
[![License: Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-115e69)](LICENSE)
[![Indigenous data: CARE](https://img.shields.io/badge/Indigenous%20data-CARE-4b6f44)](https://github.com/causeway-services/.github/blob/main/GOVERNANCE.md)
[![Tips welcome](https://img.shields.io/badge/tips-welcome-d4a017)](https://github.com/561-group/.github/blob/main/TIPS.md)
<!-- 561-group-standards:badges:end -->

An independent, unofficial, offline-first moving field guide for North Shore
scenic rail rides from Duluth. It is not affiliated with or endorsed by the
North Shore Scenic Railroad or Lake Superior Railroad Museum and does not offer
operational train status or navigation.

The service contains the two capabilities required for this rail guide:

- TUFTE renders the calm, accessible living-interface shell.
- North Shore route matching turns device GPS into progress and uncertainty on
  this modeled rail corridor.

All route matching, trip traces, bookmarks, and narration preferences remain in
the browser. The core ride requires no account and uploads no location.

```sh
north-shore-window render > index.html
printf '{"latitude":46.81,"longitude":-92.06,"accuracy":20}' |
  north-shore-window project
```

The deployable host is the separate thin [rail-assist.561.group wrapper](../../sites/rail-assist.561.group/README.md).
