|CyVerse logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


**Command Line Transfer with iCommands**
----------------------------------------

iCommands is a collection of tools developed by the `iRODS <https://irods.org/>`_
project. iRODS is the technology that supports the CyVerse Data Store. Using
iCommands is the most flexible way to interact with the Data Store.

.. #### Comment: short description

**Some things to remember about iCommands**

- This is a *command line* tool: While many biologists don't have much command
  line experience, we hope you will try to follow along anyway. There are lots
  of free available training including `Software Carpentry <https://software-carpentry.org/>`_ and
  Data Carpentry `<http://www.datacarpentry.org/>`_
- Poor support for *Windows*: Currently, we have not tested a Windows version
  of iCommands and

----

*iCommands Installation Using Mac OSX*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. note::
    iCommands is updated frequently. This tutorial assumes you have followed the
    directions to download and install iCommands following the instructions for
    `Linux <https://wiki.cyverse.org/wiki/display/DS/Setting+Up+iCommands#SettingUpiCommands-linux>`_
    or `Mac <https://wiki.cyverse.org/wiki/display/DS/Setting+Up+iCommands#SettingUpiCommands-mac>`_
    following our current best recommendation on the wiki. **We will detail the
    install instructions in this guide using the Mac installer.**

1. Assuming you are installing from Mac OSX, download the CyVerse-specific
   `iCommands Installer 4.1.9 <https://wiki.cyverse.org/wiki/download/attachments/28117338/cyverse-icommands-4.1.9.pkg?version=3&modificationDate=1472845229000&api=v2>`_.
   Follow the installation instructions.

   .. tip::

      When opening the package, you may get a security warning noting the file
      is from "an unidentified developer." To open anyway, go to the OSX
      'System Preferences' and select the 'Security & Privacy' menu. At the
      bottom of the menu,  there should be and 'Open Anyway' button that will
      allow you to proceede. Follow the prompts to begin the installation.

By default, this installation will place iCommands in your system `PATH` so
you should be ready to run iCommands immediately at the terminal.

----

*iCommands First-time Configuration*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. note::
    Once iCommands is installed and in the system `PATH` these instructions
    apply at a terminal in Mac OSX and Linux systems.

1. Open a terminal and use the `iinit` command to start the configuration
   process. When prompted, enter the values shown below as comments in the
   example code block.

   .. code:: bash

     $ iinit
     One or more fields in your iRODS environment file (.irodsEnv) are
     missing; please enter them.
     Enter the host name (DNS) of the server to connect to: #data.cyverse.org
     Enter the port number: #1247
     Enter your irods user name: #your_cyverse_username
     Enter your irods zone: #iplant
     Those values will be added to your environment file (for use by
     other i-commands) if the login succeeds.

     Enter your current iRODS password: #your_cyverse_password

2. Verify that your iCommands installation works and is properly configured
   using the `ils` command to list the contents of your Data Store home
   directory.

   .. code:: bash

      $ ils
      /iplant/home/your_home_directory:
    file1
    file2
    file3
    C- /iplant/home/your_home_directory/analyses
    C- /iplant/home/your_home_directory/another_folder

----

*Upload Files/folders from local Computer to Data Store*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. warning::
   When uploading your data to the Data Store you should not upload files/folders
   with names containing spaces (e.g. experiment one.fastq) or name that contain
   special characters (e.g. ~ ` ! @ # $ % ^ & * ( ) + = { } [ ] | \ : ; " ' <
   > , ? /). The Apps on the Discovery Environment and most command line apps
   will typically not tolerate these characters. For long file/folder names the
   use of underscores (e.g. experiment_one.fastq) is the recommended practice.

.. tip::

    There are several optional arguments that the upload iCommand `iput` can
    take:

      .. code:: bash

        $ iget -r # For recursive transfer of directories and their contents

        $ iget -P # display the progress of the upload

        $ iget -f # force the upload and overwrite

        $ iget -T # Renew socket connection after 10 min (May help connections
                  # that are failing due to some connection/firewall settings)


    See the `full iCommands documentation <https://docs.irods.org/master/icommands/user/#iput>`__
    for more information.

1. Upload a directory using the `iput` command

   .. code:: bash

      $ iput -rPT /local_directory /iplant/home/cyverse_username/destination_folder
        # This command will output the progress as it uploads your local directory

----

*Download Files/folders from Data Store to local Computer*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. tip::

    There are several optional arguments that the upload iCommand `iget` can
    take:

      .. code:: bash

        $ iget -r # For recursive transfer of directories and their contents

        $ iget -P # display the progress of the upload

        $ iget -f # force the upload and overwrite

        $ iget -T # Renew socket connection after 10 min (May help connections
                  # that are failing due to some connection/firewall settings)


    See the `full iCommands documentation <https://docs.irods.org/master/icommands/user/#iget>`_
    for more information.

1. Download a file using the `iget` command

   .. code:: bash

      $ iget -PT /iplant/home/cyverse_username/target_file /local_destination
        # This command will output the progress as it downloads to your local machine


----

*Additional Frequently Used iCommands*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In addition to the commands above, there are several frequently used iCommands
- most of which you would expect following the Linux paradigm:

- **ipwd**: Print current directory
- **imkdir**: Create a directory
- **icd**: Change directory


----

**Fix or improve this documentation:**

- On Github: `Repo link <https://github.com/CyVerse-learning-materials/data_store_guide>`_
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
