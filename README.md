
Install Mosquitto and Mosquitto clients

```
sudo apt-get install mosquitto mosquitto-clients
```
Test Mosquitto

```
BROKER=test.mosquitto.org
BROKER=localhost
mosquitto_pub -h $BROKER -d -t ultratrail/12345/56789 -m '{"user"=56789, "rpm"=120, "hrm"=172, "lat"=45.1234, "lng"=5.1234, "alt"=1479, "temp"=-1.2, "panic"=true }'
```

```
BROKER=test.mosquitto.org
BROKER=localhost
mosquitto_sub -h $BROKER -d -t ultratrail/12345/#
```




For running Meteor, execute

```
meteor run --settings settings.json
```

