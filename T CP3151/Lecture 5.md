# XSLT - [eXtensible Stylesheet Language](https://www.w3schools.com/xml/xsl_intro.asp)

The basics of XSLT is to create templates that match the nodes in the structure.

### Two type of templates:
 + Match (Unnamed) Templates
 + Named Templates

`<xsl:template>` is used to build a template

## Match (Unnamed) Templates

### Example of Match Template

```xml
<?xml version="1.0"?>
<title>
<para>A source paragraph.</para>
<note>This is a note.</note>
<para>Another source paragraph.</para>
</title>
```

```xml
<xsl:template match="/">
. . .
</xsl:template>
```

```xml
<xsl:template match="title/para">
. . .
</xsl:template>
```

+ The match attribute specifies which node the template should be invoked.

`<xsl:element>` create an element node in the output document.
`<xsl:attribute>` create an attribute node in the output document.
`<xsl:variable>` element declare a local or global variable.
`<xsl:value-of>` extracts the value of a selected node through the XPath expression.

## Named Template

Named templates operate like functions in traditional programming languages.