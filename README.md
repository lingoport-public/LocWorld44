# LocWorld44
We created this repository as an illustration of resource files, either in standard or in suboptimal forms, based on a number of applications we've been exposed to. The way resource files are created affect both  software development and localization processes. This repository will be part of LocWorld44 and can be used to illustrate some common issues with resource files.

## resource files
Resource files are part of an application code. They contain user facing strings, from UI labels and menus to email and report strings. Resource files are written by developers in a language, say US English, and sent for translation in target locales, such as French, Spanish, Japanese, Chinese, or Korean.

Resource files should be easy to identify, both in terms of which files to translate and which files were translated. They should also contain key value pairs so that the application references a key and a locale to get the corresponding value, or string, in that locale. 

## standard file formats
The <code>standard</code> directory shows illustrative examples of standard resource file formats. Programming languages have mature libraries and components for standard files, from the basic reading and displaying strings, to parameters passing and fallback locales. 

Standard file formats can be used in a variety of downstream processes and products, from <b>Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/)</b> to <b>[Localyzer Express](https://lingoport.com/software-internationalization-products/express-suite/)</b> and <b>[LocalyzerQA](https://lingoport.com/software-internationalization-products/localyzerqa-linguistic-qa/)</b> to TMS's or even pure Machine Translation engines. In the <coce>standard</code> directory, we show a few simple example of standard files well understood by the industry ecosystem.

## non standard file formats
For developers with little knowledge of i18n and L10n, creating and reading from a special file format may look like a good idea. However, non standard file formats usage tends to be short-sighted. It prevents the L10n ecosystem from working with them out of the box. 

The <code>nonstandard</code> directory shows a few illustrative examples of some non-standard file types. 

## recommendation
We strongly recommend using standard file formats whenever possible for a better overall software localization.

## Localyzer
In the case of <b>Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/)</b> automation, the transform framework  allows non standard files to be transformed into temporary standard files for L10n purposes and still keep the non standard file formats for the application and its repository. And Localyzer handles standard file formats with validation, notification, automation back and forth TMS's or pure MT. 
 
