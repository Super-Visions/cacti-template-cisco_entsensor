# Cisco - Entity Sensors
Cacti data query to graph data of a sensor listed in the Entity-MIB entPhysicalTable.

## Associated Graph Templates
* Temperature (Cisco - Entity Sensor Temperature)

Others (voltage, current, fan, ...) will be added in the future.

## Prerequisites
In order to translate the different data query input fields, 
the [CISCO-ENTITY-SENSOR-MIB](http://tools.cisco.com/Support/SNMP/do/BrowseMIB.do?local=en&step=2&mibName=CISCO-ENTITY-SENSOR-MIB) and its dependencies needs to be installed.
You can verify correct OID translation and check if your device supports this MIB by running an `snmpwalk` or `snmptable` on `CISCO-ENTITY-SENSOR-MIB::entSensorValueTable`.

## Installation
1. Copy the contents of `snmp_queries` to `resource/snmp_queries` in the Cacti directory.
1. Import `cacti_data_query_cisco_-_entity_sensors.xml` from the Cacti UI.
1. _Optional:_ Add this Data Query to the Associated Data Queries of Cisco Host Templates.
