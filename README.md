# Zabbix_TCP_Ports_Template

## Macros used

|Name|Description|Default|Type|
|----|-----------|-------|----|
|{$TCP.PORT.MATCHES}|<p>-</p>|(80|443|22|3306)|Regex|


## Template links

There are no template links in this template.

## Discovery rules

|Name|Description|Type|Key and additional info|
|----|-----------|----|----|
|Check TCP Connection on Port {$PORT}|<p>Discovers TCP within a single instance specified by Users Parameter.</p>|`Zabbix agent`|netstat.tcp.listen <p>Update Interval 1h</p>|

## Items collected

|Name|Description|Type|Key and additional info|
|----|-----------|----|----|
|TCP Port {#PORT}|check tcp connection with built-in net.tcp.service[tcp,,{#PORT}]|Zabbix Agent|net.tcp.service|

## Contributing

If you have suggestions for improvements or would like to contribute to this project, please fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

## Author

[Thaw Thu Han](https://github.com/ThawThuHan)