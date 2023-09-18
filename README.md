# Multiple XSS in webEdition Online Installer Version 2.9.8.8

**Software link**: webEdition CMS [https://www.webedition.org/de/webedition/]

**webEdition Installer Version**: 2.9.8.8

![xss00](https://github.com/al3zx/multiple_xss_webedition_online_installer_2.9.8.8/assets/20266218/dc0e089b-3130-440e-a1c9-2c9e54585c48)


**webEdition installed version**: 9.2.2 (Cardada)

![xss0](https://github.com/al3zx/multiple_xss_webedition_online_installer_2.9.8.8/assets/20266218/6b654c5a-aa30-4bec-9ba7-fbee5d0bd7c6)


**@author**: Alejandro Amorín

**Description**: Multiple cross-site scripting (XSS) vulnerabilities in OnlineInstaller/setup.php of webEdition Online Installer v2.9.8.8 allow attackers to execute arbitrary web scripts or HTML via a crafted payload injected into several parameters of the installation procedure.

## POC

When performing the installation the 'Host' field in the 'Proxy server' section is affected by the injection of arbitrary code:

![xss1](https://github.com/al3zx/multiple_xss_webedition_online_installer_2.9.8.8/assets/20266218/6b217377-8986-42e4-a9cb-8de8bee62d84)

![xss2](https://github.com/al3zx/multiple_xss_webedition_online_installer_2.9.8.8/assets/20266218/7ab738fb-bf52-4a89-a8df-2f423001c160)

When performing the installation the 'Server (Host)' and the 'Database' fields in the 'Database' section are affected by the injection of arbitrary code:

![xss3](https://github.com/al3zx/multiple_xss_webedition_online_installer_2.9.8.8/assets/20266218/b31bcff2-b889-4eda-8ea5-e654f13dd875)

![xss4](https://github.com/al3zx/multiple_xss_webedition_online_installer_2.9.8.8/assets/20266218/79c37a58-8fdf-4ade-9213-40f31b0dafa0)

![xss5](https://github.com/al3zx/multiple_xss_webedition_online_installer_2.9.8.8/assets/20266218/a98987fd-c8f8-476d-ad7f-19cb75603a94)

![xss6](https://github.com/al3zx/multiple_xss_webedition_online_installer_2.9.8.8/assets/20266218/4e7d162c-345c-4c39-8e7b-be8f390cb68c)
