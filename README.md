# Python Temperature logger for raspberry pi
A simple script running on some raspberry pies at the office for logging temperature changes over time.


Equipment: 
* 18B20 - Temperature sensor (+/- 0.5c)
* Raspberry Pi 3 B+

Overkill: Yes
Why: Quickest thing at hand with an ethernet connector

How its running: 
on Rasbian with Crontab logging at 0,20 and 40 minute mark of every hour. 

### Before use
*Change Private key and channel ID*
Change the field to match what field your using on your own channel. 
For each sensor you setup with the same channel, just change the field number. 
