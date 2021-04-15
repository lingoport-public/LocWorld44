# The format
The format in this real life example is close to that of .properties files. Properties files are well understood by lots of systems, whereas .txt files can take many forms. 

Instead of <code>strings.txt</code> (and <code>strings-fr.txt</code>, etc.)

    #################################################
    # Strings for use in GUI
    #################################################
    CloseButtonText,Close
    ApplyButtonText,Apply

<code>strings.properties</code> (and <code>strings_fr.properties</code>, etc.)could have been used

    #################################################
    # Strings for use in GUI
    #################################################
    CloseButtonText=Close
    ApplyButtonText=Apply

## Localyzer Note
With Localyzer, the transform framework is used to move files to .properties so the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
