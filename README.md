<pre>
The boundary data provided in this repository are released under the ODbL license.
The following modifications were made to the original file, which was acquired at geoboundaries.org:
- Renamed property name "BIHADM2gbOpen" to "municipalities".
- Modified object which is the value of property "properties" for each "properties" property like this:
	removed "shapeGroup", "shapeId", "shapeISO" and "shapeType" properties,
	renamed property "shapeName" to "name" and added properties "population2013" and "population1991".
	Values of these new properties are objects containing properties: "overall", "serbs", "bosniaks" and "croats",
	values of which are numbers of overall population and population of each major nation inside Bosnia and Herzegovina in years 2013. and 1991. across municipality/city.
	Data about overall population and population of each major nation in years 1991. and 2013. for each municipality/city
	inside Bosnia and Herzegovina was used from: <a href="https://bs.wikipedia.org/wiki/Op%C4%87ine_Bosne_i_Hercegovine">bs.wikipedia.org/wiki/Op%C4%87ine_Bosne_i_Hercegovine</a>.
- Added "total" property inside object which is the value of property "municipalities".
	Value of "total" property is object also containing properties "population2013" and "population1991".
	Values of these properties are objects also containing properties "overall", "serbs", "bosniaks" and "croats",
	values of which represent numbers of overall population and population of each major nation inside Bosnia and Herzegovina in years 2013. and 1991. across the whole country.
	These values were calculated by summing values of "overall", "serbs", "bosniaks" or "croats" property
	from corresponding "population2013" or "population1991" property from "properties" property for each "properties" property.
- Changed values for the following "name" properties like this:
	"Bihac" renamed to "Bihać",
	"Centar" renamed to Centar (Sarajevo)",
	"Mrkonjic Grad" renamed to "Mrkonjić Grad",
	"Novi Grad" renamed to "Novi Grad (Sarajevo)".
</pre>
