dockerize
=========

`dockerize` is a tiny wrapper for `docker build`.

It is designed to be as smallest as possible.
Thus, the ONLY use case it is intended to be used for is :

- name of the Dockerfile is the default one : `PATH/Dockerfile`
- context is current working directory : `.`
- no build-arg
- no cpu limit nor memory limit

Currently, any other case must be dealt with `docker build` directly.


## Installation

In your shell rc file, add the following line :

```
source /path/to/dockerize
```


## Usage

### Use default _name:tag_

Coming soon...

### Set your own _name:tag_

To build an image with the default tag :

```
cd /path/to/your/Dockerfile/
dockerize <name>
```

A custom tag can be specified as followed :

```
cd /path/to/your/Dockerfile/
dockerize <name>:<tag>
```


## License

All contents licensed under the [WTFPL](LICENSE)

