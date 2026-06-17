*** 0.52 ***
- Fix "UPS OK" (safety) binary_sensor inverted: a healthy UPS (UpsOk=on) was
  mapped to the safety "on" state and displayed as "Unsafe/Inseguro". Swapped
  payload_on/payload_off in device.json so healthy = Safe/Seguro.

*** 0.51 ***
- Fix crash/restart loop on serial errors: ser.is_open is a property in
  pyserial 3.x, not a method. Calling ser.is_open() inside the serial
  exception handlers raised "TypeError: 'bool' object is not callable",
  turning a recoverable serial hiccup into a fatal crash.

*** 0.42 *** 
- Fix Device-tree error 

*** 0.41 *** 
- Some serial improvements
- Some bugs
- removed webserver
- amd64-base-python:3.9-alpine3.12 bug - now using 3.9-alpine3.14
- Folders new config

*** 0.40 *** 
- alpine3.122 correction.
  
*** 0.39 *** 
- Sensors now are "state_class":"measurement"
- No need to config MQTT user and password.
- Estimated Power Use (BETA)

*** 0.38 *** 
- fix returned a non-zero code on install
- Alpine 3.13 bug - now using 3.12

