*This project has been created as part of the 42 curriculum by mayhamda.*

# Born2beRoot

## Description

Born2beRoot is a system administration project from the 42 curriculum. Its goal is to create and secure a Linux virtual server using virtualization, user management, access control, and system monitoring.

I chose Debian GNU/Linux 13 (Trixie) because it is stable, beginner-friendly, and has a large software repository.

## Instructions

The server runs in Oracle VirtualBox without a graphical interface.

Main configuration:

- Hostname: `mayhamda42`
- Operating System: Debian GNU/Linux 13
- Disk: Encrypted LVM
- SSH: Port 4242, root login disabled
- Firewall: UFW, allowing incoming traffic on port 4242
- Security: AppArmor enabled
- Users: `mayhamda` belongs to `sudo` and `user42`
- Passwords: Strong password policy and password aging
- Monitoring: Bash script scheduled with cron every 10 minutes and at startup

## Technical Choices

### Debian vs Rocky Linux

Debian uses APT for package management and is beginner-friendly. Rocky Linux uses DNF and is focused on enterprise compatibility.

### AppArmor vs SELinux

AppArmor uses path-based security profiles. SELinux uses a label-based mandatory access control system.

### UFW vs firewalld

UFW provides a simple interface for firewall rules. Firewalld supports zones and more dynamic firewall configurations.

### VirtualBox vs UTM

VirtualBox is a general-purpose virtualization platform. UTM is commonly used for virtualization and emulation on macOS, particularly Apple Silicon.

Resources

Debian Documentation: https://www.debian.org/doc/

OpenSSH Documentation: https://www.openssh.com/manual.html

Ubuntu UFW Documentation: https://documentation.ubuntu.com/security/security-features/network/firewall/

AppArmor Documentation: https://apparmor.net/

VirtualBox Documentation: https://www.virtualbox.org/manual/

AI Usage

AI was used as a learning aid to explain Linux commands, understand security concepts, troubleshoot configuration errors, and review the project documentation. Configuration steps were performed and tested in the virtual machine.
