# hagfish-watcher

The `hagfish-watcher` agent is the Smart Data Center (SDC) service for
recording telemetry about customer workloads for usage monitoring and billing
purposes.  This agent runs on every compute node in an SDC datacenter, writing
usage records that describe customer instances and their disk and network
usage, to disk files once per minute.  Usage data is grouped into hourly files,
named for the time and date of that hour.  These usage files may be archived by
the operator, potentially using the SDC log archival service, [hermes][hermes].

This repository is part of the Joyent SmartDataCenter project (SDC).  For
contribution guidelines, issues, and general documentation, visit the main
[SDC](http://github.com/joyent/sdc) project page.

## License

This Source Code Form is subject to the terms of the Mozilla Public License, v.
2.0.  For the full license text see LICENSE, or http://mozilla.org/MPL/2.0/.

[hermes]: https://github.com/joyent/sdc-hermes.git
