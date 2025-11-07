# Cold Email Sender - MAUI .NET 8 App

## Description

This application is for sending emails with attachments.  

- Uses **MAUI .NET 8**.  
- Requires configuring Gmail with an **App Passcode** (NOT PASSWORD) for this app to send emails.  
  - Create a new passcode for this app.  
  - Enable **2FA** for security.  
  - [Google App Passwords Guide](https://myaccount.google.com/apppasswords)  
- Works on **Windows** and **macOS**.

---

## Setup Instructions

1. **Edit Home.razor**
   - Open the `Home.razor` file in a text editor or IDE.  
   - Replace the placeholder values with your Gmail sender email and **App Passcode**:

   ```csharp
   var smtpUser = "your_email@gmail.com";       // Replace with your Gmail address
   var smtpPass = "your_16_char_app_password"; // Replace with your Gmail App Passcode
``


## Publish Instructions

### **Windows**
1. Open Command Prompt and navigate to the project folder:
```bash
cd path\to\ColdEmailSender_Man3 


### **MAC**
1. Open Command Prompt and navigate to the project folder:
```bash
cd path/to/ColdEmailSender_Man3
dotnet publish -f net8.0-macos -c Release -p:SelfContained=true -r osx-arm64
bin/Release/net8.0-macos/publish/ColdEmailSender.app
