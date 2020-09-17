.. include:: cyverse_rst_defined_substitutions.txt
|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


**WebDAV**
-----------------------------------

WebDAV is an extension to the HTTP protocol that allows users to remotely edit and manage files. CyVerse has added support for WebDAV to the Data Store. This means users can access their home and public folders in the CyVerse Data Store from their local computers using web browsers and other WebDAV enabled applications such as common operating system file managers. With WebDAV, users can copy files between local computer and the Data Store as easily as if they were copying them between two folders on their computer.

----

*Limitations*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
WebDAV works best for small files or small collections of files. There is no hard size limit for files, but it is recommended to not work with files over 1 GiB in size. However, 10 GiB files have been downloaded from the CyVerse WebDAV service using a web browser with decent performance. The iCommands still out perform WebDAV.  For better ways to download large files or large sets of files, please see the pages for `iCommands <./step2.html>`_ or `CyberDuck <./step1.html>`_.

----

*Accessing CyVerse data via WebDAV Services*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

There are two access points to CyVerse WebDAV services: one for anonymous read-only access and one for authenticated access. These services can be accessed directly in a web browser, or with command line tools.

The simiplest way to access WebDAV in a browser is to go to https://data.cyverse.org/dav. This will bring up a menu for the options described below.

WebDAV provides anonymous read-only access through URLs rooted at ``https://data.cyverse.org/dav-anon/``. All data that can be seen by the anonymous user can be accessed anonymously through this service, excluding the immediate contents of ``/iplant/home`` and the immediate contents of ``/iplant/home/<username>``, where <username> is any CyVerse login name. 

The service also provided authenticated access through URLs rooted at ``https://data.cyverse.org/dav/``. Once a user has authenticated with his CyVerse credentials, they can access any file or folder with the permission level they have on the file or folder.

User Data
=========
A user with a CyVerse login of <username> would use the WebDAV link ``https://data.cyverse.org/dav/iplant/home/<username>/`` to access their data. 

Community Released Data/Project Data
=============
To access data from specific projects stored in iRODS at ``/iplant/home/shared/<project>/``, use the link ``https://data.cyverse.org/dav/iplant/projects/<project>/``.

CyVerse Curated Data (Data with a DOI)
=====================
To access the data curated by CyVerse in the Data Commons (that is, datasets with DOIs), use the following link: https://data.cyverse.org/dav-anon/iplant/commons/cyverse_curated/ .


*Common Ways to Access the WebDAV Service*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Web Browser
=====================

Since WebDAV is an extension of HTTP, any web browser can be used to browse and download data through the service, using the links provided above.

File Manager
=====================

Most common operating systems come with a file manager application that can interface with a WebDAV service and can mount a WebDAV folder into the file system being managed. This allows other application running on the same computer as the file manager to access data hosted by a WebDAV service as if it were local.

Accessing through OS X Finder
''''''''''''''''''''''''''''''
Use these instructions to connect to the WebDAV service with OS X Finder.

 1. Open Finder.
 2. From the menu bar, select Go, then Connect to Server (or type command K).
 3. Enter the URL for the folder to access.
 4. Provide your CyVerse username and password if prompted. 

Accessing through Windows File Explorer
''''''''''''''''''''''''''''''
Use these instructions to connect to the WebDAV service with Windows File Explorer.

 1. Open the File Explorer.
 2. Right-click on This PC.
 3. Select Map Network Drive.
 4. Select Choose a custom network location and click next.
 5. Enter the URL for the folder to access.
 6. Provide your CyVerse username and password if prompted. 

Accessing through Gnome Files
''''''''''''''''''''''''''''''
Use these instruction to open the WebDAV service from the Gnome desktop using Files.

 1. Open Files.
 2. Select Other Locations in the Places sidebar.
 3. In the Connect to Server footer, enter the URL for the desired folder to access. Note: Files identifies TLS encrypted WebDAV URLs with the scheme davs. This means the base for the CyVerse URLs is ``davs://data.cyverse.org/`` instead of ``https://data.cyverse.org/``.
 4. Click the neighboring Connect button.
 5. Provide your CyVerse username and password if prompted. 

Accessing through Linux Terminal
''''''''''''''''''''''''''''''
This requires root or at least sudo access. Use these instruction to mount a WebDAV folder into the file system from a Linux terminal. 

 1. Ensure that davfs2 is installed, e.g., for Ubuntu, sudo apt install davfs2.
 2. Create a directory where you to want to mount the data, e.g., mkdir /tmp/data.
 3. Mount the data as root, i.e., sudo mount -o gid=<you>,uid=<you> -t davfs <link> /tmp/data, where <you> is your username on the Linux machine and <link> is the URL to the WebDAV folder you want to mount.
 4. Provide your CyVerse username and password if prompted.


----


*More help and additional information*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

See the `Data Store Manual <https://wiki.cyverse.org/wiki/display/DS/Data+Store+Table+of+Contents>`_ for full details on how to access the Data Store.

..
    Short description and links to any reading materials



----

**Fix or improve this documentation**

- Search for an answer:
  |CyVerse Learning Center|
- Ask us for help:
  click |Intercom| on the lower right-hand side of the page
- Report an issue or submit a change:
  |Github Repo Link|
- Send feedback: `Tutorials@CyVerse.org <Tutorials@CyVerse.org>`_



----

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


.. |CyVerse logo| image:: ./img/cyverse_rgb.png
    :width: 500
    :height: 100
.. _CyVerse logo: http://learning.cyverse.org/
.. |Home_Icon| image:: ./img/homeicon.png
    :width: 25
    :height: 25
.. _Home_Icon: http://learning.cyverse.org/

