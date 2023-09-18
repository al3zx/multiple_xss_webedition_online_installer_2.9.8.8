# Multiple XSS in webEdition Online Installer Version 2.9.8.8

**Software link**: webEdition CMS [https://www.webedition.org/de/webedition/]

**webEdition Installer Version**: 2.9.8.8


**webEdition installed version**: 9.2.2 (Cardada)

**@author**: Alejandro Amorín

**Description**: Multiple cross-site scripting (XSS) vulnerabilities in OnlineInstaller/setup.php of webEdition Online Installer v2.9.8.8 allow attackers to execute arbitrary web scripts or HTML via a crafted payload injected into several parameters of the installation procedure.

## POC

When performing the installation the 'Host' field in the 'Proxy server' section is affected by the injection of arbitrary code:



When performing the installation the 'Server (Host)' and the 'Database' fields in the 'Database' section are affected by the injection of arbitrary code:
