# Role Name:  Common
***
* Configure hostname
* Configure /etc/hosts file
* Update OS
* Set time and location configuration

## Requirements
***
None.

## Role Variables
***
|Variable  |Required|Default|Choices |Comments   |
|----------|--------|-------|--------|-----------|
|hostname  |yes     |false  |Hostname|test       |
|domain    |yes     |false  |Domain  |example.com|
|hosts_file|yes     |false  |Service |/etc/hosts |  


## Dependencies
***
* None.

## Example Playbook
***
```yaml
- hosts: all
  roles:
    - common
```
## License
***
Created by Sinko only for learning proposes
## Author information
***
Armando Reyes Galicia
