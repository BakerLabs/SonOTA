- Operating System: WIndows 1803 17134.590 
- Python Version: 3.7 64 bit
- Sonoff model: basic
- Sonoff firmware version: 2.60 tried upgrade to 2.61 
- I have read the README, and understand that SonOTA does not work with the latest Sonoff firmware: 

Please also drag and drop the generated `debug_########.log` file onto the issue so it is attached.

Tried the following:
- Flashed out of box no pairing with eWelink app - fail
- Paired , upgraded firmware to 2.60 > 2.61 - fail
- Tried Sonota.exe method, tried Python method - fail

Failure was the same every time.  Phase one completed. Waited for SSID "FinalStage" to appear but it was never displayed.

IP Address of device 10.10.7.1 , my machine 10.10.7.2 when connecting to ITEAD network 



2019-03-09 08:47:50,072: DEBUG: Current IPs: ['192.168.0.150', '169.254.72.46', '192.168.0.193']
2019-03-09 08:47:53,555: INFO: Using the following configuration:
2019-03-09 08:47:53,558: INFO: 	Server IP Address: 192.168.0.193
2019-03-09 08:47:53,558: INFO: 	WiFi SSID: bakerlabs2
2019-03-09 08:47:53,558: INFO: 	WiFi Password: **********
2019-03-09 08:47:53,560: INFO: Platform: win32
2019-03-09 08:47:53,729: INFO: ** Now connect via WiFi to your Sonoff device.
2019-03-09 08:47:53,729: INFO: ** Please change into the ITEAD WiFi network (ITEAD-100001XXXX). The default password is 12345678.
2019-03-09 08:47:53,729: INFO: To reset the Sonoff to defaults, press the button for 7 seconds and the light will start flashing rapidly.
2019-03-09 08:47:53,729: INFO: ** This application should be kept running and will wait until connected to the Sonoff...
2019-03-09 08:48:36,199: DEBUG: Current IPs: ['192.168.0.150', '169.254.72.46', '10.10.7.2']
2019-03-09 08:48:36,372: DEBUG: ~~ Connection attempt
2019-03-09 08:48:36,372: DEBUG: >> HTTP GET /10.10.7.1/device
2019-03-09 08:48:36,405: DEBUG: << {
2019-03-09 08:48:36,420: DEBUG:     "apikey": "4ce96483-2367-43f3-9501-43ef156e40b5",
2019-03-09 08:48:36,422: DEBUG:     "deviceid": "10006987c3",
2019-03-09 08:48:36,432: DEBUG:     "accept": "post"
2019-03-09 08:48:36,432: DEBUG: }
2019-03-09 08:48:36,432: DEBUG: >> HTTP POST /10.10.7.1/ap
2019-03-09 08:48:36,432: DEBUG: >> {
2019-03-09 08:48:36,432: DEBUG:     "version": 4,
2019-03-09 08:48:36,432: DEBUG:     "serverName": "192.168.0.193",
2019-03-09 08:48:36,432: DEBUG:     "ssid": "bakerlabs2",
2019-03-09 08:48:36,432: DEBUG:     "password": "**********",
2019-03-09 08:48:36,432: DEBUG:     "port": 8443
2019-03-09 08:48:36,432: DEBUG: }
2019-03-09 08:48:36,817: DEBUG: << {
2019-03-09 08:48:36,817: DEBUG:     "error": 0
2019-03-09 08:48:36,827: DEBUG: }
2019-03-09 08:48:36,827: INFO: ~~ Provisioning completed
2019-03-09 08:48:36,827: INFO: Starting stage2...
2019-03-09 08:48:37,007: INFO: ** The IP address of <serve_host> (192.168.0.193) is not assigned to any interface on this machine.
2019-03-09 08:48:37,009: INFO: ** Please change WiFi network to bakerlabs2 and make sure 192.168.0.193 is being assigned to your WiFi interface.
2019-03-09 08:48:37,009: INFO: ** This application should be kept running and will wait until connected to the WiFi...
2019-03-09 08:49:33,159: DEBUG: Current IPs: ['192.168.0.150', '169.254.72.46', '192.168.0.193']
2019-03-09 08:49:33,172: INFO: ~~ Starting web server (HTTP port: 8080, HTTPS port 8443)
2019-03-09 08:49:33,218: INFO: ~~ Waiting for device to connect
2019-03-09 08:49:33,564: INFO: *** IMPORTANT! ***
2019-03-09 08:49:33,574: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:49:33,625: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:49:33,665: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:49:33,714: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:50:36,104: INFO: *** IMPORTANT! ***
2019-03-09 08:50:36,105: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:50:36,105: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:50:36,105: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:50:36,105: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:51:40,572: INFO: *** IMPORTANT! ***
2019-03-09 08:51:40,572: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:51:40,575: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:51:40,576: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:51:40,576: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:52:43,628: INFO: *** IMPORTANT! ***
2019-03-09 08:52:43,628: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:52:43,628: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:52:43,628: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:52:43,628: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:53:45,927: INFO: *** IMPORTANT! ***
2019-03-09 08:53:45,934: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:53:45,934: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:53:45,934: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:53:45,934: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:54:48,695: INFO: *** IMPORTANT! ***
2019-03-09 08:54:48,697: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:54:48,697: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:54:48,697: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:54:48,697: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:55:51,475: INFO: *** IMPORTANT! ***
2019-03-09 08:55:51,475: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:55:51,475: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:55:51,475: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:55:51,480: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:55:55,927: DEBUG: Current IPs: ['192.168.0.150', '169.254.72.46', '10.10.7.2']
2019-03-09 08:56:54,544: INFO: *** IMPORTANT! ***
2019-03-09 08:56:54,546: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:56:54,546: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:56:54,547: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:56:54,547: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:57:56,920: INFO: *** IMPORTANT! ***
2019-03-09 08:57:56,921: INFO: ** AFTER the first download is COMPLETE, with in a minute or so you should connect to the new SSID "FinalStage" to finish the process.
2019-03-09 08:57:56,921: INFO: ** ONLY disconnect when the new "FinalStage" SSID is visible as an available WiFi network.
2019-03-09 08:57:56,922: INFO: This server should automatically be allocated the IP address: 192.168.4.2.
2019-03-09 08:57:56,922: INFO: If you have successfully connected to "FinalStage" and this is not the IP Address you were allocated, please ensure no other device has connected, and reboot your Sonoff.
2019-03-09 08:58:14,117: DEBUG: Current IPs: ['192.168.0.150', '169.254.72.46', '192.168.0.193']
