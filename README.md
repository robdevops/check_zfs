# check_zfs
check_zfs plugin for Nagios / Icinga. Checks for degraded zfs pools.

## Dependencies
* bash
* zfs
* coreutils

## Installation
1. Copy the script to /usr/local/sbin/check_zfs
1. Use chown and chmod to ensure the test user can execute it.
1. Give the test user sudo access:
```
visudo 
```
```
icinga ALL=(root) NOPASSWD: /usr/local/sbin/check_zfs
``` 

## Usage
```
/usr/local/sbin/check_zfs
```

### Example output
```
sudo /usr/local/sbin/check_zfs
OK: all pools are healthy.
```
```
echo $?
0
```
