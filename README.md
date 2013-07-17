supybot-plugin-pumpqt
=====================

plugin for supybot to quote a channel message to Pump.io
This should quote a user, then post the quote to Pump.io, and then allow more options later.


## Requirements ##
- nodejs in order to run the pump bin files
- you should run authorize yourself first like below

## Settings ##
    pumpPathToBin = 'pumpbin'
        #link to your pump files, or leave this to use included files
    pumpUser = 'foo'
    pumpServer = 'microca.st'
    pumpPort = '443'

## Authorization ##
    pump-register-app -s microca.st -P 443 -t CLI
    pump-authorize -s microca.st -P 443 -u username

## Test note ##
    pump-post-note -s microca.st -P 443 -u username -n "Hello World!"
