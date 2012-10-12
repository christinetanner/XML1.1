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
