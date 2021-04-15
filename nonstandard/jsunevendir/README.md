## The non standard format
The format in this real life example is close to that of .json files. 
* JSON files are well understood by lots of systems, whereas .js files can take many forms and should be used for programming, not localization data. 
* the source locale are not under the peer directory (here 'en') to the target locales (ja, ko, zh) 
* the locale target should be not be part of the source locale 
* JSON files do not have comments as opposed to .js files
* .js directives (here the very simple <code>define({</code> for instance) should not be 'translated'

Instead of the non-standard <code>i18n_general.js</code> (and <code>ja/i18n_general.js</code>, etc.)

    /* eslint no-undef: 1 */
    define({
      root: {
        loading: 'Loading',

        // Common Strings
        understand: 'Understand',


a standard file such as <code>en/i18n_general.json</code>  (and <code>ja/i18n_general.json</code>, etc.) could have been used

    {
      "loading": "Loading",
      "understand": "Understand",

## Localyzer Note
With Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/), the transform framework is used to move <code>i18n_general.js</code> type files to <code>en/i18n_general.json</code> and the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
