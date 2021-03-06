# .NET API for Comparing Documents

A .NET component that enables your apps to [detect content, style & formatting differences among two documents](https://products.groupdocs.com/comparison/net), and allows you to accept or reject the changes.

## Document Comparison Processing Features

- [Compare and detect differences](https://docs.groupdocs.com/display/comparisonnet/Comparison) among source and target documents.
- Comparison works at the paragraph, word as well as the character level.
- Identify content styling and formatting modifications.
- Choose the modifications to accept or reject.
- Export the differences to the resultant document.
- Create and fetch after comparison difference summary report.
- Fetch coordinates of the modifications in document preview images.
- Support to set metadata from the source, target files or keep it user-defined.
- Make the resultant document password protected.

## Major Features in Version 20.3.1

- This is a hotfix that fixes comparing SpreadSheet documents using .NET Core version of GroupDocs.Comparison.

For the detailed notes, please visit [GroupDocs.Comparison for .NET 20.3.1 Release Notes](https://docs.groupdocs.com/display/comparisonnet/GroupDocs.Comparison+for+.NET+20.3.1+Release+Notes).

## Enhancements in Version 20.3

- Increase performance for *TXT* MultiComparer.

For the detailed notes, please visit [GroupDocs.Comparison for .NET 20.3 Release Notes](https://docs.groupdocs.com/display/comparisonnet/GroupDocs.Comparison+for+.NET+20.3+Release+Notes).

## Microsoft Office Formats

**Microsoft Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTX
**Microsoft Excel:** XLS, XLT, XLSX, XLTM, XLSB, XLSM, XLSX
**Microsoft PowerPoint:** POT, POTX, PPS, PPSX, PPTX, PPT
**Microsoft OneNote:** ONE
**Microsoft Visio:** VSDX, VSD, VSS, VST, VDX

## Other Formats

**OpenDocument:** ODT, ODP, OTP, ODS, OTT
**Portable:** PDF
**AutoCAD:** DWG, DXF
**Email:** EML, EMLX, MSG
**Images:** BMP, GIF, JPG, JPEG, PNG, DICOM
**Web:** HTM, HTML, MHT, MHTML
**Text:** TXT, CSV
**eBook:** MOBI, DJVU

## Supported Platforms

**Microsoft Windows:** Microsoft Windows Desktop (x86, x64) (XP & up), Microsoft Windows Server (x86, x64) (2000 & up), Windows Azure
**Mac OS:** Mac OS X
**Linux:** Linux (Ubuntu, OpenSUSE, CentOS and others)
**Development Environments:** Microsoft Visual Studio (2010 & up), Xamarin.Android, Xamarin.IOS, Xamarin.Mac, MonoDevelop 2.4 and later.
**Supported Frameworks:** GroupDocs.Comparison for .NET  supports .NET and Mono frameworks.

## Getting Started with GroupDocs.Comparison for .NET

Are you ready to give GroupDocs.Comparison for .NET a try? Simply execute `Install-Package GroupDocs.Comparison` from Package Manager Console in Visual Studio to fetch & reference GroupDocs.Comparison assembly in your project. If you already have GroupDocs.Comparison for .Net and want to upgrade it, please execute `Update-Package GroupDocs.Comparison` to get the latest version.

Please check the [GitHub Repository](https://docs.groupdocs.com/display/comparisonnet/home) for other common usage scenarios.

## Use C# to Compare Multiple DOCX Files with Specific Criteria

```csharp
using (Comparer comparer = new Comparer(“source.docx”)
{
    comparer.Add(“target1.docx”);
    comparer.Add(“target2.docx”);
    comparer.Add(“target3.docx”);
    CompareOptions compareOptions = new CompareOptions()
    {
        InsertedItemStyle = new StyleSettings()
        {
            FontColor = System.Drawing.Color.Yellow
        }
    };
    comparer.Compare(“result.docx”, compareOptions);
}
```

[Product Page](https://products.groupdocs.com/comparison/net) | [Documentation](https://docs.groupdocs.com/display/comparisonnet/home) | [Demo](https://products.groupdocs.app/comparison/family) | [API Reference](https://docs.groupdocs.com/display/comparisonnet/home) | [Examples](https://docs.groupdocs.com/display/comparisonnet/home) | [Blog](https://blog.groupdocs.com/category/comparison/) | [Free Support](https://blog.groupdocs.com/category/comparison/) | [Temporary License](https://purchase.groupdocs.com/temporary-license)
