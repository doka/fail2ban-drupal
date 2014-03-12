fail2ban-drupal
===============

Fail2Ban filters for Drupal

#### Prerequisites
Drupal and Fail2ban should be installed and setup.
Root access to your host.

#### Usage
1. Copy the `.conf` files into `/etc/fail2ban/filter.d` and add the content of `drupal-jail.local` to the end of your `/etc/fail2ban/jail.local` file. 

2. Reload fail2ban by 
`service fail2ban force-reload`

#### Results
According to the pattern in the `.conf` files, IP addresses are getting blocked for a while. It results in less load on your Drupal host, and more secure Drupal installs. See particular result in your log file:
`tail -f /var/log/fail2ban.log`
