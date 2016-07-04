Base Image Docker Container
======================


### Basic Usage

FROM rbrooker/base


### Important

add these lines to the second half of your container Dockerfile, to clean up images

```
RUN apt-get purge -y wget apt-transport-https apt-utils <plus and other parts only need to build applications>
# clean extra-files 
RUN  apt-get autoremove -y ; apt-get clean && rm -rf /var/lib/apt/lists/*
```



Maintained by  
-------------

Ramon Brooker <rbrooker@aetherealmind.com>



