# Auto Install with cloud-init 

**Make a local webserver**

serve this file user-data and meta-data from directory
```
python3 -m http.server <port>
```

boot iso and in grub edit the kernel parameters 

after linux add between kernel and **---**

```autoinstall "ds=nocloud-net;s=http://<ip-address>:<port>/"```

Will install all with the cloud-init script


