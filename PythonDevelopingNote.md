# Networking
## 知识点
   * 参考
      + [TCP vs UDP: What's the Difference?](https://www.guru99.com/tcp-vs-udp-understanding-the-difference.html)<br>
      + YouTube
         - [What is UDP (User Datagram Protocol)? UDP/IP vs. TCP/IP](https://www.youtube.com/watch?v=zFS0FaSqvcQ)<br>

### 开机启动 Python 应用的方法 - Linux & Raspberry Pi
   * 参考
      + [SkinnyPi - Weight Loss Party - Python Script](https://github.com/jazmy/raspberrypi-skinnypi/README.md)<br>
         - > [How to Run a Raspberry Pi Program on Startup](https://learn.sparkfun.com/tutorials/how-to-run-a-raspberry-pi-program-on-startup#method-1-rclocal)<br>
           >```
               sudo nano /etc/rc.local
            ```
           >This is tricky but you need to ensure that you wait 10 seconds to give your pi enough time to boot and connect to the network before you run your script. This will create a log file if there are problems.
           >```
               sudo bash -c '(sleep 10;/usr/bin/python3 /home/pi/skinnypi/skinnypi.py > /home/pi/skinnypi/skinnypi.log 2>&1)' &
            ```
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
## WebSocket 


## Python Flask
   * 参考
      + [欢迎进入Flask大型教程项目！- 下面教程的中文版](http://www.pythondoc.com/flask-mega-tutorial/)<br>
      + [The Flask Mega-Tutorial Part I: Hello, World!](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)<br>
