# netmeter.club

**netmeter.club** is an experiment tracking the quality and diversity of the Internet by running ping tests to over 700 worldwide destinations. It is backed by [Smokeping](https://oss.oetiker.ch/smokeping/), with monitors in Europe and North America live @ https://netmeter.club.

## Setup

Most of the configuration for my netmeter.club instances live the root of the repo; they are based off the [split configuration](https://salsa.debian.org/debian/smokeping/blob/master/debian/split_config) shipped in the Debian and Ubuntu repos. The most important files are as follows:

- [Database](./Database): Configures the database to store less history in order to save disk space (2+ GB/node down to ~900MB/node)
- [Presentation](./Presentation): Custom display settings, expanding the number of entries under Charts
- [Targets-Shared](./Targets-Shared): The main list of destinations
- [Targets-Shared6](./Targets-Shared6): A (smaller) set of IPv6 destinations

## About the list of targets

The IP list includes data from numerous public sources, including:

- [SpeedtestServer.com](https://www.speedtestserver.com/)
- [LowEndTalk](https://lowendtalk.com), [Affyun](https://affyun.com/) forum posts
- ISP looking glasses, such as [lg.he.net](https://lg.he.net)

## License

[CC BY 4.0](./LICENSE.txt)
