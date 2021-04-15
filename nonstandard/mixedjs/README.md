## The non standard format
The format in this real life example is close to that of .json files. 
* JSON files are well understood by lots of systems, whereas .js files can take many forms and should be used for programming, not localization data. 
* JSON files do not have comments as opposed to .js files
* .js 'code' (here the very simple <code>export default {</code> for instance) should not be 'translated'
* This file mixes a number of elements, all of which should not be sent for translation:
* * audio file names
* * video file names
* * menu/submenu indices
* * other non translatable attributes

Instead of the non-standard <code>content.js</code> (and <code>french.js</code>, etc.)

    export default {
       "audio": {
        "section03": "media/audio/02.mp3"
      },
      "menu_sections": {
        "enabled": true,
        "sections": [
          {
            "range": [
              4,
              19
            ],
            "title": "Lesson 1: Leading in the Workforce"
          },
         [...]
      },
      "submenunum": 1,
      "submenupages": [
        12,
        16,
        21,
        27,
        30
      ],
      "video": {
        "video01": "<video id=\"player1\" data-video-id=\"4097463356001\" data-account=\"936125986001\" data-player=\"SkzcaSONl\" data-embed=\"default\" class=\"video-js\" controls autoStart=false style=\"width: 100%; height: 100%; position: absolute; top: 0px; bottom: 0px; right: 0px; left: 0px;\"></video>",
        "video01url": "///936125986001/SkzcaSONl_default/index.min.js",
        [...]
      }
    };



a standard file purely for translation should be created separately from the other attributes, such as <code>messages_en.json</code>  

    {
      "title.lesson1": "Lesson 1: Leading in the Workforce",
      "title.lesson2": "Lesson 2: Building Capability",
      "title.lesson3": "Lesson 3: Leading Performance",
     
with the ability for the code to reconcile the title.lesson<b>n</b> with other attributes in another file or set of files.

