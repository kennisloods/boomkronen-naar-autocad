# Boomkronen naar AutoCAD
Vertaalt boomkronen in GIS-formaat naar AutoCAD DWG-formaat.

## toelichting

R&W verwerkt vaak Boomgegevens uit de BOR in AutoCAD. Hiervoor worden vaak de boomgegevens uit ESRI Shape-formaat vertaald naar Autocad DWG-formaat.

Dit script helpt om deze vertaling van te voren, in bulk uit te voeren.

 
## productformaten

Dit script levert geen standaardproducten op. Het uitvoerformaat is AutoCAD DWG.

 
## bronnen

* boomgegevens uit de BOR: `K:\GEODATA\Themadata\BOR\Data\SHP\Bomen_punten.shp`.

 
## werking van het script

De command line aanroep is:
```
"C:\Program Files (x86)\FME\fme.exe" K:\GEODATA\Kennisloods\Tools\Boomkronen_Autocad\Boomkronen_naar_Autocad.fmw
--P_BRON_BOR_SHP "K:\GEODATA\Themadata\BOR\Data\SHP\Bomen_punten.shp"
--P_DOEL_ACAD "K:\SO\RW\Autocad\Projecten\Algemeen\Bomen_Boomkroongroottes_20181107.dwg"
--P_TEMPLATE "K:\GEODATA\Kennisloods\Tools\Boomkronen_Autocad\Boom.dwg"
--P_LOG "K:\GEODATA\Kennisloods\Tools\VanLasnaarTekst\log\Boomkronen_naar_AutoCAD.log"
```
 
De betekenis van de parameters is:

| parameter        | betekenis                                                   |
| ---------------- | ----------------------------------------------------------- |
| `P_BRON_BOR_SHP` | Locatie van het te vertalen bomenbestand.                   |
| `P_DOEL_ACAD` 	 | Naam van het bestand waarin het resultaat wordt uitgevoerd. |
| `P_TEMPLATE` 	   | Locatie van het sjabloonbestand voor AutoCAD.               |
| `P_LOG` 	       | Locatie van het logbestand.                                 |
