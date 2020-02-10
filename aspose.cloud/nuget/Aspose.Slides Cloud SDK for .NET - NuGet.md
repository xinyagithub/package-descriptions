This REST API enables your C#, ASP.NET & other .NET cloud-based apps to process & manipulate PPT, PPTX, ODP, OTP presentations in the cloud.

Aspose.Slides Cloud SDK for .NET is a wrapper around Aspose.Slides REST API and is offered under an MIT license. Enhance your .NET programs to create presentations in the cloud, pick and merge specific slides, split presentations, extract images from presentation in any of the supported file formats, extract & download slide notes, clone master slide information, and so much more.

## Presentation Processing Features

- Fetch presentation images in any of the supported file formats.
- Copy layout side or clone master slide from the source presentation.
- Process slides shapes, slides notes, placeholders, colors & font theme info.
- Programmatically create presentation from HTML & export it to various formats.
- Merge multiple presentations or split single presentation into multiple ones.
- Extract and replace text from specific slide or entire presentation.

## Read & Write Presentation Formats

**Microsoft PowerPoint:** PPT, PPTX, PPS, PPSX, PPTM, PPSM, POTX, POTM
**OpenOffice:** ODP, OTP

## Save Presentation As

**Fixed Layout:** PDF, PDF/A, XPS
**Images:** JPEG, PNG, BMP, TIFF, SVG
**Web:** HTML
**Other:** SWF (export whole presentations)

## Platform Independence

Aspose.Slides Cloud’s platform independent document manipulation API is a true REST API that can be used from any platform. You can use it with any language or platform that supports REST, be it the web, desktop, mobile, or the cloud. The API integrates with other cloud services to provide you the flexibility you require for processing documents. It is suitable for the most types of businesses, documents, or content.

## Getting Started with Aspose.Slides Cloud SDK for .NET

You do not need to install anything to get started with Aspose.Slides Cloud SDK for .NET. Just create an account at [Aspose for Cloud](https://dashboard.aspose.cloud/#/apps) and get your application information.

Simply execute `Install-Package Aspose.Slides-Cloud` from the Package Manager Console in Visual Studio to fetch & reference Aspose.Slides assembly in your project. If you already have Aspose.Slides Cloud SDK for .NET and want to upgrade it, please execute `Update-Package Aspose.Slides-Cloud` to get the latest version.

Please check the [GitHub Repository](https://github.com/aspose-slides-cloud/aspose-slides-cloud-dotnet) for other common usage scenarios.

## Convert PPTX Presentation to JPEG Format via C# Code

The following C# code sample elaborates, how to easily convert a cloud-based Microsoft PowerPoint presentation PPTX file to JPEG image format via REST API:

```csharp
PostSlidesSaveAsRequest request = new PostSlidesSaveAsRequest();
// the presentation that is to be converted
request.Name="Input_Presentation.pptx";
// the export format for the PPTX file
request.Format=ExportFormat.Jpeg;

return request;
```

## Use C# to Replace Specific Text on the Selected PPTX Slide

The following code sample demonstrates, how to replace a specific piece of text on the presentation slide of your choice using C# code:

```csharp
PostSlidesSlideReplaceTextRequest request = new PostSlidesSlideReplaceTextRequest();
// slide on which the text to be updated is present
request.SlideIndex = 0;
// name of the presentation that contains the text
request.Name = "Input_Presentation.pptx";
// text string that needs to be updated
request.OldValue = "This text is going to be replaced.";
// new text string that replaces the older value
request.NewValue = "This text replaces the older text.";
// the text manipulation is not case-sensitive
request.IgnoreCase = true;
return request;
```

[Product Page](https://products.aspose.cloud/slides/net) | [Documentation](https://docs.aspose.cloud/display/slidescloud/Home) | [API Reference](https://apireference.aspose.cloud/slides/) | [Code Samples](https://github.com/aspose-slides-cloud/aspose-slides-cloud-dotnet) | [Blog](https://blog.aspose.cloud/category/slides/) | [Free Support](https://forum.aspose.cloud/c/slides) | [Free Trial](https://dashboard.aspose.cloud/#/apps)