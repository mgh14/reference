# Python

## Files:
`file=open("/path/here.wav", 'rb')`
  - 'rb': read + binary
  - 'r' : read (strings only)?
file.close()

## Struct: https://docs.python.org/3/library/struct.html
```
import struct;
struct.unpack(<format>, <bytes>)
    e.g. struct.unpack('<h', a+b)
```

## .Wav specific: 
import wav  # Note: only reads PCI audio or something

`myWav = wav.open("/path/here.wav")`

`myWav.getparams() # gets basic file info`

`myFrame=myWav.readFrames(<number of frames>)`
    len(myFrame)=6 # ??

`myWav.rewind()`
