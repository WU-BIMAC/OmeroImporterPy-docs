Introduction
============

Research Data Management best practices
---------------------------------------
It is considered a best practice in Research Data Management (RDM) to organize files within folders and sub-folders. For Image data files, at a minimum, think about a two-level structure, where level one reflects the name of the project and level two reflects the name of individual datasets, which could correspond to individual Image acquisition sessions. 
In addition, organizing your images in further nested subdirectories is often recommended. This allows you to distinguish different imaging experiment conditions (e.g., wild type vs. mutant, treatment01 vs. treatment02, condition01 vs. condition02, etc.) and subdivide Image files accordingly. 

OMERO image data organization
-----------------------------
OMERO organizes data by utilizing two default nested container (i.e., “directory”) levels: Project and Dataset. In addition, OMERO offers the possibility of assigning Tags to Image files to create virtual nested sub-directories that allow Image file classification and facilitate search.
Typically, the OMERO Project contains the images produced by a series of related experiments that aim to answer the same scientific question (e.g., REMBI or ISA Study). Conversely, the OMERO Dataset typically contains images produced during an individual image acquisition session related to a particular experiment (e.g., REMBI Study Component or ISA Assay). As such, one Project will contain multiple Datasets, each containing various images. In addition, Tags can be assigned to sub-sets of Image files in a given Dataset depending on individual conditions or treatments to create virtual sub-directories.
If your images are organized in more than two subdirectory levels or you want to use Tags to organize image files further in OMERO, the OMERO importer tools can facilitate mapping your subfolder structure into OMERO Tags. 
