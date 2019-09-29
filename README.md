# Run in terminal:
```
$ dk run -it --rm --name my-running-script -v "$PWD":/usr/src/app -w /usr/src/app node node node-test.js
```

`-it` runs the container in the interactive mode, where you can execute several commands inside the container.

`--rm` automatically removes the container after finishing its execution.

`--name [name]` provides a name to the process running in the Docker daemon.

`-v [local-path: docker-path]` mounts a local directory into Docker, which allows exchanging information or access to the file system of the current system.

`-w [docker-path]` sets the working directory (start route). By default, this is **/**.

`node` is the name of the image to run. It always comes after all the docker run flags.

`node node-test.js` are instructions for the container. These always come after the name of the image.

#### See more in: https://blog.logrocket.com/docker-for-front-end-developers/