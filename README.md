# Docker Container with pandoc

[Docker](https://www.docker.io/) container for using [pandoc](https://pandoc.org/) to transform your docs

Display pandoc version :

```bash
docker run julienrollin/pandoc-docker
```

You can use the volume /source to convert your local files 

Usage to convert markdown to html5

```bash
docker run -v $PWD:/source julienrollin/pandoc-docker README.md -o README.html
```

Usage to convert markdown to pdf

```
docker run -v $PWD:/source julienrollin/pandoc-docker README.md -o README.pdf
```

[More examples](https://pandoc.org/demos.html) on Pandoc site