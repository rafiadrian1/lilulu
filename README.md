# ForestRacks Pterodactyl Installer
Welcome to the ForestRacks Pterodactyl Installer repository! This installer is specifically designed for ForestRacks customers to easily install and set up the Pterodactyl Panel on Debian-based or RHEL-based machines. If you encounter any issues during the installation process, our troubleshooting section has some helpful tips.

## Installation:
1) To get started, it's important to ensure that your machine is freshly reinstalled if you've made any changes to it beforehand. 
2) Point a DNS A-Record to your machine's IP address, such as panel.forestracks.com to 192.168.53.72.
3) To download and run the installer, simply enter the following command into your terminal and follow the prompts:
```
bash <(curl -Ss https://raw.githubusercontent.com/ForestRacks/PteroInstaller/Production/install.sh || wget -O - https://raw.githubusercontent.com/ForestRacks/PteroInstaller/Production/install.sh) auto
```
## Post Installation:
* Please note "example.com" refers to the panel URL you set during the installation process.
1) After the installation is complete, go to http://example.com/admin/nodes/view/1/allocation to add the necessary ports for your games.

## Troubleshooting:
1) If you receive a mysql connection error, you may have run the installer multiple times – in this case, the best solution is to reinstall your operating system and run the install script again.
2) If you encounter Let's Encrypt SSL generation errors, it could be because you're using an IP address instead of a domain or because the FQDN you're trying to generate an SSL for doesn't have an A-Record pointing to your machine IP.

## Compatible Operating Systems:
| Operating System | Version | Supported          | PHP Version |
| ---------------- | ------- | ------------------ | ----------- |
| Ubuntu           | 20.04   | :white_check_mark: | 8.3         |
|                  | 22.04   | :white_check_mark: | 8.3         |
|                  | 24.04   | :white_check_mark: | 8.3         |
| Debian           | 11      | :white_check_mark: | 8.3         |
|                  | 12      | :white_check_mark: | 8.3         |
|                  | 13      | :red_circle: \*    |             |
| Rocky Linux      | 8       | :white_check_mark: | 8.3         |
|                  | 9       | :white_check_mark: | 8.3         |
| AlmaLinux        | 8       | :white_check_mark: | 8.3         |
|                  | 9       | :white_check_mark: | 8.3         |

## Contributors ✨

We would like to thank the following contributors for their work in maintaining and creating this installer:
1) [Zinidia](https://github.com/Zinidia)
2) [Vilhelm Prytz](https://github.com/vilhelmprytz)
3) [ImGreen](https://github.com/GreenDiscord)
3) [Neon](https://github.com/DeveloperNeon)
4) [sam1370](https://github.com/sam1370)
5) [Linux123123](https://github.com/Linux123123)
