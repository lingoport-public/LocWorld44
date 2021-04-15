## The non standard format
LOC files: 
* LOC files are not understood or supported by most localization systems
* The comments with English in the file does not add anything, the directory name already has the language code.

Instead of the non-standard <code>en/HYC.LOC</code> (and <code>de/HYC.LOC</code>, etc.)

    ;	English
    ; *************************************************************************
    ;
    1	Info: Cannot open: %s
    2	Info: Memory allocation not possible
    7	Info: Cannot find %s


a standard file such as <code>hyc.properties</code>  (and <code>hyc_de.properties</code>, etc.) could have been used


    # *************************************************************************
    #
    key1=Info: Cannot open: %s
    key2=Info: Memory allocation not possible
    key7=Info: Cannot find %s

## Localyzer Note
With Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/), the transform framework is used to move <code>en/HYC.LOC</code> type files to <code>en/HYC.properties</code> and the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
