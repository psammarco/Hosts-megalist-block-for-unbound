### Hosts block megalist formatted for Unbound DNS Server and made available to you with love.

As of today *26/08/2017*, this list has been tested with Unbound's version *1.6.2 / 1.6.3* and *IPFire 2.19 Core Update 111 / 112*. 

For the time being I don't really have an update release schedule in mind, however I will monitor the below enties lists and will update it as soon as something worthwhile comes up.

Consider that maintaining it, keeping it updated and clean takes serveral hours of my spare time. If you like my work, please feel free to share any thoughts and feedbacks.

### Total blocked entries 101880

*This megalist is a combination of hosts and IPs entries from:*

 - https://adguard.com/en/filter-rules.html?id=15
 - http://someonewhocares.org/hosts/hosts
 - https://adaway.org/hosts.txt
 - http://winhelp2002.mvps.org/hosts.txt
 - http://hosts-file.net/ad_servers.txt
 - http://pgl.yoyo.org/adservers/serverlist.php?hostformat=hosts&showintro=0&mimetype=plaintext
 - http://www.malwaredomainlist.com/hostslist/hosts.txt
 - https://ransomwaretracker.abuse.ch/downloads/RW_DOMBL.txt
 - https://ransomwaretracker.abuse.ch/downloads/RW_IPBL.txt
 - https://www.eff.org/files/cookieblocklist.txt
 - https://raw.githubusercontent.com/FadeMind/hosts.extras/master/SpotifyAds/hosts
 - https://www.hosts-file.net/download/hosts.txt
 - https://filtri-dns.ga/filtri.txt
 - https://www.malwaredomainlist.com/hostslist/hosts.txt
 - https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/porn/hosts

*Note:* In order to use it you will need to add the following ~~two~~ line to your unbound.conf file and within the *"server"* section 

~~`access-control: 0.0.0.0/8 allow`~~

`include: /path/to/block.conf`

once than that, save and restart unbound

`/etc/init.d/unbound restart`

Enjoy.
