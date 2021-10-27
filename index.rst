.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_

**Data Store Guide**
====================

|data_store_icon|

Goal
----

The Data Store is more than having a place to save your files. The Data Store
is a way to manage the life cycle of your data. From the moment you create
data, to publication and beyond, there are a number of practices you should
follow to ensure the integrity and value of your data are maintained. This
includes making your data FAIR (Findable, Accessible, Interoperable, and
Reusable). The Data Store helps to achieve this with less effort. This
guide will cover the minimum needed to get you started. Please look through the
|Data Store Manual| for a more comprehensive look at Data Store capabilities.


.. list-table::
    :header-rows: 1

    * - Maintainer
      - Institution
      - Contact
    * - Jason Williams
      - CyVerse / CSHL
      - Williams@cshl.edu

----

.. toctree::
	:maxdepth: 2

	Tutorial home <self>
	Drag-and-drop Data Transfer with Cyberduck <step1.rst>
	Command Line Transfer with iCommands <step2.rst>
	Associate Data with Metadata <step3.rst>
	Data Sharing and Other Features <step4.rst>
	Desktop Access with WebDav <step5.rst>

..
	#### Comment:This tutorial can have multiple pages. The table of contents assumes
	you have an additional page called 'First Step' with content located in 'step1.rst'.
	Copy step1.rst. step2.rst has slightly different formatting to end the document.
	Edit these titles and filenames as needed ####


Prerequisites
-------------


Downloads, access, and services
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*In order to complete this tutorial you will need access to the following services/software*

..
	#### comment: delete any row not needed in this table ####

.. list-table::
    :header-rows: 1

    * - Prerequisite
      - Preparation/Notes
      - Link/Download
    * - CyVerse account (optional)
      - CyVerse supports anonymous data access to public data sets in the
        |CyVerse Data Commons|. This guide is
        written with the assumption you are a CyVerse account holder. See the
        |Data Store Manual| for more info on anonymous access.
      - - Register: |CyVerse User Portal|
    * - Cyberduck (optional)
      - Cyberduck is a 3rd party application with a graphical user interface
        that allows you to easily upload and download data. (available for Mac
        /PC). You will also need to download our connection profile (bookmark).
      - - |Cyberduck Website|
        - |Cyberduck connection profile|
    * - iCommands (optional)
      - iCommands are a set of command line binaries that can be used to
        interact with the Data Store. Download iCommands (available for Mac/
        Linux) if you want to use these functionalities.
      - - iCommands (for Mac) |Mac OS iCommands Download|
        - iCommands (for Linux; see iCommands CLI) |Linux CLI iCommands Download|
    * - Spreadsheet editor (optional)
      - To edit a metadata template in .csv format, we recommend using a
        spreadsheet editor such as Microsoft Excel or LibreOffice Calc.
      - - Free |LibreOffice|

.. warning::
		When uploading your data to the Data Store you should not upload files/folders
		with names containing spaces (e.g. experiment one.fastq) or name that contain
		special characters (e.g. ~ ` ! @ # $ % ^ & * ( ) + = { } [ ] | \ : ; " ' <
		> , ? /). The Apps on the Discovery Environment and most command line apps
		will typically not tolerate these characters. For long file/folder names the
		use of underscores (e.g. experiment_one.fastq) is the recommended practice.



----

**Fix or improve this documentation**

- Search for an answer:
  |CyVerse Learning Center|
- Ask us for help:
  click |Intercom| on the lower right-hand side of the page
- Report an issue or submit a change:
  |Github Repo Link|
- Send feedback: `learning@CyVerse.org <learning@CyVerse.org>`_

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
.. |data_store_icon| image:: ./img/data_store/datastore-icon.png
    :width: 100
    :height: 150
