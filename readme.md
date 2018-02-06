### http://pjebz.github.io/peltest

## Installing Pelican
```
$ pip install pelican 
$ pip install markdown

```

## Create a pelican project
```
$ mkdir pelican
$ cd pelican
$ mkdir site
$ pelican-quickstart

Choose no makefiles

Make file in the 'content' directory called

```

# Generate html from pelican markdown
```
$ cd site
$ pelican content ; pushd output
$ python -m pelican.server
```


## Publish html using docker-machine and docker compose
```
$ docker-machine create \
-d digitalocean \
--digitalocean-access-token=ADD_YOUR_TOKEN_HERE \
--digitalocean-size=1gb \ # 1gb default
bloghost

deval bloghost
docker-compose build
docker-compose up -d

```

## Pushing to Github pages
```bash
$ cd pjebz.github.io
$ pelican content ; pushd output
$ python -m pelican.server

or

$ git add -u ; git commit -m "make changes"
$ git push origin gh-pages

```