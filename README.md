# URI strategy IISG
(this document supersedes https://confluence.socialhistoryservices.org/display/DOC/IISG+URI+Strategy)

## Basic structure
The default URI structure is:

`{schema}://{domain}/{type}/{subtype}/{referral}`

where:

| Element    | Example                                                                        |
| ---------- | ------------------------------------------------------------------------------ |
| `{schema}` | 'https://'                                                                     |
| `{domain}` | 'iisg.amsterdam'                                                               |
| `{type}`   | 'authority', 'id', 'vocab'                                                     |
| `{subtype}`| 'collection', 'form', 'organization', 'person', 'place', 'nameofdataset', ...  |


| Authority	| Authority records                                                                       |
| --------- | --------------------------------------------------------------------------------------- |
| id        |	special resources: id has subtypes 'collection', 'dataverse', 'dataset', 'file', 'item' |
|           | For the value-level description of datasets use: 'id/<mydataset>' (see below)           |
| vocab	    | (items in) vocabularies                                                                 | 

and instances of {subtype} are used to indicate:

| Authority	      | Authority records                               |
| --------------- | ----------------------------------------------- |
| collection      |	a collection or archival material               |
| form            | the way in which the content occurs             |
| vocab	          | (items in) vocabularies                         | 
| organization    | organizations                                   |
| person	        | persons                                         |
| place           |	locations                                       |
| 'nameofdataset'	| the name of a dataset, only if type == resource |
| ...	            | ...                                             |

Conventions
Properties are written in lowerCamelCase.
Classes are written in UpperCamelCase.
Dataset specific terms can be retained by using https://iisg.amsterdam/resource/nameofdataset/vocab/myterm not via https://iisg.amsterdam/vocab/nameofdataset/myterm. Also, datasets are so far mainly described using their original column names ('headers'), and are not replaced by the subtypes above. So dataset 'mydata', with column 'municipality' and value 'Amsterdam' tends to be represented as https://iisg.amsterdam/resource/mydata/municipality/Amsterdam.
Examples
https://iisg.amsterdam/id/item/1000000
https://iisg.amsterdam/id/collection/ARCH00293
https://iisg.amsterdam/id/dataset/101 # dataverse metadata
https://iisg.amsterdam/id/file/dataverse-101-1 #dataverse metadata
https://iisg.amsterdam/id/mydataset/mycolumname/myvalue # description of dataset contents (values)

https://iisg.amsterdam/authority/event/(NL-AmISG)2025191
https://iisg.amsterdam/authority/period/2006369
https://iisg.amsterdam/authority/person/(DE-588)118578537
https://iisg.amsterdam/authority/organization/(DE-588)1065494610

https://iisg.amsterdam/vocab/CollectionShape
https://iisg.amsterdam/vocab/Postcard
