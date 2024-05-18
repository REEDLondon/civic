# Editorial Decisions

Information pertains to Civic 2.0 documents published on REED London

## Record structure in TEI

Recommendations for records in Worshipful Companies collection

1. Record filess are published by company, by particular record type, and by year or year range
2. Records are published in _draft_ format
3. something

Structure of record file in TEI

```tei
 <div type="record_set">
    <head>
<title>[title from transcription]</head></title>
    <bibl>LMA #</bibl>
       <div type="record">
       <head><supplied>[information supplied from transcription]</supplied></head>
       <pb/>
       <gap/>
       <ab>[body of text]</ab>
       </div>
</div>
```

Add as many record gobbets as needed

NOTES: Because LEAF allows us to capture notes at the point of insertion, there is no need to use endnotes at the bottom of the text.

TRANSLATIONS: Because LEAF allows us to capture translations in a subsequent div, use that function in LEAF-Writer to capture translations. However, default div should be the English language version, even if that is a modern version of the original Latin or other language.
