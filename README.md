# hsrp pack for shinken-monitoring.org 
This is just a small collection of commands and services for using the already provided modes from [check\_nwc\_health](http://labs.consol.de/nagios/check_nwc_health/)

# installation 
Just download it as a zip or clone it, then put the contents of this folder into your shinkens packs folder as follows:

    etc/packs/network/hsrp
    
You should then be able to tell your switch host that has hsrp configured like this:

    define host{
        use    cisco,switch,hsrp
        ...
    }

# what it does
The three provided commands are ```check_hsrp_state```, ```check_hsrp_failover``` and ```check_list_hsrp_groups```. They all are exact copies from the already mentioned excellent ```check_nec_health``` plugin for nagios.

# hope it helps
if not, reach me on twitter: @kjellski
