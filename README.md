# NGINX with Google Page Speed module (Docker)

[![Build Status](https://circleci.com/gh/donbeave/docker-nginx-pagespeed.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/donbeave/docker-nginx-pagespeed)
[![Analytics](https://ga-beacon.appspot.com/UA-71075299-1/docker-nginx-pagespeed/main-page)](https://github.com/igrigorik/ga-beacon)

Lightweight NGINX with Google PageSpeed module container (based on minimalist Debian wheezy image)

### Debian packages

https://bintray.com/donbeave/deb/nginx-pagespeed

#### How to install?

Add bintray repository:
```bash
curl 'https://bintray.com/user/downloadSubjectPublicKey?username=bintray' | apt-key add -
echo "deb http://dl.bintray.com/donbeave/deb wheezy main" >> /etc/apt/sources.list
```

Download the package lists from the repositories:
```bash
apt-get update
```

Install nginx package:
```bash
apt-get install -y ca-certificates nginx-pagespeed
```

### Docker image

https://hub.docker.com/r/donbeave/nginx-pagespeed

#### How to use?

In your `Dockerfile` use the following:
```
FROM donbeave/nginx-pagespeed:1.8.0-1

...
```

Copyright and license
---------------------

Copyright 2015 Alexey Zhokhov under the [Apache License, Version 2.0](LICENSE). Supported by [AZ][zhokhov].

[zhokhov]: http://www.zhokhov.com
