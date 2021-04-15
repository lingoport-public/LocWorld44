## The non standard format
.txt files tend to be used for free form text. 
Here, the .txt file has a unique structure that looks like a possible extract from a database for the purpose of localization. 
However, instead of generating a simple key/value type file, like say properties, the format makes it difficult to be used by most systems. 

Instead of the non-standard <code>evtypes.txt</code> (and <code>evtypes_ar.txt</code>, etc.)

    DN: cn=1,ou=evtypes,dc=plasec
    plasecName: Tamper

    DN: cn=2,ou=evtypes,dc=plasec
    plasecName: Power

A  more standard format such as <code>evtypes.properties</code> (and <code>evtypes_ar.properties</code>, etc.) could have been used

    cn1=Tamper
    cn2=Power

## Localyzer Note
With Localyzer, the transform framework is used to move <code>evtypes.txt</code> type files to a simple key value based <code>evtypes.properties</code> so the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
