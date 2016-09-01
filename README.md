Caleydo Vials Server ![Caleydo Web Server Plugin](https://img.shields.io/badge/Caleydo%20Web-Server-10ACDF.svg)
=====================

The vials server reads genomic files and provide data as API. It is recommended to use it in conjunction with [vials](https://github.com/Caleydo/vials).

Installation
------------

[Set up a virtual machine using Vagrant](http://www.caleydo.org/documentation/vagrant/) and run these commands inside the virtual machine:

```bash
./manage.sh clone Caleydo/vials_server
./manage.sh resolve
```

If you want this plugin to be dynamically resolved as part of another application of plugin, you need to add it as a peer dependency to the _package.json_ of the application or plugin it should belong to:

```json
{
  "peerDependencies": {
    "vials_server": "*"
  }
}
```

GenomeDataProvider
--------------

Reading Genomic Files and provide data as API

Run: `python GenomeDataProvider.py`


### Requirements

Manually install matplotlib: `sudo apt-get install python-matplotlib`


***

<a href="https://caleydo.org"><img src="http://caleydo.org/assets/images/logos/caleydo.svg" align="left" width="200px" hspace="10" vspace="6"></a>
This repository is part of **[Caleydo Web](http://caleydo.org/)**, a platform for developing web-based visualization applications. For tutorials, API docs, and more information about the build and deployment process, see the [documentation page](http://caleydo.org/documentation/).

