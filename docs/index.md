[Learning Center Home](http://learning.cyverse.org/)

# Data Store Guide

## Goal

The Data Store is more than having a place to save your files. The Data
Store is a way to manage the life cycle of your data. From the moment
you create data, to publication and beyond, there are a number of
practices you should follow to ensure the integrity and value of your
data are maintained. This includes making your data FAIR (Findable,
Accessible, Interoperable, and Reusable). The Data Store helps to
achieve this with less effort. This guide will cover the minimum needed
to get you started. Please look through the for a more comprehensive
look at Data Store capabilities.

  Maintainer       Institution      Contact
  ---------------- ---------------- ---------------------
  Jason Williams   CyVerse / CSHL   <Williams@cshl.edu>

------------------------------------------------------------------------

::: {.toctree maxdepth="2"}
Tutorial home \<self> Drag-and-drop Data Transfer with Cyberduck
\<step1.rst> Command Line Transfer with iCommands \<step2.rst> Associate
Data with Metadata \<step3.rst> Data Sharing and Other Features
\<step4.rst> Desktop Access with WebDav \<step5.rst>
:::

## Prerequisites

### Downloads, access, and services

*In order to complete this tutorial you will need access to the
following services/software*

+----------------------+----------------------+----------------------+
| Prerequisite         | Preparation/Notes    | Link/Download        |
+======================+======================+======================+
| CyVerse account      | CyVerse supports     | -   Register:        |
| (optional)           | anonymous data       |                      |
|                      | access to public     |                      |
|                      | data sets in the .   |                      |
|                      | This guide is        |                      |
|                      | written with the     |                      |
|                      | assumption you are a |                      |
|                      | CyVerse account      |                      |
|                      | holder. See the for  |                      |
|                      | more info on         |                      |
|                      | anonymous access.    |                      |
+----------------------+----------------------+----------------------+
| Cyberduck (optional) | Cyberduck is a 3rd   | -                    |
|                      | party application    | -                    |
|                      | with a graphical     |                      |
|                      | user interface that  |                      |
|                      | allows you to easily |                      |
|                      | upload and download  |                      |
|                      | data. (available for |                      |
|                      | Mac /PC). You will   |                      |
|                      | also need to         |                      |
|                      | download our         |                      |
|                      | connection profile   |                      |
|                      | (bookmark).          |                      |
+----------------------+----------------------+----------------------+
| iCommands (optional) | iCommands are a set  | -   iCommands (for   |
|                      | of command line      |     Mac)             |
|                      | binaries that can be | -   iCommands (for   |
|                      | used to interact     |     Linux; see       |
|                      | with the Data Store. |     iCommands CLI)   |
|                      | Download iCommands   |                      |
|                      | (available for Mac/  |                      |
|                      | Linux) if you want   |                      |
|                      | to use these         |                      |
|                      | functionalities.     |                      |
+----------------------+----------------------+----------------------+
| Spreadsheet editor   | To edit a metadata   | -   Free             |
| (optional)           | template in .csv     |                      |
|                      | format, we recommend |                      |
|                      | using a spreadsheet  |                      |
|                      | editor such as       |                      |
|                      | Microsoft Excel or   |                      |
|                      | LibreOffice Calc.    |                      |
+----------------------+----------------------+----------------------+

::: warning
::: title
Warning
:::

When uploading your data to the Data Store you should not upload
files/folders with names containing spaces (e.g. experiment one.fastq)
or name that contain special characters (e.g. \~ \` ! @ \# \$ % \^ & \*
( ) + = { } \[ \] \| : ; \" \' \< \> , ? /). The Apps on the Discovery
Environment and most command line apps will typically not tolerate these
characters. For long file/folder names the use of underscores (e.g.
experiment_one.fastq) is the recommended practice.
:::

------------------------------------------------------------------------

**Fix or improve this documentation**

-   Search for an answer:
-   Ask us for help: click on the lower right-hand side of the page
-   Report an issue or submit a change:
-   Send feedback: [learning\@CyVerse.org](learning@CyVerse.org)

------------------------------------------------------------------------

[Learning Center Home](http://learning.cyverse.org/)
