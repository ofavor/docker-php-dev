# docker-php-dev

## Directory Structure

* docker - docker-php-dev
* nginx - nginx config files
* mysql - mysql config files and data files
* redis - redis config and data files
* sites - php source files

## Usage

### Prepare Workspace

```
mkdir ~/Workspace/php
cd  ~/Workspace/php
```

### Clone

```git clone https://github.com/ofavor/docker-php-dev.git docker```

### Initialization

```
cd docker
chmod u+x init
./init
mkdir -p ../sites/default_server
echo "<?php phpinfo(); ?>" > ../sites/default_server/info.php
```

### Run

```
docker-compose up -d
```

Open url ```http://localhost:8080/info.php``` in browser