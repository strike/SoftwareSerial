SoftwareSerial
==============

SoftwareSerial -- library for arduino. 
In this modification you can use flash (programm) memory for print. You can you _P function (write_P, writeln_P) or usual function (write, writeln). 

USEGE
------

```cpp
#include <avr/pgmspace.h>
...

SoftwareSerial mySerial(10, 11); // RX, TX

void someFunction(){
  mySerial.begin(4800);
  ...
  // print flash string
  mySerial.writeln(F("Hello, world?"));
  // or 
  mySerial.writeln_P(F("Hello, world?"));
  ...

}

```
