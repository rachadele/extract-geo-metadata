# GEO Metadata Extractor

## Overview
The GEO Metadata Extractor is a Python script designed to simplify the process of downloading and extracting metadata from MINiML files for Gene Expression Omnibus (GEO) datasets. This script is particularly useful for researchers and data scientists working with GEO datasets who want to extract metadata for further analysis.

## Features
Downloads MINiML files for a given GEO accession (GSE) from the GEO FTP server.
Parses the MINiML file to extract metadata for all samples.
Allows filtering of samples to include only "Homo sapiens" (human) data using the --human flag.
Outputs the extracted metadata in a tab-separated values (TSV) file for easy analysis.

## Usage
1. Clone this repository to your local machine:
```
git clone https://github.com/rachadele/extract-geo-metadata.git
cd extract-geo-metadata
```
2. Install the required Python libraries:
```
pip install -r requirements.txt
```
3. Run the script to extract metadata for a specific GSE accession. Replace GSE123456 with the desired GSE accession:
```
python geo_metadata_extractor.py GSE123456
```
4. To filter for human data, use the --human flag:
```
python geo_metadata_extractor.py GSE123456 --human
```
5. The extracted metadata will be saved as a TSV file named GSE123456.tsv in the same directory.

## Acknowledgments
This script uses the BeautifulSoup library for XML parsing.
It relies on the GEO FTP server for data retrieval.
