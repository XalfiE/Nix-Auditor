# CIS-Audit
CIS Audit made easier (RHEL, CentOS)

Usage:
./CIS Audit.bash

Checks for the following CIS controls:
  # CIS 1.1.1 Test that there is a separate /tmp partition
  # CIS 1.1.2 Test that the nodev option is on the /tmp partition
  # CIS 1.1.3 Test that the nosuid option is on the /tmp partition
  # CIS 1.1.4 Test that the noexec option is on the /tmp partition
  # CIS 1.1.5 Test that there is a separate /var partition
  # CIS 1.1.6 Test that the /var/tmp directory is bind mounted onto the /tmp filesystem
  # CIS 1.1.7 Test that there is a separate /var/log partition
  # CIS 1.1.8 Test that there is a separate /var/log/audit partition
  # CIS 1.1.9 Test that there is a separate /home partition
  # CIS 1.1.10 Test that the nodev option is on the /home partition
  # TO DO CIS 1.1.11 nodev option on removable media partitions
  # TO DO CIS 1.1.12 noexec option on removable media partitions
  # TO DO CIS 1.1.13 nosuid option on removable media partitions
  # CIS 1.1.14 Test that the nodev option is on the /dev/shm partition
  # CIS 1.1.15 Test that the nosuid option is on the /dev/shm partition
  # CIS 1.1.16 Test that the noexec option is on the /dev/shm partition
  # CIS 1.1.17 Check for the sticky bit on all world writable dirs
  # CIS 1.1.18 Test that the mounting of cramfs filesystems is disabled  
  # CIS 1.1.19 Test that the mounting of freevxfs filesystems is disabled  
  # CIS 1.1.20 Test that the mounting of jffs2 filesystems is disabled  
  # CIS 1.1.21 Test that the mounting of hfs filesystems is disabled  
  # CIS 1.1.22 Test that the mounting of hfsplus filesystems is disabled  
  # CIS 1.1.23 Test that the mounting of squashfs filesystems is disabled  
  # CIS 1.1.24 Test that the mounting of udf filesystems is disabled  
  # CIS 1.2.1 Check that the CentOS GPG Key is Installed
  # CIS 1.2.2 Check that gpgcheck is globally activated
  # CIS 1.2.3 Check software package updates with yum
  # CIS 1.2.4 Verify package integrity using RPM
  # CIS 1.3.1 Check that the AIDE rpm is installed
  # CIS 1.3.2 Check periodic execution of file integrity (that aide runs from cron)
  # CIS 1.4.1 Check that SELinux is not disabled in /boot/grub2/grub.cfg 
  # CIS 1.4.2 Verify SELinux configured state in /etc/selinux/config
  # CIS 1.4.3 Verify SELinux policy in /etc/selinux/config
  # CIS 1.4.4 Check setroubleshoot RPM is not installed
  # CIS 1.4.5 Check setroubleshoot RPM is not installed
  # CIS 1.4.6 Check for unconfined daemons
  # CIS 1.5.1 Check ownership on /boot/grub2/grub.cfg
  # CIS 1.5.2 Check permissions on /boot/grub2/grub.cfg
  # CIS 1.5.3 Check permissions on /boot/grub2/grub.cfg
  # CIS 1.6.2 Verify that the flag to force randomized virtual memory region placement is set
  # CIS 2.1.1 Check telnet-server RPM is not installed
  # CIS 2.1.2 Check telnet RPM is not installed
  # CIS 2.1.3 Check rsh-server RPM is not installed
  # CIS 2.1.4 Check rsh RPM is not installed
  # CIS 2.1.5 Check ypbind RPM is not installed
  # CIS 2.1.6 Check ypserv RPM is not installed
  # CIS 2.1.7 Check tftp RPM is not installed
  # CIS 2.1.8 Check tftp-server RPM is not installed
  # CIS 2.1.9 Check talk RPM is not installed
  # CIS 2.1.10 Check talk-server RPM is not installed
  # CIS 2.1.11 Check xinetd RPM is not installed
  # CIS 2.1.12 Check chargen-dgram is not enabled
  # CIS 2.1.13 Check chargen-stream is not enabled
  # CIS 2.1.14 Check daytime-dgram is not enabled
  # CIS 2.1.15 Check daytime-stream is not enabled
  # CIS 2.1.16 Check echo-dgram is not enabled
  # CIS 2.1.17 Check echo-dgram is not enabled
  # CIS 2.1.18 Check tcpmux-server is not enabled
  # CIS 3.1 Check Daemon umask
  # CIS 3.2 Check telnet-server RPM is not installed
  # CIS 3.3 Check avahi-daemon is not enabled
  # CIS 3.4 Check cups is not enabled
  # CIS 3.5 Check dhcp RPM is not installed
  # CIS 3.6 NTP config
  # CIS 3.7.1 Check LDAP RPMs are not installed
  # CIS 3.8 Check NFS and RPC are not enabled
  # CIS 3.9 Check bind RPM is not installed
  # CIS 3.10 Check vsftpd RPM is not installed
  # CIS 3.11 Check httpd RPM is not installed
  # CIS 3.12 Check dovecot RPM is not installed
  # CIS 3.13 Check samba RPM is not installed
  # CIS 3.14 Check squid RPM is not installed
  # CIS 3.15 Check net-snmp RPM is not installed
  # CIS 3.16 MTA in local-only mode
  # CIS 4.1.1 IP Forwarding should be disabled
  # CIS 4.1.2 Send Packet Redirects should be disabled
  # CIS 4.2.1 Source Routed Packet Acceptance should be disabled
  # CIS 4.2.2 ICMP Redirect Acceptance should be disabled
  # CIS 4.2.3 ICMP Redirect Acceptance should be disabled
  # CIS 4.2.4 Log Suspicious Packets
  # CIS 4.2.5 Ignore Broadcast Requests should be enabled
  # CIS 4.2.6 Bad Error Message Protection should be enabled
  # CIS 4.2.7 RFC-recommended Source Route Validation should be enabled
  # CIS 4.2.8 TCP SYN Cookies should be enabled
  # CIS 4.3.1 Check Wireless Interfaces are deactivated
  # CIS 4.4.1.1 If IPv6 enabled IPv6 Router Advertisements should be disabled
  # CIS 4.4.1.2 If IPv6 enabled IPv6 Redirect Acceptance should be disabled
  # CIS 4.4.2 IPv6 disabled
  # CIS 4.5.1 Check that TCP Wrappers are installed
  # CIS 4.5.2 Check that /etc/hosts.allow exists
  # CIS 4.5.3 Verify permissions on /etc/hosts.allow
  # CIS 4.5.4 Check that /etc/hosts.deny exists
  # CIS 4.6.1 Check that CIS.conf file should disable uncommon network protocol dccp 
  # CIS 4.6.2 Check that CIS.conf file should disable uncommon network protocol sctp 
  # CIS 4.6.3 Check that CIS.conf file should disable uncommon network protocol rds 
  # CIS 4.6.4 Check that CIS.conf file should disable uncommon network protocol tipc 
  # CIS 4.7 Firewalld should be enabled
  # CIS 5.1.1 Check that rsyslog is installed
  # CIS 5.1.2 rsyslog should be enabled
  # CIS 5.1.3 Configure rsyslog.conf
  # CIS 5.1.4 Check perms on rsyslog.conf
  # CIS 5.1.5 rsyslog.conf sending logs to a remote host
  # CIS 5.1.6 This benchmark is only applicable to rsyslog loghosts
  # CIS 5.2.1.1 Audit Log Storage Size should be configured
  # CIS 5.2.1.2 Disable System on Audit Log Full
  # CIS 5.2.1.3 Disable System on Audit Log Full
  # CIS 5.2.2 auditd should be enabled
  # CIS 5.2.4 Record events that modify date & time info
  # CIS 5.2.5 Record events that modify user & group info
  # CIS 5.2.6 Record events that modify the system's network env
  # CIS 5.2.7 Record events that modify the system's Mandatory Access Controls
  # CIS 5.2.8 Verify Collection Login and Logout events is configured
  # CIS 5.2.9 Verify Collection of Session Initiation info is configured
  # CIS 5.2.10 Verify Collection of Discretionary Access Control permission modification events
  # CIS 5.2.11 Verify collection of unsuccessful unauthorized access attempts to files
  # CIS 5.2.12 Verify collection of privileged commands
  # CIS 5.2.13 Verify collection of privileged commands
  # CIS 5.2.14 Verify collection of privileged commands
  # CIS 5.2.15 Verify collection of privileged commands
  # CIS 5.2.16 Verify collection of privileged commands
  # CIS 5.2.17 Verify collection of Kernel Module Loading and Unloading
  # CIS 5.2.18 Verify collection of Kernel Module Loading and Unloading
  # CIS 5.3 Log rotate should be configured
  # CIS 6.1.1 cron and anacron config
  # CIS 6.1.2 enable crond daemon
  # CIS 6.1.3-6.1.8 user/group owner and perms
  # CIS 6.1.10 at daemon config
  # CIS 6.1.11 restrict at/cron to authorized users
  # CIS 6.2.1 SSH protocol should be 2
  # CIS 6.2.2 LogLevel to INFO
  # CIS 6.2.3 Permissions on sshd_config
  # CIS 6.2.4 SSH X11Forwarding 
  # CIS 6.2.5 SSH MaxAuthTries 
  # CIS 6.2.6 SSH X11Forwarding 
  # CIS 6.2.7 SSH HostbasedAuthentication
  # CIS 6.2.8 SSH PermitRootLogin
  # CIS 6.2.9 SSH PermitEmptyPasswords
  # CIS 6.2.10 SSH PermitUserEnvironment
  # CIS 6.2.11 SSH Ciphers
  # CIS 6.2.12 SSH Idle Timeout Interval for User Login
  # CIS 6.2.13 Limit access to SSH
  # CIS 6.2.14 SSH banner
  # CIS 6.3.1 SHA-512 password hashing algorithm
  # CIS 6.3.2 password creation requirement parameters using pam_pwquality
  # CIS 6.3.3 Set lockout for failed password attempts
  # CIS 6.3.4 Limit password reuse
  # CIS 6.4 Restrict root login to system console
  # CIS 6.5 Restrict access to su
  # CIS 7.1.1 Password expiration days
  # CIS 7.1.2 Password change minimum number of days
  # CIS 7.1.3 Password expiring warning days
  # CIS 7.2 Disable System Accounts
  # CIS 7.3 Default group for root account
  # CIS 7.4 Default group for root account
  # CIS 7.5 Inactive User accounts should be locked
  # CIS 8.1 user/group owner and perms on 
  # CIS 8.2 OS Information should not be in Login Warning Banners
  # CIS 8.3 Set GNOME Warning Banner
  # CIS 9.1.2 Verify perms on /etc/passwd 
  # CIS 9.1.3 Verify perms on /etc/shadow 
  # CIS 9.1.4 Verify perms on /etc/gshadow 
  # CIS 9.1.5 Verify perms on /etc/group 
  # CIS 9.1.6-9 user/group owner and perms on /etc/passwd /etc/shadow /etc/gshadow /etc/group
  # CIS 9.1.10 Shouldn't have any world writable files
  # CIS 9.1.11 Shouldn't have any unowned files & dirs
  # CIS 9.1.12 Shouldn't have any ungrouped files & dirs
  # CIS 9.1.13 Check for suid executables
  # CIS 9.1.14 Check for sgid executables
  # CIS 9.2.1 Ensure password fields are not empty
  # CIS 9.2.2 Verify no legacy "+" entries exist in /etc/passwd
  # CIS 9.2.3 Verify no legacy "+" entries exist in /etc/shadow
  # CIS 9.2.4 Verify no legacy "+" entries exist in /etc/group
  # CIS 9.2.5 Verify no UID 0 accounts exist other than root
  # CIS 9.2.6 Ensure root PATH integrity
  # CIS 9.2.7 Home dir perms
  # CIS 9.2.8 User dot file permissions
  # CIS 9.2.9 User .netrc permissions
  # CIS 9.2.10 User .rhosts files
  # CIS 9.2.11 User .rhosts files
  # CIS 9.2.12 User .rhosts files
  # CIS 9.2.13 Check home directory ownership
  # CIS 9.2.14 Check for Duplicate UIDs in /etc/passwd
  # CIS 9.2.15 Check for Duplicate GIDs in /etc/group
  # CIS 9.2.16 Check that reserved uids are assigned 
  # CIS 9.2.17 Check for Duplicate usernames in /etc/passwd
  # CIS 9.2.18 Check for Duplicate groupnames in /etc/group
  # CIS 9.2.19 Check for presence of user .netrc files
  # CIS 9.2.20 Check for presence of user .forward files

Questions, suggestions, critique? pipe them to inbox2alfie(gmail)

