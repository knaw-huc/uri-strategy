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

## Archival fonds
### Current situation
Different webaddresses for the same archive:
- PID of description: https://hdl.handle.net/10622/ARCH00860
        -> redirects to https://search.iisg.amsterdam/Record/ARCH00860
- URL of description: https://search.iisg.amsterdam/Record/ARCH00860

### Suggestions
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860

If you want to diminish the amount of blank nodes:
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860#title01
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860#date01
Would this resolve in druid? Otherwise replace '#' with '/' or '_' or something else.

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

If you want to diminish the amount of blank nodes:
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860.A_57#title01
- URI: https://iisg.amsterdam/id/recordresource/ARCH00860.A_57#date01


