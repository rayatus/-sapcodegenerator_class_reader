[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/rayatus/sapcodegenerator_class_reader/blob/master/LICENSE)
![ABAP 7.40sp08+](https://img.shields.io/badge/ABAP-7.40sp08+-brightgreen)
[![Code Statistics](https://img.shields.io/badge/CodeStatistics-abaplint-blue)](https://abaplint.app/stats/rayatus/sapcodegenerator_class_reader)

# SAPCodeGenerator : DB Class Reader
This generator creates a class reader where generic methods for retrieving data from a specific DB are generated.

By executing transaction **ZDBFRAMEWORK_WIZARD** a wizard will be showned asking for:
* DataBase table for which the class reader will be generated.
* Also a dictionary table type which will be used as exporting parameter in the corresponding method for returning several rows. 
* ClassName for the ABAP class which is going to be created. By default it will be "ZCL_< DBTableName >_READ"
* Package where to save the generated ABAP class

For testing purposes you could execute it by using:
* DataBase table > SFLIGHT
* Table Type > ZTT_SFLIGHT (already provided by this repo)


Requieres **sapcodegenerator_base** repository (https://github.com/rayatus/sapcodegenerator_base)
