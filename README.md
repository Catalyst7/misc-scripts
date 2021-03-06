misc-scripts
=============

This is a collection of miscellaneous scripts that I've written or modified
for my use. Hopefully they may be of some use to others. When I get a chance,
I'll try and update this readme with descriptions of all of the scripts.

Unless otherwise noted, these are distributed under the terms of the LICENSE
file.

* __apache_log_verify_site_move.py__ - Python script that parses Apache HTTPD access logs, finds all unique URLs, and compares the current HTTP response code to that of another server. Useful when moving a site.
* __bigipcookie.pl__ - Perl script to de/encode F5 BigIp persistence cookies.
* __check_url_list.py__ - Script to check a list of URLs (passed on stdin) for response code, and for response code of the final path in a series of redirects.
* __cmd-wrapper.c__ - C wrapper for a setuid/gid command, to ensure that ONLY a certain command and args can be run.
* __collectRsyslogInfo.php__ - Script to collect information on a crashed/hung rsyslogd process, and log it all somewhere.
* __dot_find_cycles.py__ - uses Pydot and NetworkX to find cycles in a dot file directed graph (i.e. the graph output of Puppet)
* __dumpFirefoxSession.php__ - Script to dump all URLs from a Firefox3 sessionstore.js file as text or HTML
* __dumpMysqlGrants.sh__ - Script to dump all grants from a MySQL server, for input into another.
* __dump_skype_logs.py__ - Script to dump all Skype logs from a main.db file to HTML
* __find_outdated_puppets.py__ - Script to look at a Puppet Dashboard unhidden-nodes.csv and extract the latest report time for each node, optionally, list nodes with runtime BEFORE a string.
* __git_repo_diff.py__ - uses GitPython to compare 2 git repo clones and report on branches that only exist in one, or have different head commits in the two repos
* __htmldata.py__ - Perl library to manipulate HTML or XHTML documents, required by mw2html-auth
* __increment_zone_serial__ - This script updates/increments the bind zone file serial number in a file specified as the first argument
* __ismerged__ - shell script that takes a git branch name, and tells if it is merged into master or not
* __js2phpdoc.php__ - script to take comments and function prototypes from JS files and make them PHP-ish to be parsed by phpdoc
* __kickRsyslog.php__ - script to restart rsyslog if it appears to have stopped logging
* __libvirt_csv.py__ - Use libvirt python bindings to print CSV lists of dom0_host,domU_name,ID,state,UUID for all qemu+kvm VMs running on libvirt hosts passed in as arguments
* __LICENSE__ - License for these files - GPLv3 with additional provisions
* __linode_ddns_update.sh__ - simple script to use Linode's HTTP API to update Linode DNS for a dynamic IP
* __linodeDnsToCsv.php__ - Script to pull DNS information for all of your Linode hosted zones, output as CSV
* __linode_list_records.py__ - Simple script to list all records in Linode DNS via API, along with their type, DomainID and ResourceID
* __list_github_org_repos.py__ - List information about an org's repositories using PyGithub (GitHub API library)
* __mw2html-auth__ - Produce an HTML version (standalone backup/export) of a MediaWiki site that's behind authentication
* __nagios_log_problem_interval.pl__ - Chart intervals between problem and recovery from Nagios/Icinga logs
* __nmap-xml-to-table.php__ - Script to transform multiple nmap XML output files (presumably of the same host/port range with different scan options) into a HTML table
* __print-cmd.sh__ - Simple script to log environment variables and original command for forced ssh commands
* __print-cmd-wrapper.c__ - C wrapper like cmd-wrapper.c, but just echoes back the command that was called
* __README.VCS__ - Note on my CVS/SVN to github migration
* __rebuild_srpm.sh__ - Script to rebuild a SRPM 1:1, useful when you want to build a RHEL/CentOS 6 SRPM on a RHEL/CentOS 5 system that doesn't support newer compression (cpio: MD5 sum mismatch)
* __rss_to_mail_config.py__ - sample configuration file for rss_to_mail.py
* __rss_to_mail.py__ - Dead simple python script to find new entries in an RSS feed, and email listing of new entries matching a regex to you. Intended to be run via cron.
* __rsync-wrapper.c__ - setuid/gid wrapper around rsync. Useful to allow members of a specified group to do rsync backups as root over SSH.
* __rsyslogIsHung.php__ - script to investigate rsyslog hangs, write output, and send mail
* __rsyslogPstats.php__ - script to parse rsyslog impstats output and generate a simple report
* __scrape_domain.py__ - Python script using requests and BeautifulSoup4 to request all URLs/links/images/CSS/feeds/etc. found on a domain.
* __show_dhcp_fixed_ACKs.pl__ - script to show the most recent DHCP ACKs per IP address for ISC DHCPd, from a log file. Originally written for Vyatta routers that just show the dynamic leases
* __simpleLCDproc.py__ - Simple LCDproc replacement in Python. Uses LCDd server.
* __syslogAgeChecker.php__ - script to check timestamp of last syslog line in some files, and send mail if >= X seconds
* __syslogDatesGraph.php__ - script to help visualize time distribution of syslog messages. This is the graph host part.
* __syslogDatesToArray.php__ - script to help visualize time distribution of syslog messages. This is the log host part.
* __syslogDatesToArray-sample.ser__ - example serialized data for syslogDatesGraph.php
* __test_libvirt.py__ - some tests using the libvirt python bindings, for qemu+kvm hosts accessed over SSH
* __timeout__ - shell script to execute a command with a timeout
* __ubiquiti-mac-acl/__ - PHP script and MySQL schema to manage the MAC ACL on Ubiquiti AirOS2 devices.
* __VipToInternalHosts.pl__ - script to take F5 BigIp VIP address and display the members of the pool it is served by
* __wiki-to-deckjs.py__ - simple, awful script to change markdown-like (very restricted markup set) markup to deck.js-ready html
* __wordpress_daily_post.php__ - Script to publish the oldest post with a given status, if no other post has been published in 24 hours. Intended to be run via cron on weekdays
