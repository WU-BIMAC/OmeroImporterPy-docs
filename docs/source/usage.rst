Usage
=====
This section explains how to organize your Image files on the Image Acquisition workstation or in a connected `Networked File System <https://en.wikipedia.org/wiki/Network_File_System>`_ (NFS) drive to prepare for automated metadata annotation and `OMERO <https://www.openmicroscopy.org/omero/scientists/>`_ import using the `OMERO Importer Python <https://github.com/WU-BIMAC/W-IDM_OmeroImporterPy>`_ and the associated `OMERO Importer Excel Helper <https://github.com/WU-BIMAC/W-IDM_OmeroImporterExcelHelperPy>`_ tool.

Use Case 2: Presence of subdirectories in the Dataset folder
------------------------------------------------------------

During the execution of an experiment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
1.	Open the  ``OMERO_import_template_wMacros_vXX.xlsm`` spreadsheet that was provided to you and fill in the ``Project_Name`` and ``Dataset_Name``fields with unique names that can be used to identify uniquely the Project and the Dataset in OMERO and elsewhere.
2.	``Save as...`` the "OMERO_import_template_wMacros_vXX.xlsm" spreadsheet using your chosen “Project Name” and “Dataset Name” as follows: ``Project-Name_Dataset-Name.xlsm``.
3.	 As you execute the different steps of the procedure, fill in the ``Project-Name_Dataset-Name.xlsm`` spreadsheet you have created above with the indicated metadata values, as explained `here <>`_.

.. note::

   This will take some time at first. However, things will get much easier going forward, as you can often copy   previously filled-in spreadsheets and only change the relevant metadata values (e.g., Date, Biosample information, Specimen information, Channel Names, etc.). Also, you can often use filled-in spreadsheets from lab mates performing the same experiment type as a starting point.

.. tip::

  If you need to change the structure of the spreadsheet template, please ask your Data Curator for help.

In preparation for Image data OMERO import
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
4. On the folder you will use as the source for OMERO import, create a subfolder called ``User_Name_OMERO`` where “User_Name” is your OMERO username.

When you are ready to import your first images to OMERO
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
5. In the ``User_Name_OMERO`` folder, create the following folder structure:

.. image:: docs/source/figures/README_new_Project_Dataset.png
    :width: 200px
    :align: left
    :height: 100px
    :alt: alternate text

