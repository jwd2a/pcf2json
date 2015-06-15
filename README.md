#PCF Parser

This script takes a .csv representation of the PCF and creates a nested JSON object out of it.

##Usage

- Clone this repo or download `pcf2json.js`
- Run `npm install` to install local dependencies
- Once installed, run `node ../path/to/pcf2json.js NameOfFile.xlsx`
- The result will be a file called `framework.json` in the same directory you ran the script, with all your juicy PCF goodness.

##Caveats

This script is pretty particular about how the Excel document is formatted. If you're using the official APQC frameworks, you shouldn't have a problem. If something blows up, it's likely because of the formatting.

Files should follow the format shown here: [APQC Retail Framework](https://www.apqc.org/knowledge-base/documents/apqc-process-classification-framework-pcf-retail-pcf-excel-version-600-0)


##TODO

- Package as an NPM module so you can run it globally without requiring the path. Will need to manually link for now if you want to do that.
- Create a way to name the framework and provide a description for it
- Create a way to specify the filename generated by the script
