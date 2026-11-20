# URQ Detector

A code snippet in URQL for the URQ engine family that detects the player/interpreter used to run the game.

## Supported URQ Players

This snippet has been adapted and tested for use with the following URQ players:

* RipURQ version 1.4
* URQ_DOS version 1.35
* AkURQ version 1.28
* FireURQ version 2.2.4
* URQ Module of INSTEAD version 2
* UrqW version 2.0

## Usage

1. Insert the urq_detector code block from the urq_detector.qst file into your URQ game.
2. Call it as a procedure when the game starts:
	```
	proc urq_detector
	```
3. Use the values ??of the is* numeric variables later in the code to implement logic depending on the detected player.

For demonstration and testing purposes, the urq_detector.qst file contains a working example that can be run as a standalone game in a URQ player.

Please note that RipURQ does not support implicit boolean conversion in conditions. When targeting RipURQ use explicit comparison:

```
if isRipURQ=1 then pln The file is running in RipURQ.
```

Others players also support:

```
if isDosURQ then pln The file is running in URQ_DOS.
```

## License

URQ Detector - a code snippet in URQL

Written in 2026 by Nikita Tseykovets

To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to the software and the text contained therein to the public domain worldwide. the software and the text contained therein are distributed without any warranty.

You should have received a copy of the CC0 Public Domain Dedication along with the software and the text contained therein. If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
