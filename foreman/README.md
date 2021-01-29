# Role Name:  Foreman
***
* Install Foreman
* Install Katello scenario
* Enable Foreman Plugins

## Requirements
***
|     OS         |OS Version|Mininum CPU|Mininum RAM|Minimum HDD         |
|----------------|----------|-----------|-----------|--------------------|
|CentOS          |7         |1 vCPU     | 8GB       |/var/lib/pulp/ 30GB |

## Role Variables
***
|Variable       |Required|Default|Choices       |Comments          |
|---------------|--------|-------|--------------|------------------|
|hostname       |yes     |false  |Short hostname|foreman           |
|domain         |yes     |false  |Domain        |example.com       |
|foreman_plugins|yes     |false  |Plugin name   |katello           |
|gpgkeys        |yes     |false  |RPM GPG Key   |RPM-GPG-KEY-EPEL-7|
|repositories   |yes     |false  |Repository    |epel-release      |
|packages       |yes     |false  |Package       |foreman-installer |
|firewall_ports |yes     |true   |Port/Protocol |53/udp            |


## Dependencies
***
* settime

## Example Playbook
***
```yaml
- hosts: all
  roles:
    - ../settime
    - foreman
```
## License
***
Created by Sinko only for learning proposes
## Author information
***
Armando Reyes Galicia
