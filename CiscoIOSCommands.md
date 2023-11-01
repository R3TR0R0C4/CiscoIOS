-Entrem al mode privilegiat EXEC

`enable`

-Entrem al mode de configuració global

`configure terminal` o `conf t`

-Entrem a la configuració d'intefície (física o vlan)

`interface [interface_type] [interface_number]`

-Assignem IP i Màscara

`ip address [ip_address] [subnet_mask]`

-Configurem el hostname del dispositiu:

`hostname [hostname]`

-Configurem una contrasenya amb hash (veurem un hash amb un running config) pel mode EXEC:

`enable secret [password]`

-Configurem una contrasenya amb text pla (veurem la contrasenya amb text pla amb un running config) pel mode EXEC:

`password [password]`

-Entrem a la configuració de les línies virtuals (Telnet o SSH)

`line vty 0 15`

-Entrem a la configuració de les línies físiques (Cable de consola)

`line console 0`

enable password [password] (in line configuration mode):

Explanation: Sets the enable password for accessing privileged exec mode through a specific line (e.g., console or vty). This password is stored in plain text.
show running-config:

Explanation: Displays the current running configuration of the router, showing all the settings and configurations that are currently in effect.
show ip interface brief:

Explanation: Provides a brief overview of all the router's interfaces and their current IP addresses and status.
ping [ip_address]:

Explanation: Used to send ICMP echo requests to test connectivity to a specific IP address. It's a useful diagnostic tool for network troubleshooting.
traceroute [ip_address]:

Explanation: Traces the route that packets take from the router to a destination IP address, showing each hop along the way.
copy running-config startup-config or write memory:

Explanation: Saves the current running configuration to the startup configuration, ensuring that the changes persist after a reboot.
erase startup-config:

Explanation: Erases the startup configuration, effectively resetting the router to its default settings.
reload:

Explanation: This command is used to reboot the router, applying any configuration changes that have been made but not saved.
These are some of the basic Cisco IOS commands that are commonly used to configure and manage Cisco routers. Please note that the actual command syntax may vary depending on the router model and IOS version in use.
