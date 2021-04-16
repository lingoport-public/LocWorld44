## resx files
Microsoft based programming tends to use resx files. These are very common resource file types.
See: https://docs.microsoft.com/en-us/aspnet/core/fundamentals/localization?view=aspnetcore-5.0#resource-files-2

### naming
The locale is most commonly indicated in the file name itself. such as <code>messages.ko.resx</code>. 
A file name without a locale is construed as the source file or the default locale file, for example <code>messages.resx</code>.

### structure
resx files follow an XML schema. The _bottom_ of the file contains the actual user facing strings. The entire file tends to have more overhead information at the top of the file.

 
    <data name="WarningThisAccountGroupNameAlreadyExistsWithDifferentSortOrders" xml:space="preserve">
      <value>This [Account] Group Name already exists in the table more than once with different sort orders, the sort orders will be set to {0} to be consistent.</value>
      <comment>Sort level</comment>
    </data>
    <data name="WarningThisSummaryAccountGroupNameAlreadyExistsWithDifferentSortOrders" xml:space="preserve">
      <value>This Summary [Account] Group Name already exists in the table more than once with different sort orders, the sort orders will be set to {0} to be consistent.</value>
      <comment>Sort level</comment>
    </data>
    <data name="ErrorAccountDoesNotExist" xml:space="preserve">
      <value>[Account] {0} does not exist.</value>
      <comment>{0} - Account id</comment>
    </data>
    
When following these guidelines, development and translation will be able to leverage the localization ecosystem. 

### LocalyzerExpress
For example, one can add the [LocalyzerExpress](https://github.com/marketplace/localyzer-express) GitHub marketplace application go automatically have the source files always translated in the target locales of interest right away.
See: https://lingoport.com/software-internationalization-products/express-suite/ 

### Localyzer
For more complex repositories, one can use [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/) to automate the translation with LSP's, TMS's, etc.

### LocalyzerQA
Once files are translate with [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/) or [LocalyzerExpress](https://github.com/marketplace/localyzer-express), 
linguistic reviewers can check the translations in the running application using [LocalyzerQA](https://localyzerqa.lingoport.io/localyzerqa). 
See: https://lingoport.com/software-internationalization-products/localyzerqa-linguistic-qa/ 
