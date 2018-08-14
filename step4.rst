|CyVerse logo|_

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

1. If necessary, login to the |discovery_enviornment|.

2. In the Data window, select (checkbox) an individual file you wish to share.

3. From the *Share* menu, select *Create a Public Link*.

4. In the “Manage Data Links” window, select the file you wish to share, and
   click **Create**.

5. A new URL should appear beneath the file name. Click on this URL and the
   click on Copy in order to be presented with a window that will allow you to
   copy the URL to your clipboard. Anyone who you share this link with will be
   able to download the file. You can test the link in a new web browser window.

    |data_links_window|

6. Deactivate a data link by selecting the file; from the *Share* menu click via
   Public Link. Clicking the |delete_icon| delete icon, next to the links you
   wish to inactivate. Once you deactivate the link, anyone with whom you shared
   it with will no longer be able to access that data.

  .. Tip::
    You can quickly create a link to a file by clicking the |link_icon| link icon
    next to file you wish to share. Manage these links using the "Manage Data
    Links" console which is accessible from the *Share* menu as described above.

----

*Share a File/folder in Discovery Enviornment with Another CyVerse User*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Share data with another CyVerse user by granting permission to read, write, or
own files/folders

1. If necessary, login to the |discovery_enviornment|.

2. In the Data window, select (checkbox) file(s), folder(s) you wish to share
   with another user;
   then under the *Share* menus select *Share with Collaborators...*
3. In the “Manage Sharing” menu, under ‘Selected File(s)/Folder(s) the name of
   the files and folders you are currently sharing are displayed. Ensure the
   file you wish to share now is selected.

    |manage_sharing|

4. In the ‘search for users’ field search for the CyVerse user you wish to share
   with by search for their name, or CyVerse username. You may also select
   ‘Choose from Collaborators’ which will bring up a list of people you have
   designated as collaborators.
5. Next, under ‘Permissions’ choose what permission you want to grant the person
   you are sharing this file with.
6. Once you are finished, click Done to begin sharing. The user will be notified
   that a file has been shared with them.

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

..
	#### Comment: Suggested style guide:
	1. Steps begin with a verb or preposition: Click on... OR Under the "Results Menu"
	2. Locations of files listed parenthetically, separated by carets, ultimate object in bold
	(Username > analyses > *output*)
	3. Buttons and/or keywords in bold: Click on **Apps** OR select **Arabidopsis**
	4. Primary menu titles in double quotes: Under "Input" choose...
	5. Secondary menu titles or headers in single quotes: For the 'Select Input' option choose...
	####

----

*Summary*
~~~~~~~~~

This guide has introduced the basic data management tools you need to manage
the lifecycle of Data in CyVerse. There are many more features to explore and
these are detailed in the full `Data Store Manual <https://wiki.cyverse.org/wiki/display/DS/Using+the+Data+Store>`_.


More help and additional information
`````````````````````````````````````

..
    Short description and links to any reading materials

Search for an answer:
    `CyVerse Learning Center <http://learning.cyverse.org>`_ or
    `CyVerse Wiki <https://wiki.cyverse.org>`_

Post your question to the user forum:
    `Ask CyVerse <http://ask.iplantcollaborative.org/questions>`_

----

**Fix or improve this documentation:**

- On Github: `Repo link <https://github.com/CyVerse-learning-materials/data_store_guide_>`_
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
