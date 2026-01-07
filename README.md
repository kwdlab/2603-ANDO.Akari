## 2603-ANDO.Akari
2026年3月卒業　安藤朱里

## Overview

This project investigates the effect of data compression on log transfer time in rsyslog using UDP and TCP.  

The amount of data sent during log transmission is measured by modifying the rsyslog forwarding module.



## Description

In this study, rsyslog was used to compare log transfer behavior between UDP and TCP with and without compression.  

The forwarding module (omfwd.c) was modified to output the number of bytes sent during log transmission.



Log transfer experiments were conducted using two hosts:

one acting as a log sender and the other as a log receiver.



## Files

- rsyslog_sender.conf: Configuration file used on the sender host.

- rsyslog_receiver.conf: Configuration file used on the receiver host.

- omfwd.c: Modified source file of the rsyslog forwarding module to confirm the number of bytes sent during log transmission.



## Requirement

- rsyslog (built from source)



## Usage

After building and installing rsyslog from source, log transfer experiments were performed using the logger command with four patterns: UDP/TCP and with/without compression.



## Author

Akari Ando



## License

- rsyslog GPLv2 License: https://github.com/rsyslog/rsyslog/blob/main/COPYING


## References

- rsyslog GitHub repository: https://github.com/rsyslog/rsyslog

