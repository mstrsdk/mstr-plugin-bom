# mstr-plugin-bom

### Description
This BOM can be used to create your custom MSTR Web plugins. It adds the MSTR Web JAR dependencies (provided) into your child component. This BOM inherits from mstr-bom, another BOM that includes the MSTR Web JAR references. This is how the hierarchy looks like when you use this BOM:

>mstr-bom
>>mstr-plugin-bom
>>>your-plugin-pom.

  
### How to use this BOM
Create a maven project that will create a WAR file, and add this mstr-plugin-bom as parent; example:

- We are creating a new plugin named: ***mstr-hide-banner-plugin***
- Below is an example of how the POM file looks like:

```xml
<project ...>
    <modelVersion>4.0.0</modelVersion>

    <parent>
        <groupId>com.mstsdk</groupId>
        <artifactId>mstr-plugin-bom</artifactId>
        <version>10.4</version>
    </parent>

    <groupId>com.eis.mstr.plugins</groupId>
    <artifactId>mstr-hide-banner-plugin</artifactId>
    <version>1.0-SNAPSHOT</version>
    <packaging>war</packaging>

</project>
```

This example uses MSTR Web v10.4


----

This BOM was provided by [MSTR SDK](https://www.mstrsdk.com)

Written by [Daniel Parra](mailto:daniel@mstrsdk.com)

November 2019
