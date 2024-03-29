.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


**Data Sharing and Other Features**
-----------------------------------

One of the most powerful features of the Data Store is to share all of your
data instantly, and with fine-grained permission control. You can share your
data with other CyVerse users, and you can also make data available to
anonymous users and with identifiers (e.g. DOIs, ARKs) through the CyVerse
`Data Commons <https://wiki.cyverse.org/wiki/display/DC/Data+Commons+Home>`_.
We will cover the most basic, commonly used sharing features in this guide.


.. #### Comment: short description

----

*Share a File in Discovery Environment with a URL (Public Link)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
You can quickly share files in your Data Store using a Discovery Environment
Public Link.

.. Note::
  You can **only share individual files** using the quick link. Since files are
  shared over HTTP this is only recommended for small files. This is a convenient
  , but less secure method for file transfer. Do not share sensitive/private
  data using these links.

1. If necessary, login to the |Discovery Environment|.

2. In the Data window, select (checkbox) one or more individual file(s) (not
   folders) you wish to share.

3. From the *More actions* menu, select *Public Link(s)*.

4. A new URL will be provided for you in a pop-up. Highlight and copy or click
   on Copy in order to be presented with a window that will allow you to
   copy the URL to your clipboard. Anyone who you share this link with will be
   able to download the file. You can test the link in a new web browser window.

   |public link|

  .. Tip::
    You can quickly create a link to a file by clicking the "3 dots" icon next \
    to any file and selecting "Public Link".

*To deactivate a public link*

1. To deactivate a link, select (checkbox) one or more individual file that has
   been shared with a public link; then click on the *Details* menu.

2. In the details menu under the *Permissions* tab, click the "pencil" icon
   next to "cyverse-anonymous@cyverse.org" to edit the permission.

----

*Share a File/folder in Discovery Environment with Another CyVerse User*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Share data with another CyVerse user by granting permission to read, write, or
own files/folders

1. If necessary, login to the |Discovery Environment|.

2. In the Data window, select (checkbox) file(s), folder(s) you wish to share
   with another user; then under the *Share* menus enter the CyVerse username, email, or group name you wish to share with.
3. Next, under ‘Permissions’ choose what permission you want to grant the
   recipient(s) you are sharing this file with.

   |sharing|

4. Once you are finished, click Done to begin sharing. The user will be notified
   that a file has been shared with them.

   .. tip::

      You can share several files/folders at once by selecting them and then clicking the "Add to Bag" button in the Data window.

   .. hint::
      By managing access to data, the DE allows you to share large datasets
      instantaneously. Data permissions (based on UNIX permissions) are
      described in this chart:

      .. list-table::
          :header-rows: 1

          * - Permission level
            - Read
            - Download/Save
            - Metadata
            - Rename
            - Move
            - Delete
          * - Read
            - **X**
            - **X**
            - **View**
            -
            -
            -
          * - Write
            - **X**
            - **X**
            - **Add/Edit**
            -
            -
            -
          * - Own
            - **X**
            - **X**
            - **Add/Edit**
            - **X**
            - **X**
            - **X**

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
.. |data_window| image:: ./img/de/data_window.png
    :width: 550
    :height: 300
.. |viewing_window| image:: ./img/de/viewing_window.png
    :width: 400
    :height: 200
.. |data_links_window| image:: ./img/de/manage_data_links.png
    :width: 450
    :height: 250
.. |delete_icon| image:: ./img/de/delete_icon.png
    :width: 15
    :height: 15
.. |link_icon| image:: ./img/de/link_icon.png
    :width: 15
    :height: 15
.. |manage_sharing| image:: ./img/de/manage_sharing_menu.png
    :width: 400
    :height: 300
.. |discovery_enviornment| raw:: html

    <a href="https://de.cyverse.org/de/" target="_blank">Discovery Environment</a>
