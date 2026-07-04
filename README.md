# ecovacs-DeebotUniverse


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
