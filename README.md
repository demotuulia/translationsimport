# Python translations import

## Contents

* [Introduction](#intro-section)
* [Files](#files-section)

<a name='intro-section'></a>

## Introduction

This is a small translation import tool made by the Python programming language.
To see how to use it look at the document TranslatorsGuide.pdf.

You can add an edit translations by importing the in spread sheets, which can be sent
to professional translators. After their job is done, you can import the translations back in
spreadsheets.  This application converts the spread sheets to json files, which can be read for example by a front end javascript application.

Example of a spread sheet tranlations fromt English to Dutch:

```
Key,English,Translation (NL_NL)
menu.about;about;about
menu.locale;EN;EN
menu.country;Ireland;Ireland
button.tellmemore;Tell me more;Tell me more
button.readmore.less;less;less
button.readmore.more;more;more
page.fallback.header;This website provides EU `opt--out’ from the EHDS
page.fallback.intro;Ourpean Health Data Space <red>"Select Country"</red>
page.about.title;About;About
page.about.h;I am am h1;I am am h1
page.about.p;h1 p1 text;h1 p1 text
page.about.p;h1 p2 text;h1 p2 text
page.about.h;I am a h2;I am a h2
page.about.p;h2 p1  text;h2 p1  text
page.about.p;h2 p2  text;h2 p2  text
page.about.p;h2 p3  text;h2 p3  text
page.about.h;I am a h3;I am a h3
```

Example of english json : en_GB.json

```
    {
        "pageTitle": "Compose Your Letter",
        "previous": "Previous",
        "next": "Next",
        "step1": {
            "title": "Name and Address",
            "properties": {
                "name": {
                    "title": "Full Name"
                },
            "address": {
                "title": "Address"
                }
            }
        }
    }

```

<a name='files-section'></a>

## Files



| Folder | Description |
| ------ | ----------- | 
|   lib     |    Python classes         |      
|   src/csv/languages/import     | Folder to import translations in CSV format             |      
|   src/csv/languages/export     | Folder for exported translations in CSV format from the JSON files, these can be re-imported with modifications              |  
|   src/languages/     | Json files converted from the imported CSV files      |  