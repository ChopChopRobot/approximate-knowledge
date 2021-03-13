# Installations

* [Remote Installation](../../resources/services/system-installation.pdf)
* [Self Installation](../../resources/services/self-installation.pdf)

### Quick Reference

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