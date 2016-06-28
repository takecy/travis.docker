# Docker template for travis CI

[![Build Status](https://travis-ci.org/takecy/travis.docker.svg?branch=master)](https://travis-ci.org/takecy/travis.docker)

[TravisCI](https://travis-ci.org/)

<br/>
## Why not use the travis service?

Travis CI provides [docker service](https://docs.travis-ci.com/user/docker/).  
but this docker is version `1.8.1` (2016/06/28), it is too old.  

<br/>
## Why sudo is required?

To use docker command without sudo, add user(travis) to docker group.  

[Install Docker(ubuntu)](https://docs.docker.com/engine/installation/linux/ubuntulinux/)  
```
$ sudo groupadd docker
$ sudo usermod -aG docker travis
```
but this way is need to logout/login.  

<br/>
## License
[MIT](./LICENSE)