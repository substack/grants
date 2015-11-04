knight prototype fund 2015

# Project Title

peermaps

# Describe what you will make.

Peermaps is a collection of reusable, modular tools for manipulating and
displaying maps. The peermaps data model is tailored for offline access and peer
to peer distribution.

# What problem are you trying to solve?

Journalists are often on assignment in remote areas to document natural
disasters, pandemics, the environment, and conflict zones. Internet
communication is unreliable and expensive in these settings, so their data
gathering tools should work offline and make effective use of what connectivity
is available.

Maps can be politically sensitive, particularly for unfolding current events.
Centralized map services are already a conduit for state censorship, but
peer to peer data distribution has built-in redundancy and no single point of
control that can shut off access to map data.

Both of these problems can be solved by a data model that embraces decentralized
data replication.

# Who do you intend to impact with the project and how do you understand their needs?

Journalists and field scientists are often in remote or chaotic areas with poor
internet access. They need tools for collecting geographic data that work
offline and tools for sharing their data sets with the world. Data entry might
come from sensor dumps or manual entry. The maps may change over the course of
study and should save all edits along with the time.

Data visualization professionals and data journalists need to analyze and
extract the raw field data to work with their existing toolchain. They might
also want to build visualizations on top of the peermaps web API.

Programmers can use the underlying peermaps libraries to build more specialized
mapping tools for data entry, analysis, visualization, and peer hosting.

# Please list team members and their qualifications.

James Halliday. Open source programmer. https://github.com/substack

I've worked on open source projects for many years and have published hundreds
of open source libraries and tools. I have some experience working in Geographic
Information Systems professionally.

# What progress, if any, have you made on this project?

The spatial index and peer to peer data model are mostly complete.

These pieces already exist:

* https://github.com/substack/mddf - spatial index tailored for offline use and peer delivery
* https://www.npmjs.com/package/osm-pbf-parser - Open Street Maps protobuf parser
* https://github.com/substack/osm-pbf-to-mddf - Open Street Maps to mddf converter
* https://github.com/Deadarius/mddf-viewer - graphical viewer for mddf files

These pieces remain:

* Data entry and editing interface for the mddf viewer
* Export to geojson
* Data replication using dat (Knight funded, http://dat-data.com/)
* Embedded web map viewer using webtorrent (https://webtorrent.io/)
* Zoom-level geometry simplification
