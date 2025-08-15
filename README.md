requiere instalar novnc

```bash 
python3 /usr/lib/python3.9/site-packages/websockify/websocketproxy.py --web /usr/share/novnc/ --target-config=/usr/share/novnc/tokens 6080
```

/usr/share/novnc/tokens:
```
servidor1: 192.100.1.100:5900
servidor2: 192.100.1.150:5901
```

```
firefox http://servidor:6080/vnc.html?path=?token=servidor1
```

```
firefox http://servidor:6080/vnc.html?path=?token=192.100.1.150:5900
```

