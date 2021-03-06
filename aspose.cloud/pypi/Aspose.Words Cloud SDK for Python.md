Python Cloud SDK wraps Aspose.Words Cloud API so you could seamlessly integrate Microsoft Word® file generation, manipulation, conversion & inspection features into your own python applications.

[Aspose.Words Cloud SDK for Python](https://products.aspose.cloud/slides/python) allows to work with Word document headers, footers, page numbering, tables, sections, document comments, drawing objects, FormFields, fonts, hyperlinks, ranges, paragraphs, math objects, watermarks, revisions and document protection. It also assists in appending documents, splitting documents as well as converting document to other supported file formats. Please feel free to explore the [Developer's Guide](https://docs.aspose.cloud/display/wordscloud/Developer+Guide) for all possible usage scenarios. 

## Document Processing Features

- Programmatically create new documents of various file formats.
- Availability of Mail Merge and report generation features.
- Split or merge documents on demand.
- Manage watermarks and protection.
- Full read & write access to Document Object Model.
- Fetch web pages via URL and save in Microsoft Word file formats.
- Get document information in JSON or XML representation.
- [Fetch statistical data](https://docs.aspose.cloud/display/wordscloud/Get+Document+Statistics) of a document.
- [Remove all macros](https://docs.aspose.cloud/display/wordscloud/Remove+all+Macros+from+Document) contained in a specific document.
- [Convert a document to desired file format](https://docs.aspose.cloud/display/wordscloud/Convert+Document+to+Destination+Format+with+Detailed+Settings+and+Save+Result+to+Storage) along with detailed settings.
- Convert an encrypted PDF document into Word document format.

## New Features in Version 20.4

- Added `UseTargetMachineFonts` option to `HtmlFixedSaveOptions` Data.
- Added `Password` option to `OdtSaveOptions`.
- Provision of Compare Options in Aspose.Words Cloud.
- Added new `SaveOptionsData.UpdateLastPrintedProperty`.
- Added new Saveoption Dml3DEffectsRenderingMode.
- Added new PdfSaveOption "InterpolateImages".

For the detailed notes, please visit [Aspose.Words Cloud 20.4 Release Notes](https://docs.aspose.cloud/display/wordscloud/Aspose.Words+Cloud+20.4+Release+Notes).

## Read & Write Document Formats

**Microsoft Word:** DOC, DOCX, RTF, DOT, DOTX, DOTM, FlatOPC (XML)
**OpenOffice:** ODT, OTT
**WordprocessingML:** XML
**Web:** HTML, MHTML, HtmlFixed
**Text:** TXT
**Fixed Layout:** PDF

## Save Document As

**Fixed Layout:** PDF/A, XPS, OpenXPS, PS
**Images:** JPEG, PNG, BMP, SVG, TIFF, EMF
**Others:** PCL

## Getting Started with Aspose.Words Cloud SDK for Python

Firstly, create an account at [Aspose for Cloud](https://dashboard.aspose.cloud/#/apps) to get your application information and free quota to use the API. Now execute `pip install aspose-words-cloud` from the command line to fetch the SDK. Then import the package via `import asposewordscloud`. 

### Install via Setuptools

Execute `python setup.py install --user` and import the package as `import asposewordscloud`.

The complete source code is available at [GitHub Repository](https://github.com/aspose-words-cloud/aspose-words-cloud-python).

## Delete Watermarks from Word Document via Python

```python
import asposewordscloud
import asposewordscloud.models.requests

api_client = asposewordscloud.ApiClient()
api_client.configuration.host = 'https://api.aspose.cloud'
api_client.configuration.api_key['api_key'] = '' # Put your appKey here
api_client.configuration.api_key['app_sid'] = '' # Put your appSid here
storage_api = asposestoragecloud.StorageApi(asposestoragecloud.ApiClient('', '')) # Same credentials for storage
storage_api.api_client.configuration.base_url = 'https://api.aspose.cloud/v1.1'
words_api = asposewordscloud.WordsApi(api_client)
filename = 'test_doc.docx'
remote_name = 'TestDeleteDocumentWatermark.docx'

with open(os.path.join(self.local_common_folder, filename), 'rb') as f:
    file = f.read()
self.storage_api.put_create(os.path.join(self.remote_test_folder, self.test_folder, remote_name), file)
request = asposewordscloud.models.requests.DeleteDocumentWatermarkRequest(remote_name,
                                                                           os.path.join(
                                                                                 self.remote_test_folder,
                                                                                 self.test_folder))
result = words_api.delete_document_watermark(request)
self.assertTrue(result.code == 200, 'Error has occurred while delete document watermark')
```

[Product Page](https://products.aspose.cloud/words/python) | [Documentation](https://docs.aspose.cloud/display/wordscloud/Home) | [Demo](https://products.aspose.app/words/family) | [API Reference](https://apireference.aspose.cloud/words/) | [Examples](https://github.com/aspose-words-cloud/aspose-words-cloud-python) | [Blog](https://blog.aspose.cloud/category/words/) | [Free Support](https://forum.aspose.cloud/c/words) | [Free Trial](https://dashboard.aspose.cloud/#/apps)
