# ecovacs-DeebotUniverse

## ha System information

~~~
Version	core-2026.6.4
Installation type	Home Assistant Container
Development	false
Supervisor	false
Docker	true
Container architecture	aarch64
User	root
Virtual environment	false
Python version	3.14.5
Operating system family	Linux
Operating system version	6.12.75+rpt-rpi-2712
CPU architecture	aarch64
Timezone	Asia/Shanghai
Configuration directory	/config
~~~

## deebot inforation

~~~
DEEBOT X5 PRO
Model: MXSE7W
Region: China

~~~


~~~
 docker exec -it ha  sh
/config # cd  /usr/local/lib/python3.14/site-packages/deebot_client/hardware/
/usr/local/lib/python3.14/site-packages/deebot_client/hardware # ls -l


~~~

## modify mxse7w.py
~~~
cd /data/homeassistant202405

docker cp  ha:/usr/local/lib/python3.14/site-packages/deebot_client/hardware/mxse7w.py .

docker cp mxse7w.py ha:/usr/local/lib/python3.14/site-packages/deebot_client/hardware/

docker restart ha
~~~
