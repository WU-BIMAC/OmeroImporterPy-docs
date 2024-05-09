OMERO Importer Python Usage
===========================
This section explains how to organize your Image files on the Image Acquisition workstation or in a connected `Networked File System <https://en.wikipedia.org/wiki/Network_File_System>`_ (NFS) drive to prepare for automated metadata annotation and `OMERO <https://www.openmicroscopy.org/omero/scientists/>`_ import using the `OMERO Importer Python <https://github.com/WU-BIMAC/W-IDM_OmeroImporterPy>`_ tool.

Use Case 2: Presence of subdirectories in the Dataset folder
------------------------------------------------------------

During the execution of an experiment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
1.	Open the  ``OMERO_import_template_wMacros_vXX.xlsm`` spreadsheet that was provided to you and fill in the ``Project_Name`` and ``Dataset_Name``fields with unique names that can be used to identify uniquely the Project and the Dataset in OMERO and elsewhere.
2.	``Save as...`` the ``OMERO_import_template_wMacros_vXX.xlsm`` spreadsheet using your chosen “Project Name” and “Dataset Name” as follows: ``Project-Name_Dataset-Name.xlsm``.
3.	 As you execute the different steps of the procedure, fill in the ``Project-Name_Dataset-Name.xlsm`` spreadsheet you have created above with the indicated metadata values, as explained `here <https://omeroimporterpy-docs.readthedocs.io/en/latest/usage2.html>`_.

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
 
   .. image:: figures/README_new_Project_Dataset.png
      :width: 225px
      :align: left

.. note::

   * \* Use a unique name or identifier for the “Project-Name” folder and the same name used for the ``Project_Name`` field in the ``Project-Name_Dataset-Name.xlsm`` spreadsheet.
   * ** Use a unique name or identifier for the “Dataset-Name” folder and use the same name for the ``Dataset_Name`` field in the ``Project-Name_Dataset-Name.xlsm`` spreadsheet.

6. Move the ``Project-Name_Dataset-Name.xlsm`` spreadsheet you filled in above to the “Project-Name” folder as follows:

   .. rst-class:: image-no-text-wrap

   .. image:: figures/README_new_Project_Dataset_Spreadsheet_padding.png
      :width: 675px
      :align: left

    

7. During image acquisition, save image files in a nested subdirectory structure in the corresponding Dataset folder as follows:


   .. figure:: figures/README_new_Folder_structure_Tags.png
      :width: 475px
      :align: left

.. tip::

  In the example above, Images are organized according to two experimental conditions and one treatment, whereas Condition01 will be captured as Tag01, Condition02 will be captured as Tag02, and Treatment011 will be captured as Tag011.

8. Open the filled-in ``Project-Name_Dataset-Name.xlsm`` spreadsheet.
9. Follow the instructions `here <https://omeroimporterpy-docs.readthedocs.io/en/latest/usage2.html>`_, which are also found in the three workbook tabs.
10. Save the file.
11. The `OMERO Importer Python <https://github.com/WU-BIMAC/W-IDM_OmeroImporterPy>`_ tool will run according to the specifications set by your OMERO administrator.
12. When the import process is terminated, you will receive an email confirming that it was correctly executed or alerting you of eventual errors.


