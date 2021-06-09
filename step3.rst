.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


**Associate Data with Metadata**
--------------------------------

The Data Store supports a variety of solutions that allow you to associate your
raw data with metadata. Metadata is of critical importance to a quality research,
(See this article on `FAIR Principles <https://www.nature.com/articles/sdata201618>`_)
yet it is often given less consideration until the time of publication and
sharing. Here are a few metadata features that you can adopt and be aware of at
the outset, see more of CyVerse's capabilities on the `Data Commons <https://wiki.cyverse.org/wiki/display/DC/Data+Commons+Home>`_
page.

.. #### Comment: short description

**Some things to remember about the platform**

- You can add metadata to a single file/folder, or in bulk to large collections
  of data. You can use your own metadata schema, or apply one of our `metadata templates <https://wiki.cyverse.org/wiki/display/DEmanual/Using+Metadata+in+the+DE#UsingMetadataintheDE-AttachTemplate>`_
- The Discovery Environment supports several metadata templates that can be used
  for submission of metadata. Additional templates you may wish to use can be
  found at resources like `FairSharing.org <https://fairsharing.org/>`_
- Metadata can be managed through a graphical interface in the Discovery Environment
  or using iCommands at the command line. We will only cover the Discovery Environment
  in this guide. See instructions for `iCommands metadata <https://wiki.cyverse.org/wiki/display/DS/Adding+Metadata+to+a+File+Using+iRODS+imeta+%28Metadata%29+Commands>`_
  on the CyVerse wiki.

----

*Adding Metadata to a Single File/folder in the Discovery Environment*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. note::
   You must have `write` or `own` permission to edit an object's metadata.

1. Log into the |discovery_enviornment|.

2. Click on the **`Data`** icon to open a Data window. Select (checkbox) a
   single file/folder to add metadata to.

3. Click on the **`Metadata`** menu and select `Edit / View Metadata`. Click the
   `Add` button to add a single metadata entry in Attribute, Value, Unit (AVU) format.
   Click `Save` to save that entry.

   |edit_view_metadata|

   .. tip::
      A single piece of metadata, or an AVU, is made up of attributes, values,
      and units. An attribute is a changeable property or characteristic of the
      file or folder you have selected that can be set to a value. For example,
      length is an attribute of a file, while 7 is its value, and cms is the
      unit.

4. Click 'Save' to save all entries and apply the metadata.

*Adding Metadata to Multiple Files/folder in the Discovery Environment*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Adding Metadata using a CyVerse Template**

1. Log into the |discovery_enviornment|.

2. Click on the **`Data`** icon to open a Data window. Click on the **`Metadata`**
   menu and select `Download template`. Select a template and click `OK` to
   download. (In this example, we will use the `DOI Request - DataCite Metadata`)
   template.

3. Unzip the downloaded template; it will contain |blank| and |guide|.
   Open these files using the spreadsheet editor of your choice.

   .. tip::
      - `blank.csv` is the metadata template that you will complete for your data
      - `gude.csv` contains instructions for your template, and will usually  include
         controlled vocabulary terms for metadata descriptors.

4. Edit the template in one of two ways:

  - *If all data will be in a single folder*

    a. In the guide.csv spreadsheet, add a row for the first data file.

    b. In the first column of the first row, enter the file location in the Data
       Store.

    c. In the remaining columns of the first row, enter the values for each
       file/attribute combination.

    d. Repeat for each file.

    e. If desired, add additional columns to the end of the template. The
       metadata in the additional columns will be saved in the Data Store but
       will not be stored as part of the template.

    f. Save the file in **CSV format**. Make sure none of the names of the files or
       the parent folder includes spaces or special characters.

  - *If data will be in multiple folders*

    a. In the guide.csv spreadsheet, add a row for the first data file.

    b. In the first column of the first row, enter the **full path**
       to the file location in the Data Store. (e.g. /iplant/home/cyverse_username/data_folder)

    c. In the remaining columns in the first row, enter the values for each
       file/attribute combination.

    d. Repeat for each file.

    e. If desired, add additional columns to the end of the template. The
       metadata in the columns will be saved in the Data Store but will not
       be stored as part of the template.

    f. Save the file in **CSV format**. Make sure none of the names of the files or
       the parent folder includes spaces or special characters.

5. In an open 'Data' window in the Discovery Environment, navigate to appropriate
   location for uploading the template:

   - If the first column of your metadata file contains only file names
     (that is, all data files are in the same folder), move the bulk metadata
     file to the same folder as the location of the data files.
   - If the first column of your metadata file contains the full path to each
     file (that is, the data files are in different folders), it does not
     matter where the metadata file is located on the Data Store.

    In the Data window, under the **Upload** menu, select 'Simple Upload from
    Desktop' to upload the modified `guide.csv`.

6. To apply the metadata, in the Data window, select (checkbox) the name of the
   folder containing the data files to which you want to apply the metadata in
   bulk.

7. Click the **`Metadata`** menu and select 'Apply Bulk Metadata', and the click
   'Select Metadata File'.

8. Browse to the location of the bulk metadata file and select it.

9. Select the corresponding template from the dropdown menu; click "Okay"

Your metadata should now be applied to your files. You should receive a notification
in the Discovery Enviornment and you can confirm the metadata has been correctly
applied by selecting 'View / Edit Metadata' from the **`Metadata`** menu of a
Data window.










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
.. |edit_view_metadata| image:: ./img/data_store/edit_view_metadata.png
    :width: 400
    :height: 150
.. |discovery_enviornment| raw:: html

    <a href="https://de.cyverse.org/de/" target="_blank">Discovery Environment</a>
.. |blank| raw:: html

    <a href="http://datacommons.cyverse.org/browse/iplant/home/shared/cyverse_training/platform_guides/data_store/doi_metadata_template/guide.csv" target="_blank">blank.csv</a>
.. |guide| raw:: html

    <a href="http://datacommons.cyverse.org/browse/iplant/home/shared/cyverse_training/platform_guides/data_store/doi_metadata_template/blank.csv" target="_blank">guide.csv</a>
