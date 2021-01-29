# Role Name:  settime
***
* Install and configure chrony

## Requirements
***
None.

## Role Variables
***
|Variable           |Required|Default|Choices   |Comments           |
|-------------------|--------|-------|----------|-------------------|
|package            |yes     |false  |Package   |chrony             |
|chrony_conf_file   |yes     |false  |Path      |/etc/chrony.conf   |
|chrony_service_name|yes     |false  |Service   |chronyd            |
|chrony_pool        |no      |false  |Pool      |2.pool.ntp.org     |
|chrony_server      |no      |false  |Server    |cronos.cenam.mx    |
|chrony_allow       |no      |false  |CIDR Block|192.168.100.0/24   |


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
