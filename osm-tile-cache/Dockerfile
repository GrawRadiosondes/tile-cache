FROM python:2.7

RUN pip install Paste

RUN easy_install TileCache
RUN tilecache_install_config.py

COPY tilecache.cfg /etc/tilecache.cfg

#CMD ["cat", "/etc/tilecache.cfg"]
CMD ["tilecache_http_server.py"]