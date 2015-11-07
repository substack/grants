knight prototype fund 2015

# Project Title

peermaps

# Describe what you will make.

Peermaps will host Open Street Map (OSM) tile data over webtorrent to provide
free web-based maps unencumbered by the usage limits and cost of centralized
tile providers.

Recently, web browsers have implemented webrtc support, which allows web pages to
make direct connections to other browsers without going through a centralized
server. Peermaps uses webtorrent, an implementation of the bittorrent protocol
designed to work over webrtc. This means that peermaps can provide maps in an
ordinary web page with decentralized, cooperative infrastructure that can
compete with the ease of use of commercial providers like Google Maps.

This peer hosting technique has some unique advantages that commercial offerings
support poorly or avoid to cement their platform lock-in such as offline support
and full data export.

# What problem are you trying to solve?

Open Street Map data is already published to bittorrent in raw form, but the raw
data cannot be used to build a map without making tiles first. It is possible to
generate tiles from OSM data, but requires technical expertise and a large
amount of computing power and disk space.

Due to this difficulty, the most practical option right now for mapping projects
is to use a commercial provider for map data. Whether this provider uses
proprietary map data or OSM data doesn't remove the inherent costs and platform
dependence that occur with a centralized web service.

Peer to peer networks can flip these economic models around: the more people use
a peer to peer platform, the more aggregate resources are available and the
better the system scales. This means for a modest fixed cost, peermaps can
operate as an internet-scale, non-commercial public service. Even if the service
becomes very popular, the hosting demands are fixed because the users get data
from each other as they use the service instead of from a single source.

# Who do you intend to impact with the project and how do you understand their needs?

Peermaps will provide data journalists, civic activists, scientists, and
computer programmers a cost-free, openly licensed, public resource for
building custom maps on the web.

These users care more about their own projects than about the underlying
architecture of their maps. Right now, the simple and easy thing for these users
is to pick a cheap or free tier of service from a commercial map tile provider.
Peermaps must be as easy to use as these commercial offerings to be successful.

Some other users are not well served by existing map offerings because they
spend much more of their time offline in remote areas. The peermaps data model
works offline by default, so programmers can create new offline mapping tools
which target journalists and field scientists covering natural disasters,
pandemics, the environment, and conflict zones where an internet uplink may be
very slow and unreliable.

# Please list team members and their qualifications.

James Halliday. Open source programmer. https://github.com/substack

I've worked on open source projects for many years and have published hundreds
of open source libraries and tools. I have worked professionally in Geographic
Information Systems and have build web-based peer to peer distributed systems.

# What progress, if any, have you made on this project?

I've built a streaming Open Street Maps protobuf parser, a prototype tile
server processing chain, and torrent feed to publish updates.

Most of the work of this project involves fully automating the tile server
processing chain.
