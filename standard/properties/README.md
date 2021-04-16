## properties files
Properties files are one of the most used resource file format for localization. For example, when developing a Java application, it should be the standard file format. 
See: https://docs.oracle.com/javase/tutorial/i18n/intro/steps.html

### naming and context
The source files (written by developers and to be translated) are simple key/value pairs in a file typically without a locale, such as <code>messages.properties</code>:

    greetings = Hello
    farewell = Goodbye
    inquiry = How are you?
    
The corresponding translated file simply needs the locale, such as <code>messages_fr.properties</code> for the French translation.

    greetings = Bonjour.
    farewell = Au revoir.
    inquiry = Comment allez-vous?
    
 When following these properties (Java and other programming languages) guidelines, development and translation will be able to leverage the localization ecosystem. 

### LocalyzerExpress
For example, one can add the [LocalyzerExpress](https://github.com/marketplace/localyzer-express) GitHub marketplace application go automatically have the source files always translated in the target locales of interest right away.
See: https://lingoport.com/software-internationalization-products/express-suite/ 

### Localyzer
For more complex repositories, one can use [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/) to automate the translation with LSP's, TMS's, etc.

### LocalyzerQA
Once files are translate with [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/) or [LocalyzerExpress](https://github.com/marketplace/localyzer-express), 
linguistic reviewers can check the translations in the running application using [LocalyzerQA](https://localyzerqa.lingoport.io/localyzerqa). 
See: https://lingoport.com/software-internationalization-products/localyzerqa-linguistic-qa/ 
