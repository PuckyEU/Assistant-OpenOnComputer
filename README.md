# Hey Google, Open ... On My Computer
> [!NOTE]
> This guide is still in development and might not contain all the steps necessary to achieve complete functionality.

Guide on how to set up a Google Assistant command to open an application on your computer.

It will require manual setup and almost no coding.

## Table of Contents
- [General Idea](#general-idea)
- [Obtaining your IP](#obtaining-your-ip)
  - [Windows](#windows)
  - [MacOS](#macos)
  - [Linux](#linux)
- [How to Set up the Google Assistant Command](#how-to-set-up-the-google-assistant-command)

## General Idea
This program would run a local server on the computer you want to open something on. The server would have code that would open a website whenever someone entered a specific link. For example, if you wanted to open Netflix, you would enter the link `[computer_ip]:8080/netflix`. The server would recognize that you want to open Netflix and open the website.

You can also use custom routines in the Google Home app to simplify this process. You can create a routine that, when you say "Hey Google, open Netflix on my TV," the assistant will open the link `[computer_ip]:8080/netflix`. [Here](#how-to-set-up-the-google-assistant-command) is a guide on how to do this.

Here is a more detailed explanation of how the program would work:

1. The program would start a local server on the computer you want to open something on.
2. The server would have code that would open a website whenever someone entered a specific link.
3. When someone entered the link, the server would recognize the link and open the website.
4. You could also create a custom routine in the Google Home app to simplify this process.
5. The custom routine would, when you said a specific phrase, open the link.

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
<div align="center">
  <details>
    <summary>Show Diagram</summary>
    <img src="/Images/google_home.png" alt="Google Home App" width="1200"/>
  </details>
</div>
