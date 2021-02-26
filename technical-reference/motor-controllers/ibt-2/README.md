The IBT-2 (or IBT_2) is a small, external board consisting of 2 BTS7960 chips (each a half H-Bridge) designed to handle high current.

What we know about the board:

* Can handle our current needs. Rated to over 40A, realistically can do 30 or so. We will only allow 5A and possibly 10
* Has a current sense on each chip, but from chip to chip, the tolerance can vary wildly, so even on the same board, chip A can show different current than chip B
* We typically tie both sense pins together and connect them to an analog pin (usally A5) on the Arduino. With a 10k sense resistor for each chip, that is a 5k sense resistance.
* The "nominal" value for current sense in the 5A range is 1/8500th of the load current. This can be anywhere from 1/3000th to 1/14000th though!
