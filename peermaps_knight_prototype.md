knight prototype fund 2015

# Project Title

peermaps

# Describe what you will make.

Peermaps is a collection of reusable, modular tools for manipulating and
displaying maps. The peermaps data model is tailored for offline access and peer
to peer distribution.

The first part of the peermaps project is seeding Open Street Maps tile data to
bittorrent and webtorrent, where the users of the system will help to host the
content. The second part is a spatial index (mddf) that overlays the Open Street
Maps data for community mapping projects and custom visualizations.

These two pieces together will provide a visable alternative to Google Maps and
other commerial providers for community mapping projects.

With peer distribution, we can collectively share the costs of running mapping
infrastructure in a cooperative, non-commercial way with fixed costs.

# What problem are you trying to solve?

Open Street Maps is a vast repository of open geographic information, but using
OSM data in an open project can be challenging.

The OSM data is free under an open license and can be downloaded in bulk,
but to make a map requires domain expertise with advanced database tools and
huge amounts of disk and cpu.

Many mapping projects use commercial services that provide tile data derived
from commercial or open street maps data, but these services come with usage
restrictions and added cost. These commercial offerings are not tailored to
offline use because their business models are predicated upon fetching data from
a centralized service.

With peer to peer hosting, we can serve map data without rate limits that works
online and offline for free, where the users of the system help host the
content.

# Who do you intend to impact with the project and how do you understand their needs?

Data scientists and programmers will benefit from the
They can create visualizations and analyses without worrying about signing up
for the right plan from a commercial offering or downloading the entire OSM
dataset and having to do everything themselves.

Journalists and field scientists will benefit from the offline features of the
peermaps data models. In remote areas with poor internet access, the peermap
toolchain will continue to work. Offline features are very important for
coverage of natural disasters, pandemics, the environment, and conflict zones.

Activists and citizen cartographers will have an easy, non-commercial way to
publish datasets that overlay Open Street Maps data without worrying about usage
limits or tile service restrictions.

# Please list team members and their qualifications.

James Halliday. Open source programmer. https://github.com/substack

I've worked on open source projects for many years and have published hundreds
of open source libraries and tools. I have some experience working in Geographic
Information Systems professionally. I have been working with collaborate peer to
peer technologies for the past year.

# What progress, if any, have you made on this project?

The spatial index and peer to peer data model are mostly complete.

These pieces already exist:

* https://github.com/substack/mddf - spatial index tailored for offline use and peer delivery
* https://www.npmjs.com/package/osm-pbf-parser - Open Street Maps protobuf parser
* https://github.com/substack/osm-pbf-to-mddf - Open Street Maps to mddf converter
* https://github.com/Deadarius/mddf-viewer - graphical viewer for mddf files

These pieces remain:

* Tile data generation scripts and hosting
* Data entry and editing interface for the mddf viewer
* Export to geojson
* Data replication using dat (Knight funded, http://dat-data.com/)
* Embedded web map viewer using webtorrent (https://webtorrent.io/)
* Zoom-level geometry simplification
