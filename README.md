Caddy + LetsEncrypt + Sonarr
============================

THIS PROJECT IS AN EXAMPLE, DO NOT CHANGE NAMES AND USE IT
THERE IS NO AUTHENTIFICATION SCHEME AND AS SUCH IS OPEN TO
THE WORLD

Documentation
-------------
https://caddyserver.com/docs
https://sonarr.tv/
https://github.com/Sonarr/Sonarr
https://docs.docker.com/compose/compose-file/

Directory structure:
--------------------

```
caddy-letsencrypt-sonarr/
├── data
│   └── web
│       ├── Caddyfile
│       └── www
│           └── index.html
└── services
    ├── sonarr
    │   └── docker-compose.yml
    └── web
        └── docker-compose.yml
```

How to use
----------
```
cd # Go to home directory
git clone https://github.com/Magicking/caddy-letsencrypt-sonarr.git
docker-compose -f caddy-letsencrypt-sonarr/services/sonarr/docker-compose.yml -f caddy-letsencrypt-sonarr/services/web/docker-compose.yml up
```
