Python program to query MAC address on https://macaddress.io/



- Build docker container
  Docker should be installed and in running state.
  to check please run docker --version

2) Clone git code
```bash
git clone https://github.com/Flyinsky9/Cisco.git
```
3) Build Dockerfile
```bash
cd Cisco
docker build -t mac-adder:public .
```
4) List the images
```bash
docker image ls -a| grep -i mac-addr
```
5) Run container
```bash
docker run -it <image id>
```
- Query MAC Address
```bash
root@329c70f143c8:~# python mac-addr.py 44:38:39:ff:ef:57
```
