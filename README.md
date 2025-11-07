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
