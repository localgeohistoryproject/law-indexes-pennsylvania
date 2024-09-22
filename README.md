# Law Indexes: Pennsylvania

## Summary

As part of efforts to expand the Local Geohistory Project, which aims to educate users and disseminate information concerning the geographic history and structure of political subdivisions and local government, this repository has been created to disseminate law index data for the Commonwealth of Pennsylvania. This index currently covers a portion of the private and special laws only from 1700 through 1892.

Private and special laws concern one or several individuals, entities, or localities, unlike public or general laws, which apply to all similarly situated individuals, entities, and localities within a jurisdiction. Prior to the Constitution of 1874, private and special laws were a common method used to alter municipal and county boundaries and forms of government. The law index is released as a tab-separated values (TSV) file, **output/PaLawIndex.tsv**.

This repository does not contain the full text of the laws, nor does it currently contain links to the full text. Because the index was created using OCR technology, it may contain uncaptured errors. This preliminary release is subject to additional caveats explained in the Methodology.

## Harmful Content

The terms used in the law indexes were drawn from Source Works that were written before current diversity, equity, and inclusion principles were developed, and have not been updated to reflect modern standards. Some terms may:[^1]

- reflect racist, sexist, ableist, misogynistic/misogynoir, and xenophobic opinions and attitudes;
- be discriminatory towards or exclude diverse views on sexuality, gender, religion, and more;
- demonstrate bias and exclusion in the subjects documented.

## Using tab-separated values (TSV) files

TSV files do not use quotation marks to escape fields containing tabs; therefore, the **String delimiter** option in LibreOffice Calc or the **Text qualifier** option in Microsoft Excel must be left blank to ensure the file imports accurately.

The file uses Unix-style [line endings](https://en.wikipedia.org/wiki/Newline#Representations) (LF), which may have to be adjusted in applications that expect Windows-style line endings (CR LF).

A header row containing column names is included. When importing into a relational database system, like PostgreSQL, it may be necessary to remove this header line, particularly when using the [PostgreSQL COPY function](https://www.postgresql.org/docs/16/sql-copy.html) in the Text Format.

## Source Works

The following Source Works were used to create this law index:

| Citation | Coverage | Online Version | Notes |
| -------- | -------- | -------------- | ----- |
| Price, Giles D., comp. *Index to local legislation in Pennsylvania from 1700 to 1892: together with an index to the titles of corporations organized by special acts, and to all laws relating thereto.* Philadelphia, Pa.: T. & J. W. Johnson, 1894. | 1700-1892 | [Internet Archive](https://archive.org/details/indextolocallegi00pric/) | Copyright expired in the United States. Version used for this index taken from cited Online Version. |

Prior to inclusion, source works were examined to determine whether they fell under the public domain in the United States, using the following guides:

Hirtle, Peter B. "Copyright Services: Copyright Term and the Public Domain." *Cornell University Library.* 2004-2023. <https://guides.library.cornell.edu/copyright/publicdomain>.

U.S. Copyright Office. *Compendium of U.S. Copyright Office Practices,* 3rd ed. 2021. § 313.6(C). <https://www.copyright.gov/comp3/docs/compendium.pdf#page=83>.

## Methodology

The data included in this resource was primarily processed in 2012 and prior, and no contemporaneous methodology document was created detailing the data transformations used as part of data cleaning. In some cases, when data in the Source Works was determined to be incomplete or erroneous, additional information may have been added that is not derived from the Source Works. Some spellings were standardized across the data; for example, Pittsburgh is generally spelled with the final h, despite the general omission of the character in the Source Works.

The data included in this resource is incomplete, and is not an exact transcription of the Source Works. Because the data was created to facilitate the compilation of information concerning local government formations, charter amendments, and boundary changes, the Corporations group of the Source Works was never processed, and is not included in this repository.

Because Smith's Laws often do not contain the full text of laws, an effort was made to translate these citations to use the Statutes as Large instead when available.

[^1]: Some content in this section was derived from the following work: National Archives and Records Administration. *NARA's Statement on Potentially Harmful Content.* 17 June 2022. <https://www.archives.gov/research/reparative-description/harmful-content>.
