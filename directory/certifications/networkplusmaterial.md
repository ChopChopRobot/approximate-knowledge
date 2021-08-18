## CompTIA Network+ Training Material

### Network Scopes
* **PAN** : Personal Area Network
  * 0-10 meters
  * Connects electronic devices with a user's immediate area
  * Can be wired or wireless
    * Wired (USB, FireWire, Thunderbolt, etc)
    * Wireless (Bluetooth, Zigbee, IrDA, etc)
  * PANs do not typically do not connect to the Internet directly but may through a LAN

* **LAN** : Local Area Network
  * 0-100 meters
  * Scope of floor/home/office
  * Ethernet, WiFi
  * IEEE 802.3, IEEE 802.11

* **CAN** : Campus Area Network
  * Building centric LAN
  * Stretches across multiple buildings / miles

* **MAN** : Metropolitan Area Network
  * Up to about 25 miles or bigger

* **WAN** : Wide Area Network 
  * Connects geographically disparate internal networks and cists of leased lines or VPNs tunnels
  * State/Country/World
  * Internet is considered a WAN

### Network Types
  * **Client <-> Server Model**
    * Server provides resources to clients
    * Benefits : centralized resources, easier to manage and backup, scalable
    * Cons : costs more money, requires dedicated hardware, higher skillset
    * Leading model in the business world

  * **Peer <-> Peer Model**
    * Peers share resources collectively, no centralized data
    * Benefits : no infrastructure, no dedicated hardware, decentralized management
    * Cons : Hard to backup, bad scalability
    * Example : Napster & Torrenting, each person gives/receives files

### Topologies
  * **Bus Topology**
    * Single Cable running through an area that requires network connectivity
    * Each device taps into the cable
    * Single collision domain

  * **Ring Topology**
    * Single cable like a bus, however, running in a complete loop
    * Single collision domain
    * Uses Token Ring
      * Passed around logically allowing devices to take turns to talk

  * **FDDI Ring**
    * Fiber networks
    * Two rings running in opposite directions
    * Multiple rings allows for redundancy 

  * **STAR topology**
    * Everything talks to a central point
    * Central point of failure
    * Most popular type of network topology

  * **Hub and Spoke Topology**
    * Similar to STAR
    * Connects multiple sites together
    * Not fully redundant

  * **Full Mesh Topology**
    * Every single node or device is connected to every other node and optimal routing is always available
    * Single jump to each device
    * Often used in virtual implementations, physical is expensive
    * x = n(n-1) / 2 : number of connections required

  * **Partial Mesh Topology**
    * Hybrid of full mesh and hub & spoke topology

  * **Wireless**
    * Uses a wireless access point as a centralized point (similar to a star topology)
    * Supports wireless security controls and uses centralized management

  * **Ad Hoc**
    * Decentralized wireless network creating peer to peer connections and does not require a router

  * **IoT**
    * Internet of Things : (pretty much anything online)
    * 802.11 - WiFi (wireless or ad hoc)
    * Bluetooth
    * RFID : Radio Frequency ID
    * NFC : Near Field Communication (4cm)
    * IR - Infrared
    * Z-Wave - Short range, low latency data transfer (Home automation)
    * ANT+ - sensor data collection