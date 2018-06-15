-------------------------------------------SETUP------------------------------------------------

Unpack RPITempsProbe.zip into a folder.
Both the Server.exe and the Client are standalone executables, and you can put them wherever you like it.
If you encounter any error when opening the server, extract libstdc++ -6.dll and put it in the same folder as Server.exe.

On the first boot, it will generate the standard configuration file, which changes between Server and Client.

Server features:
[General]
Show in the terminal the sensor values;
Log into a file .log the server status raw per raw;

[Network]
Set the network port;
Set the network protocol, you can choose between ipv4 and ipv6;

[Engine]
Set the name of your cpu sensor. You can check it inside HWiNFO64;

Client features:
[General]
Show in the terminal the sensor values;

[Network]
Set the Server ip, whereas the server is able to send data to any client, the reverse is not, so this is required for the connection to happen;
Set the network port;

[GPIO]
Set the GPIO pin for the safe mode;
Set the GPIO pin for the warning mode;
Set the GPIO pin for the critical mode;
You can find the GPIO pin configuration here: http://pi4j.com/images/j8header-3b.png

[Temperature]
Set value after which the cpu has reached warning temperatures;
Set value after which the cpu has reached critical temperatures;

------------------------------------------------------------------------------------------------
-----------------------------------------CHANGELOG----------------------------------------------

v1.3
Added support for server status logging for server only.

v1.2
Added support for configuration files for both server and client.

v1.1
Minor fixes.
Code optimization.

v1.0
First full release.
Only data recover from HWiNFO64 and network data transfer.

Alpha v0.3
Unified raw data recover from HWiNFO64 without the use of custom functions and network transfer between server and client.

Alpha v0.2
Added support for non-textual network data transfer.

Alpha v0.1b
Only network data transfer between server and client as IRC.

Alpha v0.1a
First alpha release.
Only data recover from HWiNFO64 using custom functions.

------------------------------------------------------------------------------------------------"# RPITC" 
