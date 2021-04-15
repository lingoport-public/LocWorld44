## The non standard directory structure
Here the files are standard and well-formed. However, the source and target locales do not follow the same pattern

Instead of the non-standard <code>directory structure</code> 

    .../resources/source/en.json
    .../resources/es.json
    .../resources/fr.json


a standard directory structure could have been used

    .../resources/en.json
    .../resources/es.json
    .../resources/fr.json

## Localyzer Note
With Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/), the transform framework is used to move the <code>.../resources/source/en.json</code> type files to <code>.../resources/en.json</code> and the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
And it does not change the way the files are in the repository. 
