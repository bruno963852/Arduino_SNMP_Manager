# CHANGELOG for SNMP Manager For ESP8266/ESP32/Arduino

## 1.1.3

Focus: Increase robustness

- Better handling devices sending invalid packets in response to requests
- Better handling for receiving responses with OID that weren't requested
- Added DEBUG log messages to aid future troubleshooting. Just add extra defines `#define DEBUG` and/or `#define DEBUG_BER`
- Added support for using test data in `SNMPManager::receivePacket` to better support users experiencing issues

## 1.1.2

- Reduce max size of SNMP message on ESP8266 to address [reported issue](https://github.com/shortbloke/Broadband_Usage_Display/issues/4_) which triggered exception: `Exception 9: LoadStoreAlignmentCause: Load or store to an unaligned address`

# 1.1.1

- Improve OctetString handling for long stringds
- Handle OID > 50 characters

# 1.1.0

- Initial library release