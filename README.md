# Weatherstation
Sensor BME280
Can someboy help me with the code for this sensor
we use it with a raspberry pi 3b and get the following fould
bme280 sensor

pi@raspberrypi:~ $ i2cdetect -y 1
0 1 2 3 4 5 6 7 8 9 a b c d e f
00: -- -- -- -- -- -- -- -- -- -- -- -- -- 
10: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
20: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
30: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
40: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
50: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
60: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- 
70: -- -- -- -- -- -- -- 77 
pi@raspberrypi:~ $ python bme280.py
Traceback (most recent call last):
File "bme280.py", line 168, in <module>
main()
File "bme280.py", line 157, in main
(chip_id, chip_version) = readBME280ID()
File "bme280.py", line 56, in readBME280ID
(chip_id, chip_version) = bus.read_i2c_block_data(addr, REG_ID, 2)
IOError: [Errno 5] Input/output error

