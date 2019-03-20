# Python Temperature logger for raspberry pi
A simple script running on some raspberry pies at the office for logging temperature changes over time.


**Equipment**: 
* 18B20 - Temperature sensor (+/- 0.5c)
* 4.7k resistor between data and the power pin (pullup)
* Raspberry Pi 3 B+

**Crontab**:
`0,20,40 * * * * /usr/bin/python3 /home/pi/templogger.py > /home/pi/templogger.log`
*We are loggint to `templogger.log` just so that we can take a look at the latest run result if we ever encounter issues*

**Overkill**: Yes

**Why rPI**: Quickest thing at hand with an ethernet connector

**How its running**: 
on Rasbian with Crontab logging at 0,20 and 40 minute mark of every hour. 

### Before use
*Change Private key and channel ID*
Change the field to match what field your using on your own channel. 
For each sensor you setup with the same channel, just change the field number. 
