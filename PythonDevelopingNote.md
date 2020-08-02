# Networking
## 知识点
   * 参考
      + [TCP vs UDP: What's the Difference?](https://www.guru99.com/tcp-vs-udp-understanding-the-difference.html)<br>
      + YouTube
         - [What is UDP (User Datagram Protocol)? UDP/IP vs. TCP/IP](https://www.youtube.com/watch?v=zFS0FaSqvcQ)<br>
## Socket
   * 参考
      + [socket — Low-level networking interface](https://docs.python.org/3/library/socket.html)<br>
      + [socket — Low-level networking interface -3.8 Version](https://docs.python.org/3.8/library/socket.html)<br>
      + [Socket Programming HOWTO](https://docs.python.org/3/howto/sockets.html)<br>
      + [asyncore — Asynchronous socket handler](https://docs.python.org/3.8/library/asyncore.html)<br>
      + [Streams](https://docs.python.org/3.8/library/asyncio-stream.html)<br>
      
      
      + [Python socket – chat server and client with code example](https://www.binarytides.com/code-chat-application-server-client-sockets-python/)<br>
   * Sample Code
      + [Socket Server with Multiple Clients | Multithreading | Python](https://codezup.com/socket-server-with-multiple-clients-model-multithreading-python/)<br>

## Socket 的 Thread 方法
   * 参考
      + 这个例子是很重要（重要参考）：[Write a Multithreaded Server in Python](https://www.techbeamers.com/python-tutorial-write-multithreaded-python-server/)<br>
      + [Python Threaded TCP Socket Server Example](https://forum.derivative.ca/t/python-threaded-tcp-socket-server-example/12002)<br>
      + 例子：[matthewwachter/py-tcp-threaded-server](https://github.com/matthewwachter/py-tcp-threaded-server><br>
      + [Python socketserver.ThreadingTCPServer(https://www.programcreek.com/python/example/107959/socketserver.ThreadingTCPServer) Examples]()<br>
## WebSocket 

## MQTT
   * 参考
      + [Beginners Guide To The Paho MQTT Python Client](http://www.steves-internet-guide.com/into-mqtt-python-client/)<br>
      + [Paho Python MQTT Client Subscribe With Examples](http://www.steves-internet-guide.com/subscribing-topics-mqtt-client/)<br>
      + [How to Install Mosquitto on The Raspberry Pi - 安装的重要参考](https://stevessmarthomeguide.com/install-mosquitto-raspberry-pi/)<br>
      + [Paho Python - MQTT Client Library Encyclopedia](https://www.hivemq.com/blog/mqtt-client-library-paho-python/)<br>
         - 说明：指定版本、指定用户等，研究这篇文章及例子
Calling mosquitto stop and start from Python](https://www.raspberrypi.org/forums/viewtopic.php?t=262978) - 两种方法<br>
      + [mosquitto_pub man page](https://mosquitto.org/man/mosquitto_pub-1.html)<br>
      + [mosquitto_sub man page](https://mosquitto.org/man/mosquitto_sub-1.html)<br>
      + [mosquitto_pub - an MQTT version 5/3.1.1/3.1 client for publishing simple messages](https://manpages.debian.org/testing/mosquitto-clients/mosquitto_pub.1.en.html)<br>
      + [CloudAMQP with MQTT and Python Getting started](https://www.cloudamqp.com/docs/python_mqtt.html) - 例子中事件全，参考<br>
      
      + [Node-RED - Low-code programming for event-driven applications](https://nodered.org/)<br>
      + Youtube
         - [Understanding MQTT: How Smart Home Devices Communicate](https://www.youtube.com/watch?v=NjKK5ab0-Kk)<br>
   * 源代码 - Sample
      + /raspberrypidev_local/pythondev/mqttdev/example/PiPy-MQTT
      + [C语言的例子](MQTT client examples](https://cumulocity.com/guides/device-sdk/mqtt-examples/)<br>
      + [CloudMQTT 的例子](https://www.cloudmqtt.com/docs/python.html)<br>
      + [Sending and Receiving Messages with MQTT](https://www.ev3dev.org/docs/tutorials/sending-and-receiving-messages-with-mqtt/) - 乐高的机器人编程工具教程<br>
   * 查询是否运行及占用的端口
      + [MQTT Broker help](https://www.raspberrypi.org/forums/viewtopic.php?t=268552)<br>
      + ps -ef | grep mosq
      + sudo netstat -tlnpu | grep mosq
      + sudo systemctl status mosquitto
   * 安装步骤
      1. 下载
         - ```
              ce /softwares
              wget http://repo.mosquitto.org/debian/mosquitto-repo.gpg.key
              sudo apt-key add mosquitto-repo.gpg.key
           ```
      2. Then make the repository available :
         - ```
               cd /etc/apt/sources.list.d/
           ```
      3. Then , depending on which version of debian you are using:
         - ```
              sudo wget http://repo.mosquitto.org/debian/mosquitto-jessie.list
              sudo wget http://repo.mosquitto.org/debian/mosquitto-stretch.list
              sudo wget http://repo.mosquitto.org/debian/mosquitto-buster.list
           ```
      4. Then update apt information:
         - ```
              sudo apt-get update
              sudo apt-get install mosquitto
              sudo apt-get install mosquitto-clients
           ```
   * Running Mosquitto Manually
      1. The first step is to stop mosquitto using:
         - ```
              sudo systemctl stop mosquitto.service 
           ```
      2. Then you can start it using:
         - ```
               mosquitto -v   #start in verbose mode
           ```
   * Testing the Install
      1. So first open two command prompts in one type.
         - ```
             mosquitto_sub -h localhost -t bedroom/light -d
           ```
      2. in the second type
         - ```
             mosquitto_pub -h localhost -t bedroom/light -m  message
           ```
## Python 异步的方法
   * 参考
      + [Python-based MQTT #1: HBMQTT Broker & Paho MQTT Client](https://www.youtube.com/watch?v=hmM4h174suk)<br>
## Python Flask
   * 参考
      + [欢迎进入Flask大型教程项目！- 下面教程的中文版](http://www.pythondoc.com/flask-mega-tutorial/)<br>
      + [The Flask Mega-Tutorial Part I: Hello, World!](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)<br>

# Run Python App
## 执行Python脚本的方法
   * Google Search: run python script in background - raspberry pi
   * Google Search: launch python script on startup raspberry pi
   * Google Search: how to run python script as a background process
