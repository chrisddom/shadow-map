ShadowMap is a utility for mapping shadow copies, allowing them to be queried and compared.

# [Standalone Application 1.2](http://code.google.com/p/shadow-map/downloads/detail?name=shadowmap_executable_1_2.zip&can=2&q=#makechanges) #
[Documentation](http://code.google.com/p/shadow-map/downloads/detail?name=Help.pdf&can=2&q=) [Sourcecode](http://code.google.com/p/shadow-map/downloads/detail?name=source_code_1_2.zip&can=2&q=#makechanges)


## How it works ##
The tool works by:
  * Mounting all shadow copies
  * Running the tool ftimes to create detailed maps of specified locations (shadow copy volumes, folders, original volumes etc.)
  * Importing these maps into a SQLLite database for fast and detailed querying
  * Running ftimes for comparison


## Mounting Images ##
Unfortunately, the only tool capable of mounting images in a manner that the volume shadow copy service can access them appears to be the commercial Encase suite. Therefore the included ImDisk drivers will not mount images in a manner suitable for mounting shadow copies.


## Tools used ##
  * IMDisk 1.5.7 http://www.ltr-data.se/opencode.html/#ImDisk
  * Ftimes 3.9 http://ftimes.sourceforge.net/FTimes/Man+Pages/ftimes.shtml
  * Makes use of vssadmin and fc tools installed with Windows Vista and later
  * Code from http://pastebin.com/81iHJ5C8 was used for interacting with shadow copies

## About ##
Created by Christopher Doman (http://www.christopherdoman.com) for the DC3 Forensics Challenge 2012 (http://www.dc3.mil/challenge/2012). Created on quite a short schedule, so please consider this beta software and inform me of any bugs.

![http://shadow-map.googlecode.com/files/shadow.png](http://shadow-map.googlecode.com/files/shadow.png)