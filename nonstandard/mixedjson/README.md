## The format
The JSON files mix some attributes which should not be translated and segments which should be. 
This file can actually be sent for translation and the systems will work fine, provided the TMS filters are set up or the translators are coached to make sure the attributes are not modified.
Better would be to have one file purely for translation purposes, and another file (or more) for non translatable attributes. 

Instead of the current <code>en/license.json</code> (and <code>ko/license.json</code>, etc.)

      "issueDescription": {
        "messages": {
          "onprem": "This WLC \"{wlcName}\" is currently licensed to support {maxCount} AP(s) and currently has {inUseCount} AP(s). If this trend continues, this WLC will exhaust all its AP license(s)."
       },
      "attributes": {
         "00000_LRMARRCONV": {
            "params": {
              "00000_LRMARRCONV": "wlcName",



a better and simple file, purely for translation, could have been used


   {
     "license.onprem": "This WLC \"{wlcName}\" is currently licensed to support {maxCount} AP(s) and currently has {inUseCount} AP(s). If this trend continues, this WLC will exhaust all its AP license(s).",
     "license.suggestion": Purchase and install additional AP adder licenses."
   }

## Localyzer Note
With Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/), the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
It is up to the TMS or the translation team to make sure things work well. And they may not.
