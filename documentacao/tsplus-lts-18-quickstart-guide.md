# TSplus LTS 18 - Quickstart Guide

> **Documentação completa TSplus** — 9 páginas

---


---
*Página 1*

TSplus Remote Access v18: Quickstart
Guide
Prerequisites:
On the Server:
OS: Microsoft Windows Versions 7 to 11 or Windows Server 2008R2 to 2025 with at least
2GB of RAM.
TSplus does not support installation of Remote Access on Windows Home Editions.
The operating system must be on the C: drive.
Java Runtime Environment. If Java is not already installed, Remote Access will install
OpenJDK during setup.
If you are installing Remote Access on a Windows Server operating system, make sure that
the RDS/Terminal Services and RDS/Terminal Services licensing roles are not installed
before installing TSplus Remote Access.
Your Remote Access server must have a static private IP address.
For External access, your server must have a static public IP address or dynamic DNS
provider.
TSplus Remote Access built-in Web server requires Java OpenJDK 17 or greater..
On the Client:
OS: Microsoft Windows Versions 7 to 11 are fully supported.
For MacOS you can use any Mac RDP client or the TSplus HTML5 client.
For Linux you can use Rdesktop or the TSplus HTML5 client.
Java Runtime Environment.
A PDF reader (example: Foxit Reader or Acrobat DC)
For more detailed prerequisites please see the documentation
Note:
Starting with Remote Access Version 15, the Administration console has changed its look. A Lite
Mode and an Expert Mode have been introduced. Administrators can toggle between the two
interface styles by clicking the button in the upper-right corner of the Admin Console.

---
*Página 2*

Step 1 : Installation.
Note:
The trial version of Remote Access is the fully-featured Enterprise Edition. It is licensed for up to
5 concurrent users for a period of 15 days.
Installing TSplus Remote Access is an easy process. Just download it from our web site, run the
Setup-TSplus.exe program.
Files are decompressed and copied into:
C:\Program Files\TSplus (32-bit systems)
C:\Program Files(x86)\TSplus (64-bit systems).
Once the installation is complete the installer will ask you to reboot.
After the reboot, you will see 2 new icons on your Desktop:

---
*Página 3*

The AdminTool is what you need to use Remote Access.
The Portable Client Generator is used to create Remote Access connection clients for your
users.
See the documentation for full installation instructions.
Step 2 : Creating users.
After the reboot, the Remote Access Server is almost ready to go. Now we’ll create users. Open
the AdminTool to get started. Then go to the System Tools tab and click on “Users and Groups”.
This will take you to the Local Users and Groups window:

---
*Página 4*

Each user must have a User Name AND a Password. When creating users, be aware of the box
labeled “User must change password at next logon”. If you don’t want your users to change their
password during the first login, uncheck this box and check the “Password never expires” or
“User cannot change password”.
Step 3 : Select the most suitable client for your needs.
Remote Access is compatible with Windows Remote Desktop Protocol. Any user can connect
locally or remotely with a standard Remote Desktop Connection client (mstsc.exe) or any RDP
compatible client. To fully benefit from the advanced features in Remote Access (RemoteApp,
Universal Printer…) you can use a generated client or the Remote Access Web Portal.
Remote Access is a very flexible solution and offers multiple ways to open a session:
Classic Remote Desktop Connection (MSTSC.EXE).
Portable TSplus RDP client which will display a windowed environment for your remote
connection that you can minimize in the Windows taskbar.
MS RemoteAPP client which will display application using the native MS RemoteApp.
Windows client over the TSplus Web Portal.
HTML5 client over the TSplus Web Portal.
These clients give the user the following experience:

---
*Página 5*

With Remote Desktop Connection (mstsc.exe)
Connection: The connection is a very standard one. The Universal Printer is not supported
with this type of connection.
Display: Users will see their session within a Remote Desktop window. This desktop displays
the content of the user’s desktop folder.
If the administrator has assigned specific applications with the AdminTool, only these
applications will be displayed (no taskbar, no Desktop).
TSplus RDP generated client.
This is a unique TSplus solution, it empowers local and remote users to connect using one single
dedicated program.
It includes the connection program, the Universal Printing advanced feature, portability with high
level of security while keeping it very simple for the users.
For more information about using the TSplus Client Generator, see this documentation
The TSplus RemoteApp generated Client.
Remote applications will look and behave like a local application. Instead of a classic Remote
Desktop window, you will be free to switch between your local and remote applications without
having to minimize a Remote Desktop window.
For more information about these clients, see this documentation.
Accessing your TSplus Remote Access server from a
remote location
To access your Remote Access server from outside of your local network, you will have to create
a port forwarding or port redirection rule of 3389/80/443 ports depending on your preferred
connection method. You can change the RDP port in the Home tab:

---
*Página 6*

The 80/443 ports can be changed in the Web Server tab:

---
*Página 7*

Step 4 : Application Publishing and Application
Control.
In the Remote Access AdminTool you can assign application to users or groups.
If you assign one application to a user, they will only see this application.
You also can assign them the TSplus Taskbar, the Floating Panel or the Application Panel to
display multiple applications.
You can also publish a full Remote Desktop.
Now available in
Lite Mode
from the home tab.

---
*Página 8*

Or go to Expert Mode > Apps tab to add, edit, delete, and assign apps.

---
*Página 9*

In this example, the administrator has decided that the user ‘John’ will get the TSplus Taskbar.
See this documentation for more information.
Thank you for using TSplus Remote Access!