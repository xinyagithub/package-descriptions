# GIS Data Manipulation & Conversion APIs for .NET

[Aspose.GIS for .NET](https://products.aspose.com/gis/net) API helps developers render maps, read, write & convert geographic information fetched from vector-based geospatial data formats without needing any other GIS software. The GIS .NET API supports working with Shapefile, GeoJSON, ESRI File Geodatabase (FileGDB), Geography Markup Language (GML), Keyhole Markup Language (KML), Scalable Vector Graphics (SVG) and many others.

It allows to read and write GIS data, [convert GIS file formats](https://docs.aspose.com/display/gisnet/Conversion), and [render maps](https://docs.aspose.com/display/gisnet/Map+Rendering) to SVG format. You can also create and analyze feature geometries as well as create basic geometries, such as, Point, MultiPoint, Line, Multiline and Polygon from scratch. The API supports to build non-linear (curve) geometries, linearize non-linear geometries, and control precision mode of calculations.

## GIS API Features

- [Render maps to PNG, JPEG, BMP, or SVG](https://docs.aspose.com/display/gisnet/Map+Rendering).
- Iterate through layer features.
- Read layer features by index.
- Fetch metadata about vector layers.
- Create new layers and datasets as well as work with multi-layer dataset.
- Convert vector data to [popular file formats](https://docs.aspose.com/display/gisnet/Supported+File+Formats).
- Perform re-projection during data conversion.
- Adjust feature attributes while converting.
- Customize styling of each geometry type.
- Perform complex drawing by combining several symbolizers.
- Apply layer rendering rules to control feature visual representation.
- Use value attributes to calculate styling parameters of a feature.
- Perform vector analysis & [manipulate geometries](https://docs.aspose.com/display/gisnet/Working+with+Geometries).
- Support for [Spatial Reference Systems](https://docs.aspose.com/display/gisnet/Spatial+Reference+Systems).

## Enhancements in Version 20.4

- Read *EsriASCII*, *GeoTIFF* and *TIFF*.
- Read georeference and raster sizes.
- Read values of numeric types (Bit, SByte, Byte, Short, UShort, Integer, UInteger, Long, Float, Double).
- Read raw bits for unknown data types.
- Read raster data by blocks.
- Supports *multy и single* bands.
- Summary statistics (count, sum, mean, min and max)

For detailed notes, please visit [Aspose.GIS for .NET 20.4 Release Notes](https://docs.aspose.com/display/gisnet/Aspose.GIS+for+.NET+20.04+Release+Notes).

## Read & Write GIS Formats

**ESRI Shapefile:** SHP, SHX, DBF
**GeoJSON:** JSON, GeoJSON
**TopoJSON:** JSON, TopoJSON
**ESRI File Geodatabase:** GDB
**Google Earth:** KML

## Read GIS Formats

**Geography Markup Language:** GML
**GPS Exchange Format:** GPX
**MapInfo Interchange Format:** MIF
**MapInfo Tab Format:** TAB, DAT, DBF
**OpenStreetMap:** OSM
**Other:** GeoTIFF, ESRI ASCII

## Render GIS Files As Images

**Images:** SVG, PNG, JPEG, JPG, BMP

## Platform Independence

Aspose.GIS for .NET API's uniform model is based on 100% managed code. This API can be used to develop several different types of .NET apps including ASP.NET, WinForms and Windows Services. It is easy to use & deploy, and provides the ideal solution to work with geo-spatial information with .NET Framework 4.7, .NET Standard 2.0 & Xamarin platforms.

## Getting Started with Aspose.GIS for .NET

Are you ready to give Aspose.GIS for .NET a try? Simply execute `Install-Package Aspose.GIS` from Package Manager Console in Visual Studio to fetch the NuGet package. If you already have Aspose.GIS for .NET and want to upgrade the version, please execute `Update-Package Aspose.GIS` to get the latest version.

## Convert a Shapefile to GeoJSON Format with C#

You can execute below code snippet to see how Aspose.GIS API works after adding Aspose.GIS for .NET to your project or check the [GitHub Repository](https://github.com/aspose-gis/Aspose.GIS-for-.NET) for other common usage scenarios. 

```csharp
VectorLayer.Convert(dir + "template.shp", Drivers.Shapefile, dir + "output.json", Drivers.GeoJson);
```

[Product Page](https://products.aspose.com/gis/net) | [Documentation](https://docs.aspose.com/display/gisnet/Home) | [Demo](https://products.aspose.app/gis/family) | [API Reference](https://apireference.aspose.com/net/gis) | [Examples](https://github.com/aspose-gis/Aspose.GIS-for-.NET) | [Blog](https://blog.aspose.com/category/gis/) | [Free Support](https://forum.aspose.com/c/gis) |  [Temporary License](https://purchase.aspose.com/temporary-license)
