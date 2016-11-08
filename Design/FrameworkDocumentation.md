#Overview

In this document we will outline our thought process and reasoning behind each of our framework/library choices. These choices are not set in stone, but represent our best estimate of resources that best match project requirements at this time.

##Database

We've chosen to use H2 as our backend database. It is a very popular embedded SQL database engine that supports relational database architectures and file saves.

H2's popularity as a light-weight embedded database is the primary reason we chose it. It has very thorough documentation, and widespread support across various languages. The relational database architecture will also help us organize the user's financial accounts and transactions. H2 also provides more than sufficient performance and storage (maximum database file size of 4 terabytes) for the needs of this project.

For more information, visit the [official website](https://www.h2database.com/).

##Encryption

We’ve chosen to use [H2's built in Encryption](http://www.h2database.com/html/features.html?highlight=encryption&search=Encry#file_encryption). H2 offers encryption using AES and a few other encryption ciphers. We chose AES because it is the most secure of the ciphers that are offered. H2 handles encrypting and decrypting the database when provided a username and password.

##User Interface

[JavaFx](http://docs.oracle.com/javafx/) is our chosen framework for the user interface. JavaFX includes a [charting library](http://docs.oracle.com/javafx/2/charts/jfxpub-charts.htm) so that we can include metrics and charts regarding the user’s data.

JavaFX is developed by Oracle, so it has very extensive documentation and support. Additionally, JavaFX is included as part of the standard Java JRE, so there are no extra external libraries to include. This also means it will be compatible with all major operating systems. JavaFX applications can be easily installed on a client’s computer by either packaging it in a runnable jar or having it hosted on a website where it will be downloaded then cached on the client’s computer.

In regards to development, JavaFX has very good IDE integration and comprehensive online documentation. After designing the user interface layout, it is easy to add custom texture and effects to any graphic component without doing any redesign.
