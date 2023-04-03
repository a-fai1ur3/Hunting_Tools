## Whois
WHOIS (pronounced as the phrase "who is") is a query and response protocol that is widely used for querying databases that store the registered users or assignees of an Internet resource, such as a domain name, an IP address block or an autonomous system, but is also used for a wider range of other information.The protocol stores and delivers database content in a human-readable format. [Read more on Wikipedia](https://en.wikipedia.org/wiki/WHOIS)

    # whois -h
    whois: option requires an argument -- 'h'
    Usage: whois [OPTION]... OBJECT...

    -h HOST, --host HOST   connect to server HOST
    -p PORT, --port PORT   connect to PORT
    -I                     query whois.iana.org and follow its referral
    -H                     hide legal disclaimers
          --verbose        explain what is being done
          --help           display this help and exit
          --version        output version information and exit

    These flags are supported by whois.ripe.net and some RIPE-like servers:
    -l                     find the one level less specific match
    -L                     find all levels less specific matches
    -m                     find all one level more specific matches
    -M                     find all levels of more specific matches
    -c                     find the smallest match containing a mnt-irt attribute
    -x                     exact match
    -b                     return brief IP address ranges with abuse contact
    -B                     turn off object filtering (show email addresses)
    -G                     turn off grouping of associated objects
    -d                     return DNS reverse delegation objects too
    -i ATTR[,ATTR]...      do an inverse look-up for specified ATTRibutes
    -T TYPE[,TYPE]...      only look for objects of TYPE
    -K                     only primary keys are returned
    -r                     turn off recursive look-ups for contact information
    -R                     force to show local copy of the domain object even
                           if it contains referral
    -a                     also search all the mirrored databases
    -s SOURCE[,SOURCE]...  search the database mirrored from SOURCE
    -g SOURCE:FIRST-LAST   find updates from SOURCE from serial FIRST to LAST
    -t TYPE                request template for object of TYPE
    -v TYPE                request verbose template for object of TYPE
    -q [version|sources|types]  query specified server info


## Use Cases - 

#### Simple Command usage : use IP or domain name --
    whois [IP|Domain]
#### Want to take the output into a file --
    whois [IP] > output.txt
#### Use IP address instead of the domain name for some extra information --
    whois [IP]
#### For query specificnformation use --
    whois -q version [IP]
    whois -q types [IP]

### Additional Resource --
 [Whois](https://who.is/)
