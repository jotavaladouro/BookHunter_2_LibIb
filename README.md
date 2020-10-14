# BookHunter2LibIb
This is a notebook to convert data from Book Hunter toLibIb. 
Here we translate a book collection from Book Hunter to a CSV to import in LibIb. 

Book Hunter is a Book Collection Manager for MacOs that is not supported.

LibIb is a cloud app to manage Book Collections. 

The main problem with this importation is that LibIb must have an ISBN for all books, 
so you need to complete your book information with an ISBN code.


## Build with
* [SqlLitle Studio](https://sqlitestudio.pl/)
* [Jupyter](https://jupyter.org/)
* [isbnlib](https://pypi.org/project/isbnlib/)


# Getting Started

## Prerequisites
* SqlLitle Studio
* python 3
* pip
* jupyter 


## Instalation
```sh
pip3 install isbnlib google-api-python-client urllib3 re
```
If you have a Google API Key, copy to the file GoogleBookApiKey.py .



# Usage

## Export the data
1. Copy Book Hunter data (in my case, it was in /home/User/Lib/Application Support/Book_Hunter/Book_Hunter.bhdata)
2. Change the file extension to bd.
3. Decompress the file. 
4. Open library.sql with SqulLitle Studio.
5. Export ZBOOK table to CSV. Export only tabla data, setting "Column names in the first row".

## Lanch the notebook
```sh
jupyter notebook Hunter2LibIb.py
```

# License
Distributed under the MIT License. 

# Contact
JotaValadouro - jotavaladouro@gmail.com

Project Link: https://github.com/jotavaladouro/BookHunter_2_LibIb/
