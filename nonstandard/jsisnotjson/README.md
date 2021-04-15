## The non standard format
The format in this real life example is close to that of .json files. 
* JSON files are well understood by lots of systems, whereas .js files can take many forms and should be used for programming, not localization data. 
* the locale for a source or a translated file should use the ISO form
* the locale should be only indicated in the file name
* JSON files do not have comments as opposed to .js files
* .js directives (here the very simple <code>export const english = {</code> for instance) should not be 'translated'

Instead of the non-standard <code>english.js</code> (and <code>french.js</code>, etc.)

    // To be translated
    //
    export const english = {
      // #
      "2D": "2D",
      "3D": "3D",


a standard file such as <code>messages_en.json</code>  (and <code>messages_fr.json</code>, etc.) could have been used

    {
      "2D": "2D",
      "3D": "3D",

## Localyzer Note
With Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/), the transform framework is used to move <code>english.js</code> type files to <code>messages_en.json</code> so the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
