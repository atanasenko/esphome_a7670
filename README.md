# esphome_a7670
An implementation to talk to A7670X (possibly others as well) modems for esphome that is heavily based on sim800l component, but solves some problems

* Allows it to work on lilygo's t-eth-elite + t-eth-elite-lte shield as these need to wake modem up using a power pin
* Supports setting pin code
* Incoming and outgoing SMS messages are processed in PDU mode which allows full unicode support (courtesy of https://github.com/mgaman/PDUlib)
* Fixes stability issues caused by modem responses coming asynchronously
* Other minor imporovements
