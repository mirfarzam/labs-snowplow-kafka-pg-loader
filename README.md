# Kafka to Postgres simple scala storage loader

## Getting Started

This Code is ready to use Storage loader which save atmoic data. for custom events or custom dimension you need to add to this code and you know how !


### Configuration

In the config.conf file you can adjust your Ne04j storage loader with cofiguration that you want.

Firstly, Set you Kafka connection information in below. It is better to set specific consumer id in order to Kafka manages offsets. you can seperate yor brokers just by comma !

```
kafka{
  brokers = "broker1,broker2"
  topic = "someTopic"
  consumerGroupId = "someConsumerGroupID"
}
```

Secondly, You should set you Postgres Connection information. In numberOfThread field you should mention that how many thread you need to start.

```
postgres{
  driver = "org.postgresql.Driver"
  url = "jdbc:postgresql://ip:port/databaseName"
  username = "########"
  password = "#########"
  groupid = "GroupID"
  numberOfThreads = 1
}

```

## Contributing

This Program is Coded by [Digikala](https://Digikala.com) Data Science Team.

## RoadMap

we decided to refactor our code and design in ib actor model and implement by akka, but at this time it is not reqired.

## Author

* **SeyedFarzam Mirmoeini** - *Data Science Specialist* - [Github](https://github.com/mirfarzam)

