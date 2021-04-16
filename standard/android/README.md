## Android
When writing an Android application, the standard file format is strings.xml located in standard directories:
https://developer.android.com/guide/topics/resources/string-resource#FormattingAndStyling 

The base source files (say US English written by developers) will reside under a <code>res/values</code> directory.
The translated resource files (say the French translation) will reside under a <code>res/values-[localecode]</code>, for example <code>res/values-fr</code>.

The strings.xml file itself will follow the Android schema for strings and the file will look like:

    <?xml version="1.0" encoding="utf-8"?>
    <resources xmlns:tools="http://schemas.android.com/tools" tools:ignore="UnusedResources">
      <string name="action_cancelled">Action Canceled</string>
      <string name="no_internet_title">No Internet Connection</string>
      <string name="internet_disconnect_try_again">This action cannot be completed. Please check your connection, and try again.</string>
      <string name="ok">OK</string>
      <string name="cancel">Cancel</string>
    </resources>
    
When following these Android guidelines, development and translation will be able to leverage the ecosystem. 

## LocalyzerExpress
For example, one can add the [LocalyzerExpress](https://github.com/marketplace/localyzer-express) GitHub marketplace application go automatically have the source files always translated in the target locales of interest right away.
See: https://lingoport.com/software-internationalization-products/express-suite/ 

## Localyzer
For more complex repositories, one can use [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/) to automate the translation with LSP's, TMS's, etc.

## LocalyzerQA
Once files are translate with [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/) or [LocalyzerExpress](https://github.com/marketplace/localyzer-express), 
linguistic reviewers can check the translations in the running application using [LocalyzerQA](https://localyzerqa.lingoport.io/localyzerqa). 
See: https://lingoport.com/software-internationalization-products/localyzerqa-linguistic-qa/ 
