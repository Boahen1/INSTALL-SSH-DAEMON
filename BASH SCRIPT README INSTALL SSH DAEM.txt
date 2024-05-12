BASH SCRIPT README: INSTALL SSH DAEMON

Description
This Bash script is designed to check if the SSH daemon (sshd) is installed on a system. If it's not installed, the script will proceed to install it using the DNF package manager (commonly found in Centos, RedHat and Fedora-based Linux distributions).

Instructions
Check for SSH Daemon Installation: The script begins by checking if the sshd package is already installed on the system.
Installation Procedure: If sshd is not found, the script proceeds to install it using dnf install sshd -y. The -y flag is used to automatically confirm the installation without user prompts.

Usage
Ensure the script has executable permissions. If not, grant them using:
chmod +x ssh_install.sh
Execute the script:
. / ssh_install.sh or bash ssh_install.sh

Notes
Root Permissions: The script utilizes sudo to gain administrative privileges for the installation process. Ensure the user running the script has sudo privileges.
Package Name: The script assumes the package name for SSH daemon as "sshd". If the package name varies in your distribution, modify the package_name variable accordingly.

Compatibility
This script is primarily designed for systems using the DNF package manager, commonly found in Fedora-based Linux distributions and Linux Redhat Enterprise. Adjustments may be necessary for other package managers such as APT or YUM.
Disclaimer
Use this script at your own risk. Ensure you understand the implications of installing system packages, especially when running scripts with elevated privileges.

Author
This script was created by Boahen Appiah-Agyei. Feel free to modify and distribute it according to your needs.
