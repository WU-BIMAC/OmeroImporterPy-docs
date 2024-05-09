Metadata annotation Excel spreadsheet
================================================
This section explains how to fill in metadata values in customized metadata annotation Excel spreadsheets to prepare for automated metadata annotation and `OMERO <https://www.openmicroscopy.org/omero/scientists/>`_ import using the `OMERO Importer Python <https://github.com/WU-BIMAC/W-IDM_OmeroImporterPy>`_ tool.

1.	Open the  ``OMERO_import_template_wMacros_vXX.xlsm`` spreadsheet that was provided to you and fill in the ``Project_Name`` and ``Dataset_Name`` fields as explained in Points 4 and 10.
2.	``Save as…`` the ``OMERO_import_template_wMacros_vXX.xlsm`` spreadsheet using your chosen *“Project Name”* and *“Dataset Name”* as follows: ``Project-Name_Dataset-Name.xlsm``.
3.	 As you execute the different steps of the procedure, fill in the ``Project-Name_Dataset-Name.xlsm`` spreadsheet with the indicated metadata values as explained in Points 7 and 14.

Project TAB
-----------
4.	Fill in cells C10 and C11 with the name and description of the Project; the same values will be used to fill in C14 and C15, respectively.
5.	Skip C12.
6.	Choose an Overwrite status for cell C13. 

.. note::

   * Overwrite is set to ``No`` by default. In this case, if an existing Project with the same name exists in OMERO, existing Key-Value pairs will be maintained. 
   * On the other hand, when Overwrite is set to ``Yes``, the Key-Value pairs in the spreadsheet will be used to overwrite existing Project Key-Value pairs in OMERO (e.g., this might be useful in case errors need to be corrected).


7.	Starting from C16, fill in all relevant metadata in the Value column (Column C) or choose from existing allowable values.
8.	Leave the ones you do not need empty. They will be skipped.
9.	Save the file.

Dataset TAB
-----------
10.	Fill in cells C10 and C11 with Dataset_Name and Dataset_Description.
11.	If the value in C12 is set to ``Study_Component``, the values in C10 and C11 will be used to fill in C14 and C15, respectively. 
12.	Skip C12.
13.	Choose an Overwrite status for cell C13. 

.. note::

   * Overwrite is set to ``No`` by default. In this case, if an existing Dataset with the same name exists in OMERO, existing Key-Value pairs will be maintained. 
   * On the other hand, when Overwrite is set to ``Yes``, the Key-Value pairs in the spreadsheet will be used to overwrite existing Project Key-Value pairs in OMERO (e.g., this might be useful in case errors need to be corrected).

14.	Starting from C16, fill in all relevant metadata in the Value column (Column C) or choose from existing allowable values.
15.	Leave the ones you do not need empty. They will be skipped.
16.	Save the file.


Image-List TAB
--------------
17.	In the ``IMAGE LEVEL KEY-VALUE PAIRS`` columns, starting at Column E, fill in relevant metadata (leave the ones you do not need empty).
18.	Save the file.

.. note::

   * Use the ``Select Metadata`` button to select the filled-in metadata information and quickly transfer it to another file.
   * Use the ``Jump to Allowed values list`` button to quickly move to the ``Allowed value`` tab.

