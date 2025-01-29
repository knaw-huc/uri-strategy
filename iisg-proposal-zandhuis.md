# PIDs, URLs and URIs @IISH

## Library
### Current situation
For reference, different webaddresses for the same book:
- URI of description: https://iisg.amsterdam/id/item/397374 
        -> resolves to druid, data contains PID als object in the property iisgv:nativeViewer
- PID of description: https://hdl.handle.net/10622/E02E622C-9176-401D-BFE6-9215AF0970DE 
        -> redirects to https://search.iisg.amsterdam/Record/397374
- URL of description: https://search.iisg.amsterdam/Record/397374
- URL of IIIF manifest: https://access.iisg.amsterdam/iiif/presentation/N10213901/manifest
- PID of IIIF manifest: https://hdl.handle.net/10622/N10213901 
        -> redirects to https://access.iisg.amsterdam/universalviewer/#?manifest=https://access.iisg.amsterdam/iiif/presentation/N10213901/manifest

### Suggestions for improvements?
There is yet another identifier for the digital representation, which is a reasonable choice. But not consequently applied in archives ...

>> ok. this we then need to discuss in detail and at least have a general guideline. re different uri's for digital representations, according to ppl at the VU, this is a browser issue. So should have 1 uri, but do something specific to tell your browser that it needs to go a specific view. Not sure whether that works in practice.

## Archival fonds
### Current situation
Different webaddresses for the same archive:
- PID of description: https://hdl.handle.net/10622/ARCH00860
        -> redirects to https://search.iisg.amsterdam/Record/ARCH00860
- URL of description: https://search.iisg.amsterdam/Record/ARCH00860

### Suggestions
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860

>> agreed.


If you want to diminish the amount of blank nodes:
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860#title01
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860#date01
Would this resolve in druid? Otherwise replace '#' with '/' or '_' or something else.

>> I think '/' are needed. Clicking the link gives the error: `Resource https://iisg.amsterdam/id/recordresource/ARCH00860 does not appear in this dataset.` indicating it misses the #xxx part. 
Not sure about diminishing blank nodes. See https://collectiedata.hetnieuweinstituut.nl/the-other-interface/knowledge-graph/browser?resource=https%3A%2F%2Fcollectiedata.hetnieuweinstituut.nl%2Fid%2Fpeople%2F18153


## Archival file
### Current situation
Different webaddresses for the same archival file:
- PID of description: https://hdl.handle.net/10622/ARCH00860.A_57 (only available because this thing is digitised)
        -> redirects to https://search.iisg.amsterdam/Record/ARCH00860/ArchiveContentList#A_57
- URL of description: https://search.iisg.amsterdam/Record/ARCH00860/ArchiveContentList#A_57
- URL of IIIF manifest: https://access.iisg.amsterdam/iiif/presentation/ARCH00860.A_57/manifest
- PID of IIIF manifest:  https://hdl.handle.net/10622/ARCH00860.A_57?locatt=view:manifest
        redirects to: https://access.iisg.amsterdam/iiif/presentation/ARCH00860.A_57/manifest



### Suggestions
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860.A_57

>> agreed.

If you want to diminish the amount of blank nodes:
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860.A_57#title01
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860.A_57#date01

>> not sure. see: https://collectiedata.hetnieuweinstituut.nl/the-other-interface/knowledge-graph/browser?resource=https%3A%2F%2Fcollectiedata.hetnieuweinstituut.nl%2Fid%2Fpeople%2F18153


