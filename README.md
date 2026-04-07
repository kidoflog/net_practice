*This project has been created as part of the 42 curriculum by kkido*
## Description
NetPractice is a puzzle-based assignment designed for learning the fundamentals of the Internet. In this assignment, you are required to properly set up a communication environment by correctly configuring IP addresses, subnet masks, and routing for devices such as hosts and routers.
## Instructions

### Preparation

- Run the following command to download the NetPractice archive file:
```
wget https://cdn.intra.42.fr/document/document/46101/net_practice.1.9.tgz
```
- Run the following command to extract the archive file:
```
tar -xvf net_practice.1.9.tgz
```

### Usage
- Run the following command within the ```net_practice``` directory obtained in the preparation step:
```
./run.sh
```
## Resources
### References
- [「ネットワークはなぜつながるのか 第2版 知っておきたいTCP/IP、LAN、光ファイバの基礎知識」](https://www.amazon.co.jp/ネットワークはなぜつながるのか-第2版-知っておきたいTCP-IP、LAN、光ファイバの基礎知識-戸根/dp/4822283119)
- [「【ネットワーク】TCP/IP　インターネット層とIPを理解する」](https://qiita.com/rgj0830/items/cb6e248d75d641f0a138)
- [「TCP/IPとは？」](https://www.itmanage.co.jp/column/tcp-ip-protocol/)
- [「デフォルトゲートウェイ」](https://biz.kddi.com/content/glossary/d/default-gateway/)
- [「OSI参照モデルとは？TCP/IPとの違いを図解で解説」](https://www.itmanage.co.jp/column/osi-reference-model/)
### Terms

#### TCP/IP addressing
- TCP/IP is a globally standard communication protocol used in computer networks. TCP is a communication protocol designed to ensure accurate data exchange. Meanwhile, IP is a protocol used to specify communication destinations using numerical values known as IP addresses. Although there are IPv4 and IPv6 addresses, 32-bit IPv4 is currently the mainstream and is the one used in this assignment. IP addressing refers to the process of uniquely identifying a communication destination using these IP addresses.
#### subnet masks
- A subnet is a smaller network unit created by dividing a large network. By using subnets, you can limit the reach of communication and reduce unnecessary traffic, which allows routing to be performed more efficiently. Users utilize a subnet mask to divide an IP address into a network portion and a host portion. Hosts can form a subnet by sharing the same network portion.
#### default gateways
- A default gateway refers to a network device used when data is sent from within a network to the outside, and it generally refers to a router. It is used when the destination is not located within the same network, serving as a gateway to access the internet.
#### routers and switches
- A router is a device used for the aforementioned default gateway, responsible for defining the route (routing) to ensure that data is properly transmitted and received. - A switch is a relay device used to transmit and receive data between devices located within the same network.
#### OSI layers
- The OSI reference model divides and defines the functions required for a computer network into a 7-layer structure.
- The Application Layer defines the specific functions, communication procedures, and data formats for the software operated by the user. Since there are countless variations depending on the application being used, it utilizes the hardware's communication capabilities according to the specific application.
- In the Presentation Layer, data is converted into an appropriate format, enabling the delivery of suitable data to the Application Layer.
- The Session Layer defines the procedures for establishing, maintaining, and terminating communication between hosts. The currently mainstream protocol is TLS. TLS enables secure communication through the use of digital certificates.
- The Transport Layer is responsible for achieving communication quality, such as reliability and real-time performance, with TCP and UDP being representative examples. TCP is a protocol that excels in reliability, while UDP excels in real-time performance.
- The Network Layer connects multiple networks to enable mutual communication, with IP being the representative protocol.
- The Data Link Layer enables communication between directly connected devices (nodes). A representative example is an Ethernet connection using MAC addresses. A MAC address is used as the destination when transferring data between nodes.
- The Physical Layer defines physical connections, such as the shape of hardware connectors.
### How AI was used
- Documentation Support: Translating and refining content for `README.md`.

## Submission details
The 10 config files obtained from the training must be submitted directly in the root directory of the submitted repository.
