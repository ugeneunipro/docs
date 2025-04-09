---
title: "Searching NCBI Genbank"
weight: 1900
---


# Searching NCBI Genbank

UGENE allows searching data in NCBI GenBank remote database. To do this open the following dialog by _File->Search NCBI Genbank_ main menu:


![](/images/65929336/65929337.jpg)

To search data in the nucleotide or protein databases enter a general text query to the search field, select the database and click on the _Search_ button. You can use a protein name, gene name, or gene symbol directly. Searching for a submitter or author name in the following format will produce the best results.

Use the boolean operator AND to find records that contain every one of your search terms, the intersection of search results.

Use the boolean operator OR to find records that include one of several search terms, the union of search results.

Use the boolean operator NOT to exclude records matching a search term.

To limit results use the _Result limit_ field.

After you click the _Search_ button, UGENE searches the biological objects and shows it in the _Results_ field. You can download the object(s). Select one or several objects (for selecting several objects use the _Ctrl_ button) and click the _Download_ button. The dialog will appear:


![](/images/65929336/65929339.png)

The meanings of all parameters are similar to the parameters from the dialog _Fetch Data from Remote Database_ which is called through _File→Access Remote Database_.

You can save the downloaded file in one of two formats: fasta or GenBank.

_Force download appropriate sequence_ parameter is not available if you select fasta format.

After you click the _OK_ button, UGENE downloads the biological objects and adds it to the current project if _Add to project option_ is checked.
