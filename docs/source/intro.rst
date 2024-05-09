Introduction
============

Research Data Management best practices
---------------------------------------
It is considered a best practice in `Research Data Management <https://rdmkit.elixir-europe.org/data_organisation#how-do-you-organise-files-in-a-folder-structure>`_ (RDM) to organize files within **folders**. 

For Image data files, at a minimum, think about a **two-level structure**, where level one reflects the name of the **Project** and level two reflects the name of individual **Datasets**, which could correspond to individual Image acquisition sessions. 

In addition, organizing your images in further nested subdirectories is often recommended. This allows distinguishing different **experimental conditions** (e.g.,treatment01 vs. treatment02, condition01 vs. condition02) and **sample characteristics** (e.g., wild type vs. mutant, etc.) and subdivide Image files accordingly. 

OMERO image data organization
-----------------------------
OMERO organizes data using two default nested container (i.e., “directory”) levels: **Project** and **Dataset**. In addition, OMERO offers the possibility of assigning **tag annotations** to Image files to create **virtual nested sub-directories** that allow Image file classification and facilitate search.

Typically, the OMERO Project contains the images produced by a series of related experiments that aim to answer the same scientific question (e.g., `REMBI <https://doi.org/10.1038/s41592-021-01166-8>`_ or `ISA <https://isa-specs.readthedocs.io/en/latest/index.html>`_ ``Study``). Conversely, the OMERO Dataset typically contains images produced during an individual image acquisition session related to a particular experiment (e.g., `REMBI <https://doi.org/10.1038/s41592-021-01166-8>`_ ``Study Component`` or `ISA <https://isa-specs.readthedocs.io/en/latest/index.html>`_ ``Assay``). 

As such, one Project will contain multiple Datasets, each containing various images. In addition, Tags can be assigned to sub-sets of Image files in a given Dataset to create virtual sub-directories to reflect on individual conditions or treatments.

.. tip::

  Please Note - If your images are organized in more than two subdirectory levels or you want to use Tags to organize image files further in OMERO, the OMERO Importer Python tools can facilitate mapping your subfolder structure into OMERO Tags. 
