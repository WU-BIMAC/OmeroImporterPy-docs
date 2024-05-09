OMERO Importer Excel Helper
===========================

19.	Launch the ``Project-Name_Dataset-Name.xlsm`` file created `here <https://omeroimporterpy-docs.readthedocs.io/en/latest/usage.html>`_ and filled-in `here <https://omeroimporterpy-docs.readthedocs.io/en/latest/usage2.html>`_
20.	Open the ``Image-List`` tab.
21.	 Check that B9 contains the correct “Dataset-Name”.
22.	In cell B10, enter all the extensions of all Image data files you want to import to OMERO. Separate each extension with a comma as follows:

	``ext1, ext2, …, extN``

23.	Click on the button called "Auto-fill Image Names and Tags "to explore the “Dataset-Name” folder. Then, auto-fill the names and file paths of the Image files and assign Tags to each image file depending on its position in the file system. 

   .. figure:: figures/README_new_Folder_structure_Tags.png
      :width: 475px
      :align: left

.. Tip::

   In the directory structure above, Image-file01 would be assigned Tag01 and Tag011, and Image-file11 would be assigned Tag02, respectively. 
