# Installations

* [Remote Installation](../../resources/services/system-installation.pdf)
* [Self Installation](../../resources/services/self-installation.pdf)
* [Networking Guidlines](../../resources/networking/networking-guide.pdf)
* [Hardware Support Matrix](../../resources/scale/hardware-matrix.pdf)
* [Software Support Matrix](../../resources/scale/software-matrix.pdf)

#### Credentials
```
username : admin
password : admin
```
#### Commands
```
sudo scnodeinit
sudo scclusterinit
```
#### SNS
```
sudo singleNodeCluster=1 scclusterinit
```
#### Node Initialization Failure
```
REINITIALIZE=yes sudo scnodeinit
```
#### Network Inaccessible
```
BYPASS_NETWORK_CHECK=yes sudo scnodeinit
```
#### Combined Remedial Commands
```
BYPASS_NETWORK_CHECK=yes REINITIALIZE=yes sudo scnodeinit
```
#### Node Initilization Prompt
```
LAN IP : <>
LAN Netmask : <>
LAN Gateway : <>
Backplane IP of this node : <>
Backplane IP of first node in cluster : <>
Unique Software Serial : <>
Backplane VLAN ID : <> (single NIC applications only)
```