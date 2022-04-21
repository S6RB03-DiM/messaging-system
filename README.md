# messaging-system
GIT repository for our messaging system

First terminal in `\messaging-system`\
`.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties`

Second terminal in `\messaging-system`\
`.\bin\windows\kafka-server-start.bat .\config\server.properties`

Third terminal in `\messaging-system\bin\windows` for other commands:
- Create topic `.\bin\kafka-topics.bat --create --topic TOPIC --bootstrap-server localhost:9092`
- Send event `kafka-console-producer.bat --topic TOPIC --bootstrap-server localhost:9092` and then e.g. `Test event 1`, `Test event 2`
- Read events `kafka-console-consumer.bat --topic TOPIC --from-beginning --bootstrap-server localhost:9092`
