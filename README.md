# Reverse Engineered Relay Board

This is the schematic for common 5VDC operated relay board commonly found on
Ebay. The power select jumper is an odd one, it bridges external voltage and
ground. I'm not sure why these boards were designed this way. There is no way
for this board to function unless the jumper is bridged between `VCC` and
`JD-VCC`.

To use this board hook up `EXT_PWR-` to your circuit's ground, `EXT_PWR+` to
`+5V` in your circuit. Each control pin `CTRL1` through `CTRL8` need to be
brought to ground (`EXT_PWR1`) to activate the associated relay.

## Parts

* The transistors are labelled `G1` and appear to be some generic NPN version
* The relays on my specific board are labelled `JQC-3FF-S-Z` but I have
  previously gotten these boards with `SRD-05VDC-SL-C`.
* The photocoupler relays are labelled `DP-817C-1650`

Other values are in the schematic.
