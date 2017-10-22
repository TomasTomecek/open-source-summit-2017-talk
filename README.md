# From Dockerfiles to Ansible Container

[Slides](https://tomastomecek.github.io/open-source-summit-2017-talk/)

## Running locally

GitHub uses [jekyll](https://github.com/jekyll/jekyll) to deploy, here's how to do it locally:

```
docker run --rm --name=os-summit-talk -v ${PWD}:/srv/jekyll:Z \
  -it -p 127.0.0.1:4000:4000 jekyll/jekyll jekyll serve
```

and

```
$ xdg-open localhost:4000
```

[Source](https://github.com/jekyll/docker/wiki/Usage:-Running)
