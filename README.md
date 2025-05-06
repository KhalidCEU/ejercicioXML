## Ejercicio XML (DTD)

[Enlace](https://www.truugo.com/xml_validator/) hacia validador (**poner el DTD (entre la linea ```<xml>``` y el comienzo del XML)**)


### Ejercicio 1

> Crea un **XML** que sea **válido** para el siguiente **DTD**:

```
<!DOCTYPE TVSCHEDULE [
<!ELEMENT TVSCHEDULE (CHANNEL+)>
<!ELEMENT CHANNEL (BANNER,DAY+)>
<!ELEMENT BANNER (#PCDATA)>
<!ELEMENT DAY (DATE,(HOLIDAY|PROGRAMSLOT+)+)>
<!ELEMENT HOLIDAY (#PCDATA)>
<!ELEMENT DATE (#PCDATA)>
<!ELEMENT PROGRAMSLOT (TIME,TITLE,DESCRIPTION?)>
<!ELEMENT TIME (#PCDATA)>
<!ELEMENT TITLE (#PCDATA)>
<!ELEMENT DESCRIPTION (#PCDATA)>
<!ATTLIST TVSCHEDULE NAME CDATA #REQUIRED>
<!ATTLIST CHANNEL CHAN CDATA #REQUIRED>
<!ATTLIST PROGRAMSLOT VTR CDATA #IMPLIED>
<!ATTLIST TITLE RATING CDATA #IMPLIED>
<!ATTLIST TITLE LANGUAGE CDATA #IMPLIED>
]>
```

**R**: Fichero [XML](/xml.xml)



### Ejercicio 2

> Crea un **DTD** que valide el siguiente **XML**:

```
<articles>
<article id="x34675">
<name>Apache Spark Architecture</name>
<month>december</month>
<author name="kay vennisla"/>
<reviews lang=""/>
<feedback > high rating</feedback>
<reviews lang="de">The best content with diagrams</reviews>
</article>
</articles>
```


**R**: Fichero [DTD](/dtd.xml)