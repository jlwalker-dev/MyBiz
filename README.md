# MyBiz
Visual FoxPro 9 Small Business System supporting VFP, SQL Server, MySQL and eventually PostGreSQL
---------------------------------------------
## 2023/01/23
Back in the 1980's, I created a package that I named Simply Retail which was a basic Inventory, Point of Sale, and Reporting system that I gave away to people who bought a computer from my store.  It was written in FoxPro DOS 2.6 and was used by several small businesses.  Eventually, a new job and moving to another state caused me to quit developing it and eventually support, letting it wither away.  However, I always considered that a worthy project that gave me real life experience writing business software.

Around the time FoxPro 2.6 for Windows came out, I started to consider the idea that I should resurrect and rewrite it, but work, family, and life in general kept me from making it a priority.  Now, years after Microsoft dropped VFP as a product (may they rot), I am still gainfully employeed as a VFP developer, but finally found the time to make it a priority to work on ideas that have been in the back of my mind, literally, for decades.

MyBiz is intended to be a powerful small business package that will first be written in VFP with the intent of creating something that can eventually be moved over to a new language.  Perhaps to Alaska Software's VFP successor, or to a language that runs in many operating systems, such as C++, Java, or Kotlin.

The MyBiz system is designed to be very class oriented and understood by anyone with a modicom of VFP experience.  There are several oriented for the project, and a copule that are capable of being used in any VFP project.  Once such example is the SQL class which allows you to write VFP syntax that can be used to access data from SQL Server, MySQL, and eventually PostgreSQL with very little effort.  If you write fairly generic VFP SQL statements, there is virtually no need to worry about translating.  If you do need something language specific or a concept not supported easily by VFP, supporting syntax for one or more SQL engines is a straight forward process.

MyBiz is designed to be easily understood VFP code with no licensing requirements.  It uses some external libraries and utility programs available from GitHub or otherwise freely available on the web.  The idea is to have a system that can be developed and used by anyone with some real-world Visual FoxPro development experience, or as a project to learn VFP development.  There are extensive English language comments in the system and an intent to not use "clever" code.  However, when you create sophisticated classes, some "cleverness" is essential, but every effort is made to make easily read by anyone with junior developer competence.

## Core System
MyBiz has the following features out of the box
* Company, customer, employee, vendor, manufacture support
* Picture support for people and items
* Item catalog, lot tracking, item images, multi building, room, and slot based inventory tracking
* Point of Sale system for different departments or businesses (eg Grocery, Bakery, Deli, Coffee bar, resturant, hardware, etc)
* Full reporting system with graphics, logos, and barcodes printed to paper or PDF
* Support for most printers that use the Windows printing system
* 1D and 2D barcode printing
* TWAIN based camera support
* Basic English, French, German, and Spanish support selected at the user login form
* Portions designed to run on Windows Tablet PCs

## Features included or currently under development
* Multi-user data system
* Dual-monitor support
* A framework that does a lot of the coding work for you
* Builders that help you quickly create standard forms and set up controls
* Expanding the language support for all parts of the system and providing users to support more languages
* GMT based time keeping with local time translation
* Multi-language on-form help, hints, and tool tips.
* Support for more TWAIN devices (cameras and scanners) using external support programs.
* Storing graphics and pictures in the database.  Pictures support versions and multiple angles.
* Supports some of Craig Boyd's [https://www.codemag.com/People/Bio/Craig.Boyd] FLLs, including encryption and compression
* Demonstrates the use of TT barcode fonts for Code39, UPCA, and PDF417, along with using the ZINT project for many more barcode symbologies
* Multi-printer support for reports, receipts, and labels with barcodes, logos, and pictures
* An external report system that moves the work to a separate process on the workstation or another workstation on the network
* Demonstrates a setup and update system
* Demonstrates a near-zero-effort workstation setup concept under Windows 10 and 11
* Asset tracking
* Data auditing

## Notes
* While the system will likely work on versions of some SQL Engines as old as SQL Server 2000, official support starts at SQL Server 2012, MySQL Version 8, VFP 9, and eventually PostGre SQL 14
* There is no expectation to directly support SQL Express or earlier versions of the above listed engines, though many should work without code changes
* As of January 2023, PostGreSQL support is in the planning stages until a new Windows server is provisioned
* Testing of SQL engines is done with separate Windows servers with some MySQL testing on an Ubuntu Linux server
* The system is designed to run on inexpensive workstation hardware.  It has successfully been tested on stick PCs with a Intel® Celeron® Processor J4125 and 8GB RAM, as well several 64 bit Dell PCs built after between 2012 - 2015.  If the PC is able to run Windows 10, has 4 cores, and at least 6GB RAM, is should have very acceptable performance in a production setting.  Debug mode tends to require much faster hardware as a lot of data will end up in the log files, drastically slowing down execution speed.
* Stored procedures, if used, are all language specific and support is currently under development to streamline installing for each SQL engine

## Release
The MyBiz system is slated to be released in the second quarter of 2023, and full source will be available along with current documentation.  It is expected to be open to people to join and commit sometime in late 2023 or early 2024.

## Timeline
Dates subject to life events
# 2023 Q2 Initial Source Release
# 2023 Q3 Wiki setup
# 2023 Q4 Complete the basic system
# 2024 Q1 Open repository up to other developers

Jon Walker
Questions may be directed to jlwalker.dev at gmail.com
