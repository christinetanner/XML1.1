XML1.1
======

XML class


<?xml version="1.0" encoding="utf-8"?>
<!--Created by Christine Tanner 10-12-12 Activity 2-1 FileName: RealEstate.dtd-->
<!ELEMENT ResidentialProperty (Listing*)>
	<!ELEMENT Listing (StreetAddress, ListingPrice, LivingArea, Memo?, AgentDescription+)>
		<!ELEMENT StreetAddress (StreetNumber, StreetName, City, State, Zip)>
			<!ELEMENT StreetNumber (#PCDATA)>
			<!ELEMENT StreetName (#PCDATA)>
			<!ELEMENT City (#PCDATA)>
			<!ELEMENT State (#PCDATA)>
			<!ELEMENT Zip (#PCDATA)>
		<!ELEMENT ListingPrice (#PCDATA)>
		<!ELEMENT LivingArea (#PCDATA)>
		<!ELEMENT PricePaid (#PCDATA)>
		<!ELEMENT Memo (#PCDATA)>
		<!ELEMENT AgentDescription (#PCDATA | HomeType)*>
			<!ELEMENT HomeType (#PCDATA)>
		<!ATTLIST ListingPrice CurrencyCode CDATA #REQUIRED>
		<!ATTLIST LivingArea Units CDATA #REQUIRED>
		<!ATTLIST PricePaid CurrencyCode CDATA #REQUIRED>




<?xml version="1.0" encoding="UTF-8"?>
<!--Updated by Christine Tanner 10-12-12 FileName: Brown County Properties.xml-->
<!DOCTYPE ResidentialProperty SYSTEM "RealEstate.dtd"><!--looking for where is validates the structure-->
<!-- BROWN COUNTY PROPERTIES -->
<ResidentialProperty>
<Listing>
<StreetAddress>
<StreetNumber>100</StreetNumber>
<StreetName>Street Name</StreetName><!--Teresa found this line was missing-->
<City>Rochester</City>
<State>New York</State>
<Zip>14699</Zip>
</StreetAddress>
<ListingPrice CurrencyCode="USD">250000</ListingPrice>
<LivingArea Units="SqFeet">3000</LivingArea>
<AgentDescription>
<HomeType>Federal </HomeType>style house with large 3 story barn, and a second guest house</AgentDescription>
<AgentDescription>
<HomeType>Federal </HomeType>style house with barn and guest house</AgentDescription>
</Listing>
<Listing>
<StreetAddress>
<StreetNumber>200</StreetNumber>
<StreetName>Pear Street</StreetName>
<City>Rochester</City>
<State>New York</State>
<Zip>14699</Zip>
</StreetAddress>
<ListingPrice CurrencyCode="USD">150000</ListingPrice>
<LivingArea Units="SqFeet">2500</LivingArea>
<Memo><![CDATA[One of the oldest frame dwellings in upstate New York. Built 1863 by John Smith III during the Civil war.]]></Memo>
<AgentDescription>
<HomeType>Colonial</HomeType> style home in a beautiful neighborhood of other historic <HomeType>colonials</HomeType>
</AgentDescription>
</Listing>
<Listing>
<StreetAddress>
<StreetNumber>300</StreetNumber>
<StreetName>Apple Grove Lane</StreetName>
<City>Rochester</City>
<State>New York</State>
<Zip>14699</Zip>
</StreetAddress>
<ListingPrice CurrencyCode="USD">190000</ListingPrice>
<LivingArea Units="SqFeet">2000</LivingArea>
<Memo><![CDATA[Situated in upstate NY, a comfortable home on a 9 acre tract, set back 105' from the shaded tree lined street.]]></Memo>
<AgentDescription>Elegant Italiante <HomeType>Victorian</HomeType> style home.</AgentDescription>
</Listing>
<Listing>
<StreetAddress>
<StreetNumber>400</StreetNumber>
<StreetName>Plum Street</StreetName>
<City>Rochester</City>
<State>New York</State>
<Zip>14699</Zip>
</StreetAddress>
<ListingPrice CurrencyCode="USD">205000</ListingPrice>
<LivingArea Units="SqFeet">2600</LivingArea>
<AgentDescription>
Gigantic <HomeType>ranch</HomeType> out in a lovely forest environment.</AgentDescription>
<AgentDescription>
Enormous <HomeType>ranch</HomeType> sprawling out in a secluded wooded setting.</AgentDescription>
</Listing>
<Listing>
<StreetAddress>
<StreetNumber>500</StreetNumber>
<StreetName>Canteloupe Way</StreetName>
<City>Rochester</City>
<State>New York</State>
<Zip>14699</Zip>
</StreetAddress>
<ListingPrice CurrencyCode="USD">245000</ListingPrice>
<LivingArea Units="SqFeet">2800</LivingArea>
<Memo><![CDATA[Cosmopolitan living in a country setting best describes this impeccable home.]]></Memo>
<AgentDescription>
Brand new design! Modernized <HomeType>contemporary</HomeType> home designed for the high end customer in a middle class area.</AgentDescription>
</Listing>
<Listing>
<StreetAddress>
<StreetNumber>600</StreetNumber>
<StreetName>Plum Lane</StreetName>
<City>Rochester</City>
<State>New York</State>
<Zip>14699</Zip>
</StreetAddress>
<ListingPrice CurrencyCode="USD">300000</ListingPrice>
<LivingArea Units="SqFeet">3500</LivingArea>
<Memo><![CDATA[3378 Sq Ft Cape Cod Revival, Large combo Kitchen & Dining Room with fireplace and woodmode cherry cabinets, ceramic tile floor. Beautiful views overlooking the valley.]]></Memo>
<AgentDescription>
Brand new design! Modernized <HomeType>contemporary</HomeType> home designed for the high end customer in a middle class area.</AgentDescription>
<AgentDescription>
New and beautifully modernized <HomeType>contemporary</HomeType> home designed for the future.</AgentDescription>
</Listing>
</ResidentialProperty>










