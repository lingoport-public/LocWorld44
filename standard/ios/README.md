## iOS
When writing an iOS application, the standard file format follows Localizable.string type format located in standard directories:
https://developer.apple.com/library/archive/documentation/MacOSX/Conceptual/BPInternational/MaintaingYourOwnStringsFiles/MaintaingYourOwnStringsFiles.html

The base source files (say US English written by developers) will reside under a <code>Base.lproj</code> directory.
The translated resource files (say the French translation) will reside under a <code>[localecode].lproj</code>, for example <code>ja.lproj</code>.

The Localizable.string type file itself will follow the iOS form and the file will look like:

    /* Class = "NSTableColumn"; headerCell.title = "Location"; ObjectID = "f0Y-kT-hVz"; */
    "f0Y-kT-hVz.headerCell.title" = "Location";
 
    /* Class = "NSTextFieldCell"; title = "Address:"; ObjectID = "gfa-oA-9cr"; */
    "gfa-oA-9cr.title" = "Address:";
 
    /* Class = "NSTextFieldCell"; title = "for:"; ObjectID = "gsV-Sg-yiA"; */
    "gsV-Sg-yiA.title" = "for:";
    
with or without the /* comments */ 

When following these iOS guidelines, development and translation will be able to leverage the localization ecosystem. 

### LocalyzerExpress
For example, one can add the [LocalyzerExpress](https://github.com/marketplace/localyzer-express) GitHub marketplace application go automatically have the source files always translated in the target locales of interest right away.
See: https://lingoport.com/software-internationalization-products/express-suite/ 

### Localyzer
For more complex repositories, one can use [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/) to automate the translation with LSP's, TMS's, etc.

### LocalyzerQA
Once files are translate with [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/) or [LocalyzerExpress](https://github.com/marketplace/localyzer-express), 
linguistic reviewers can check the translations in the running application using [LocalyzerQA](https://localyzerqa.lingoport.io/localyzerqa). 
See: https://lingoport.com/software-internationalization-products/localyzerqa-linguistic-qa/ 
