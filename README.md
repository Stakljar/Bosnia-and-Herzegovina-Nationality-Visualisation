# Bosnia-and-Herzegovina-nationality-visualisation
The boundary data provided in this repository are released under the Open Database License (ODbL): [https://opendatacommons.org/licenses/odbl/1-0/](https://opendatacommons.org/licenses/odbl/1-0/).<br>
The following modifications were made to the original file, which was acquired at [geoboundaries.org](https://www.geoboundaries.org/):
- Renamed property name "BIHADM2gbOpen" to "municipalities".
- Modified object which is the value of property "properties" for each "properties" property like this:
	removed "shapeGroup", "shapeId", "shapeISO" and "shapeType" properties,
	renamed property "shapeName" to "name" and added properties "population2013" and "population1991".<br>
	Values of these new properties are objects containing properties: "overall", "serbs", "bosniaks" and "croats",
	values of which are numbers of overall population and population of each major nation inside Bosnia and Herzegovina in years 2013. and 1991. across municipality/city.<br>
	Data about overall population and population of each major nation in years 1991. and 2013. for each municipality/city
	inside Bosnia and Herzegovina are licensed under Creative Commons Attribution-ShareAlike International License (CC BY-SA): [https://creativecommons.org/licenses/by-sa/4.0/deed.en](https://creativecommons.org/licenses/by-sa/4.0/deed.en).<br>
 	These data were acquired from: [bs.wikipedia.org/wiki/Op%C4%87ine_Bosne_i_Hercegovine](https://bs.wikipedia.org/wiki/Op%C4%87ine_Bosne_i_Hercegovine).
- Added "total" property inside object which is the value of property "municipalities".<br>
	Value of "total" property is object also containing properties "population2013" and "population1991".<br>
	Values of these properties are objects also containing properties "overall", "serbs", "bosniaks" and "croats",
	values of which represent numbers of overall population and population of each major nation inside Bosnia and Herzegovina in years 2013. and 1991. across the whole country.<br>
	These values were calculated by summing values of "overall", "serbs", "bosniaks" or "croats" property
	from corresponding "population2013" or "population1991" property from "properties" property for each "properties" property.<br>
- Changed values for the following "name" properties like this:
	"Bihac" renamed to "Bihać",
	"Centar" renamed to Centar (Sarajevo)",
	"Mrkonjic Grad" renamed to "Mrkonjić Grad",
	"Novi Grad" renamed to "Novi Grad (Sarajevo)".