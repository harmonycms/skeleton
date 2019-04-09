HarmonyCMS Skeleton
===================
This is a skeleton application for HarmonyCMS.
This repository contain a pre-configured Docker environment for development and test purpose.

Instructions
------------

### Requirements
* [Docker]
* [Docker compose]

### Services configuration

| Service | Ports       |
| ------- | ----------- |
| php     | 9000        |
| nginx   | 8080:80     |
| mariadb | 3306:3306   |
| mongodb | 27017:27017 |

### Installation
1. Start Containers
```bash
docker-compose up -d
```

2. Connect to php container
```bash
docker-compose exec php bash
```

3. Create new project
```bash
composer create-project harmony/skeleton demo
```

License
-------
This bundle is part of the [HarmonyCMS] and licensed under the [LGPLv3 License]. 

[Docker]: https://docs.docker.com/install/
[Docker compose]: https://docs.docker.com/compose/install/
[HarmonyCMS]: https://harmonycms.net
[LGPLv3 License]: https://opensource.org/licenses/lgpl-3.0.html