# modou gem

Your modouwifi CLI.

Built based on [Modou HTTP API](https://github.com/modouwifi/modouwifi-api)

Work in process.

[![Build Status](https://travis-ci.org/modouwifi/modou-gem.svg?branch=master)](https://travis-ci.org/modouwifi/modou-gem)
[![Code Climate](https://codeclimate.com/github/modouwifi/modou-gem/badges/gpa.svg)](https://codeclimate.com/github/modouwifi/modou-gem)

## Installation

Add this line to your application's Gemfile:

    gem 'modou'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install modou

## Usage

available commands:

#### show version info

    modou version

output:

```
Firmware Version: 0.6.04_beta4
Hardware Version: m101c
Firmware Track:   inter
```

#### check for update

    modou update_check

#### download firmware

    modou download_firmware

#### upgrade system

    modou upgrade

#### reboot

    modou reboot

#### reboot into safe mode

    modou safe_reboot

#### show client MAC address

    modou client_mac

#### test Internet connectivity

    modou internet_test

#### show wired connections

    modou wired_connections

output:

```
+------+-------+
| lan1 | false |
| lan2 | true  |
| code | 0     |
| wan  | false |
| usb  | false |
+------+-------+
```

#### show system time of router

    modou system_time

#### show flash info

    modou flash_info

output:

```
+------------------+-----------------+
| ddr2_total_size  | 127999.99904633 |
| ddr2_remain      | 72420           |
| flash_remain     | 48256           |
| flash_total_size | 128000          |
+------------------+-----------------+
```

### firmware

    modou firmware info

    modou firmware check

    modou firmware download

    modou firmware upgrade

### backlight control

    modou backlight lock

    modou backlight unlock

    modou backlight wakeup

### security

    modou security info

    modou security on

    modou security off

### WAN

    modou wan info

    modou wan traffics

### Wi-Fi

    modou wifi info

    modou wifi enabled

### LAN

    modou lan info

### disk

    modou disk info

    modou disk eject

### devices

    modou devices wired

    modou devices wifi

    modou devices whitelisted

    modou devices blacklisted

    modou devices graylisted

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
