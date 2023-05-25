# Hey Google, Open ... On My Computer
<blockquote>Note that this guide is still in development and might not have all the steps necessary.</blockquote>

Guide on how to set up a Google Assistant command to open an application on your computer.

It will require manual setup and almost no coding.

## Table of Contents
- [Obtaining your IP](#obtaining-your-ip)
  - [Windows](#windows)
  - [MacOS](#macos)
  - [Linux](#linux)
- [How to Set up the Google Assistant Command](#how-to-set-up-the-google-assistant-command)

## Obtaining your IP
#### Windows:
- Press the Windows key + R to open the Run dialog box.
- Type cmd and press Enter to open the Command Prompt.
- In the Command Prompt, type ipconfig and press Enter.
- Look for the "IPv4 Address" or "IPv6 Address" under the network adapter you are connected to. This address represents your computer's IP address.

#### macOS:
- Open "Terminal" from the Applications > Utilities folder.
- In the Terminal window, type ifconfig and press Enter.
- Look for the "inet" or "inet6" address associated with your network connection. This address represents your computer's IP address.

#### Linux:
- Open the Terminal application.
- Type ifconfig and press Enter.
- Look for the "inet" or "inet6" address associated with your network interface. This address represents your computer's IP address.

## How to Set up the Google Assistant Command
- Open the Google Home app
- Go to the Automations Tab
- Create a new Automation:
  - Pick whether it will be a household or personal automation
  - Add a starter:
    - Pick the option `When I say to Google Assistant`
    - Type a catchphrase to open your program on the computer, but you might have to find a specific one that works for your case, because sometimes the assitant might confuse it with other commands.
  - Add an action:
    - Pick the option `Try adding your own`
    - Type `Open [your_ip_address]`. Replace the `[your_ip_address]` with [your computer's IP address](#obtaining-your-ip).
<img src="/Images/google_home.png" alt="Google Home App" width="500"/>