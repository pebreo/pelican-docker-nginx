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
$ mkdir pjebz.github.io
$ pelican-quickstart

Choose no makefiles
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