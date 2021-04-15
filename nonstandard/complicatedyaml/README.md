## The non standard format
The yaml/yml files in this directory look more like an XML structure than a standard localization yaml/yml file with simple key value pairs. 
Instead of the non-standard <code>en.yaml</code> (and <code>fr.yaml</code>, etc.)

    - key: barcelona_too_many_tags
      translation:
        msg: "A Managed Object cannot have more than %d tags"
    - key: barcelona_invalid_tag_prefix
      translation:
        msg: "The tag key cannot start with the reserved prefix '%s'"

the more standard <code>message_en.yaml</code> (and <code>messages_fr.yaml</code>, etc.) could have been used

    barcelona_too_many_tags: "A Managed Object cannot have more than %d tags"
    barcelona_invalid_tag_prefix: "The tag key cannot start with the reserved prefix '%s'"

## Localyzer Note
With Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/), the transform framework is used to move <code>en.yaml</code> type files to a simple key value based <code>en.yml</code> so the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
