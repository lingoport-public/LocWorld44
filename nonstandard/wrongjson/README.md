## The less than optimal usage of .json files.
This json file is an array with the identifier as a value instead of a key. 
The translator should not be changing the "id" string value (for instance "upgrade") and depending on the content of the file, it may be difficult to know.

Instead of the non-standard <code>en.json</code> (and <code>bg.json</code>, etc.)

    [
        {
            "id": "0",
            "text": "The game is currently not available. Try again later."
        },
        {
            "id": "10",
            "text": "There is not enough money in your account."
        },
     [...]
        {
            "id": "upgrade",
            "text": "Please upgrade {0} in {1}."
        }
    ]


a simpler and better file could have been used

    {
      "id.0": "The game is currently not available. Try again later.",
      "id.10": "There is not enough money in your account.",
      [...]
      "upgrade": "Please upgrade {0} in {1}."
    }

## Localyzer Note
With Lingoport [Localyzer](https://lingoport.com/software-internationalization-products/localyzer-localization-automation/), the transform framework is used to change <code>en.json</code> type files to a simpler <code>message_en.json</code> and the system (automation, verification, dashboard, TMS or MT, etc.) works smoothly.
And it does not change the way the files are in the repository.
