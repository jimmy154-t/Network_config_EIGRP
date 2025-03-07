# EIGRP Network Project

This project is a network design using Cisco Packet Tracer, implementing EIGRP (Enhanced Interior Gateway Routing Protocol) for routing between four routers.

## Project Description

The project consists of a network setup where four routers are connected through serial interfaces and configured to use EIGRP for routing. The network involves different subnets and is designed to test routing functionality and EIGRP's behavior in a multi-router environment.

### Devices in the Network:
- **Router 1**: Connected to three serial interfaces and one FastEthernet interface.
- **Router 2**: Connected to three serial interfaces and one FastEthernet interface.
- **Router 3**: Connected to three serial interfaces and one FastEthernet interface.
- **Router 4**: Connected to three serial interfaces and one FastEthernet interface.

### IP Addressing:
- **Router 1**:  
  - FastEthernet 0/0: 10.10.10.1/8  
  - Serial 0/0/0: 192.168.10.1/24  
  - Serial 0/1/0: 192.168.40.2/24  
  - Serial 0/0/1: 192.168.50.1/24  

- **Router 2**:  
  - FastEthernet 0/0: 11.11.11.1/8  
  - Serial 0/0/0: 192.168.20.1/24  
  - Serial 0/1/0: 192.168.10.2/24  
  - Serial 0/0/1: 192.168.60.1/24  

- **Router 3**:  
  - FastEthernet 0/0: 12.12.12.1/8  
  - Serial 0/0/0: 192.168.30.1/24  
  - Serial 0/1/0: 192.168.20.2/24  
  - Serial 0/0/1: 192.168.50.1/24  

- **Router 4**:  
  - FastEthernet 0/0: 10.10.10.1/8  
  - Serial 0/0/0: 192.168.40.1/24  
  - Serial 0/1/0: 192.168.30.2/24  
  - Serial 0/1/1: 192.168.60.1/24  

## EIGRP Configuration

EIGRP has been configured on all routers with the same Autonomous System (AS) number (`AS 10`). The networks advertised and included in the EIGRP process are:

- **Router 1**:  
  - `network 192.168.10.0 0.0.0.255`
  - `network 192.168.40.0 0.0.0.255`
  - `network 192.168.50.0 0.0.0.255`
  - `network 10.10.10.0 0.255.255.255`

- **Router 2**:  
  - `network 192.168.10.0 0.0.0.255`
  - `network 192.168.20.0 0.0.0.255`
  - `network 192.168.60.0 0.0.0.255`
  - `network 11.11.11.0 0.255.255.255`

- **Router 3**:  
  - `network 192.168.30.0 0.0.0.255`
  - `network 192.168.20.0 0.0.0.255`
  - `network 192.168.50.0 0.0.0.255`
  - `network 12.12.12.0 0.255.255.255`

- **Router 4**:  
  - `network 192.168.40.0 0.0.0.255`
  - `network 192.168.60.0 0.0.0.255`
  - `network 192.168.30.0 0.0.0.255`
  - `network 13.13.13.0 0.255.255.255`

## How to Open the Project

1. **Prerequisites**:
   - You need to have [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) installed on your computer to open and view the `.pkt` file.

2. **Opening the File**:
   - Download the `.pkt` file from the repository.
   - Open the file using Cisco Packet Tracer.

3. **Running the Network**:
   - Once the network is loaded in Cisco Packet Tracer, you can start the simulation to see the routing protocol in action.
   - You can also check the routing table and verify the EIGRP configurations on each router.

## Network Topology

![Network Topology](./images/NETWORK_EIGRP.png)  
*(Optional: You can add a network topology image if you have one.)*

## Contributing

Feel free to fork this repository, make improvements, and create pull requests. If you have suggestions or want to report issues, open an issue in the repository.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

