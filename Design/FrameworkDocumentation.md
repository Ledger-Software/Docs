#Overview

In this document we will outline our thought process and reasoning behind each of our framework/library choices. These choices are not set in stone, but represent our best estimate of resources that best match project requirements at this time.

##Database

We’ve chosen to use UnQLite as our backend database. It is an embedded NoSQL database engine, with support for both key/value and JSON document storage.

The support for JSON document storage is the primary reason we chose to use UnQLite (as Quicken financial records are stored as JSON objects). UnQLite also provides more than sufficient performance and storage for the needs of this project. It’s driven by a powerful disk storage engine that supports O(1) lookup, and can support terabyte sized databases.

For more information, visit the [official website](https://unqlite.org/) or its [GitHub repository](https://github.com/symisc/unqlite).

##Encryption

We’ve chosen to use the [Java Cryptography Architecture](https://docs.oracle.com/javase/8/docs/technotes/guides/security/crypto/CryptoSpec.html) (JCA) for our cryptography library. JCA is developed by Oracle and has been included with java since version 1.1 of the JDK. JCA exposes APIs to allow programmers to easily access java’s encryption (symmetric/asymmetric block/stream ciphers), key generation and management, and secure random number generation.

##User Interface

[JavaFx](http://docs.oracle.com/javafx/) is our chosen framework for the User Interface. JavaFx includes a [charting library](http://docs.oracle.com/javafx/2/charts/jfxpub-charts.htm) so that we can include metrics and charts regarding the user’s data. 

JavaFx is developed by Oracle therefore has extensive support. Also JavaFx is already included as part of the standard Java JRE so there is nothing to include and has high compatibility will all major operating systems. JavaFx applications can be easily installed on a client’s computer by either embedding into a runnable jar or having it hosted on a website where it will be downloaded then cached on the client’s computer.

On the development side it has good IDE integration allowing for faster development. There is also plenty of documentation and examples. After development it is simple to add custom texture and effects to any component without doing any redesign.
