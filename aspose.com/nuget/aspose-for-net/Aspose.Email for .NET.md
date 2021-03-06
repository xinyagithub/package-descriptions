# .NET Email API

[Aspose.Email for .NET](https://products.aspose.com/email/net) allows you to work with MIME messages, appointments, Microsoft Outlook® items, Outlook storage files, various clients & protocols ([SMTP](https://docs.aspose.com/display/emailnet/Working+with+SMTP+Client), [POP3](https://docs.aspose.com/display/emailnet/Working+with+POP3+Client), [IMAP](https://docs.aspose.com/display/emailnet/Working+with+IMAP+Client), [Exchange EWS](https://docs.aspose.com/display/emailnet/Working+with+Exchange+EWS+Client), [Exchange WebDav](https://docs.aspose.com/display/emailnet/Working+with+Exchange+WebDav+Client), [Gmail](https://docs.aspose.com/display/emailnet/Programming+with+Gmail), [Thunderbird](https://docs.aspose.com/display/emailnet/Programming+with+Thunderbird), [Zimbra](https://docs.aspose.com/display/emailnet/Working+with+Zimbra), [IBM Notes](https://docs.aspose.com/display/emailnet/Working+with+IBM+Notes) & AMP HTML emails and more.

## Email API Features

- Open or save emails in Microsoft Outlook & other formats.
- Conversion of email files to various formats.
- Parse, read & save MS Outlook emails, PST & OST files.
- [Comprehensive support for MIME messages](https://docs.aspose.com/display/emailnet/Working+with+MIME+Messages).
- Send & receive emails via POP3, IMAP, Microsoft Exchange Server.
- Send emails in bulk while performing mail merge via various types of data sources.
- Send iCalendar compliant messages.
- Consume and produce recurrence patterns in the iCalendar (RFC 2445) format.
- Tools to verify email addresses, email syntax, email domain, mail server & MX records.
- Extract objects from various mail storage formats as well as [create email storage files from scratch](https://docs.aspose.com/display/emailnet/Create+New+PST+File+and+Add+SubFolders).

## New Features in Version 20.4

- Ability to enable mail clients activity logging in the .NET Core projects.
- Support for the ability to ignore exceptions.

## Enhancements in Version 20.4

- Get message information by unique identifiers for *Pop3Client* and *ImapClient*.

For the detailed notes, please visit [Aspose.Email for .NET 20.4 Release Notes](https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+20.4+Release+Notes).

## Read & Write Email Formats

**Microsoft Outlook:** MSG, PST, OST, OFT
**Email:** EML, EMLX, MBOX
**Others:** ICS, VCF, HTML, MHTML

## Read Email Formats

**Mac Outlook:** OLM

## Platform Independence

Aspose.Email for .NET is implemented using Managed C# and can be used with any .NET based languages including C#, VB.NET, J# and so on. Aspose.Email for .NET can be integrated with any kind of application on Windows, Linux, Mac OS X and Xamarin Platforms.

## Getting Started with Aspose.Email for .NET

Are you ready to give Aspose.Email for .NET a try? Simply execute `Install-Package Aspose.Email` from Package Manager Console in Visual Studio to fetch the NuGet package. If you already have Aspose.Email for .NET and want to upgrade the version, please execute `Update-Package Aspose.Email` to get the latest version.

## Create an Email Message & Save it in MSG Format using C# Code

You can execute below code snippet to see how Aspose.Email API performs in your environment or check the [GitHub Repository](https://github.com/aspose-email/Aspose.Email-for-.NET) for other common usage scenarios. 

```csharp
// create an instance of the MailMessage class
var message = new MailMessage();
// set from, to, subject and body properties
message.From = "sender@domain.com";
message.To = "receiver@domain.com";
message.Subject = "This is test message";
mamessageilMsg.Body = "This is test body";
// create an instance of the MapiMessage class and pass object of MailMessage as argument
var msg = MapiMessage.FromMailMessage(message);
// save file on disc
msg.Save(dir + "output.msg");
```

## Send Bulk Emails via SMTP

```csharp
// create SmtpClient as client and specify server, port, user name and password
SmtpClient client = new SmtpClient("mail.server.com", 25, "Username", "Password");

// create instances of MailMessage class and Specify To, From, Subject and Message
MailMessage message1 = new MailMessage("msg1@from.com", "msg1@to.com", "Subject1", "message1, how are you?");
MailMessage message2 = new MailMessage("msg1@from.com", "msg2@to.com", "Subject2", "message2, how are you?");
MailMessage message3 = new MailMessage("msg1@from.com", "msg3@to.com", "Subject3", "message3, how are you?");

// create an instance of MailMessageCollection class
MailMessageCollection manyMsg = new MailMessageCollection();
manyMsg.Add(message1);
manyMsg.Add(message2);
manyMsg.Add(message3);

// send emails in bulk
client.Send(manyMsg);
```

## Use C# to Create an ICS Appointment

```csharp
// create and initialize an instance of the Appointment class
var appointment = new Appointment(
	"Meeting Room 3 at Office Headquarters",// Location
	"Monthly Meeting",                      // Summary
	"Please confirm your availability.",    // Description
	new DateTime(2015, 2, 8, 13, 0, 0),     // Start date
	new DateTime(2015, 2, 8, 14, 0, 0),     // End date
	"from@domain.com",                      // Organizer
	"attendees@domain.com");                // Attendees

// save the appointment to disk in ICS format
appointment.Save("output.ics", AppointmentSaveFormat.Ics);
```

[Product Page](https://products.aspose.com/email/net) | [Documentation](https://docs.aspose.com/display/emailnet/Home) | [Demo](https://products.aspose.app/email/family) | [API Reference](https://apireference.aspose.com/net/email) | [Examples](https://github.com/aspose-email/Aspose.Email-for-.NET) | [Blog](https://blog.aspose.com/category/email/) | [Free Support](https://forum.aspose.com/c/email) | [Temporary License](https://purchase.aspose.com/temporary-license)
