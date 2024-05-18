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

## PEOPLE

Named people (both explicit and implicit, e.g. by honorific) are identified with `<persName>` tag once in each of the records in a record set.

People who have a REED identifier are tagged with that identifier (if there is also a Wikidata identifier, this will connect that information.)

People should have a REED identifier with the following conditions:

1. They are identified by at least a last name (can be variant spelled)
2. They have at least one life date (the date of the record counts as a 'floruit date')
3. They are referred to in the body of a record (not in REED edition editorial or documentary apparatus)

## PLACES

REED London has captured over 400 place names /link/ and disambiguated them against the Map of Early Modern London and Wikidata URIs. Named places are identified with `<placeName>` tag once in each of the records in a record set.

## ORGANIZATIONS

REED London has created identifiers for all XX worshipful companies in London that were active during the scoped period (e.g. 1300-1650).LINK

Named organizations are captured in the titles of record sets as well as once in contextual references in each of the records in a record set.

## OCCUPATIONS

REED London has resolved occupation types against the LINCS vocabularies. Occupations are captured as roles associated with named persons. 

## TRANSLATIONS

Because LEAF allows us to capture translations in a subsequent div, use that function in LEAF-Writer to capture translations. However, default div should be the English language version, even if that is a modern version of the original Latin or other language.

## EVENTS

Because REED London is particularly interested in events that were associated in some way with performance (and vice versa) we are using the `<eventName>` tag to capture information about *known* events, and capturing types of events, such that:

1. holy day (e.g., Saint's Day)
2. royal (any event that involves a monarch or member of the royal family)
3. municipal (any event that involves the political life of the City, e.g., a mayoral pageant or oath)
4. guild (any event at which a guild gathers)
5. calendar (any event by which Londoners understood the year, e.g., May Day, Twelfth Night, Christmas time, etc.)