---
title: "Searching NCBI Genbank"
weight: 1900
---

# Searching NCBI Genbank

UGENE enables users to search data in the NCBI GenBank remote database. To do this, open the following dialog through the main menu by selecting _File->Search NCBI Genbank_:

![](/images/65929336/65929337.jpg)

To search for data in the nucleotide or protein databases, enter a general text query in the search field, select the appropriate database, and click the _Search_ button. You can use a protein name, gene name, or gene symbol directly. Searching for a submitter or author name in the specific format will yield the best results.

Use the boolean operator AND to find records containing all your search terms, which is the intersection of search results.

Use the boolean operator OR to find records that include any of several search terms, which is the union of search results.

Use the boolean operator NOT to exclude records matching a particular search term.

To limit the results, use the _Result limit_ field.

After clicking the _Search_ button, UGENE searches for the biological objects and displays them in the _Results_ field. You can download the object(s) by selecting one or more objects (to select multiple objects, use the _Ctrl_ button) and clicking the _Download_ button. The dialog will appear:

![](/images/65929336/65929339.png)

The meanings of all parameters are similar to those in the dialog _Fetch Data from Remote Database_, which is accessed through _File→Access Remote Database_.

You can save the downloaded file in one of two formats: fasta or GenBank.

The _Force download appropriate sequence_ parameter is not available if you select the fasta format.

After clicking the _OK_ button, UGENE downloads the biological objects and adds them to the current project if the _Add to project_ option is checked.