# A git 101 codelab

Positive
: To Enter the codelab go to [https://roei-bracha.github.io/git-codelab](https://roei-bracha.github.io/git-codelab)

# This repo use Claat Docker image 

> Docker image of claat tool used to generate beautiful codelabs from markdown or Google doc

### 🐳 [Image on Docker Hub](https://hub.docker.com/r/bpetetot/claat)

## Install

```sh
docker pull bpetetot/claat
```

## Usage

```sh
docker container run -it -v $(pwd):/app bpetetot/claat export my-codelab.md
```

When you are working on the codelab, you can serve it on localhost:

```sh
docker container run -it -p 9090:9090 -v $(pwd):/app bpetetot/claat serve -addr 0.0.0.0:9090 my-codelab.md
```
