# Firefox in Singularity

This repository contains a [Singularity](https://www.sylabs.io/docs/) recipe to
build a container image with Firefox installed on CentOS 7.uild a container
image with Firefox installed on CentOS 7.

To build:

```
sudo singularity build singularity-firefox.sif Singularity
```

Or, to pull the pre-built image:


```
singularity pull shub://nuitrcs/singularity-firefox
```


To run Firefox (make sure `$DISPLAY` is set!):


```
singularity exec -B ~/run:/run singularity_firefox.sif firefox
```
