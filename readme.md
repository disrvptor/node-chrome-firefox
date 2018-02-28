# Forked

This is a fork of Atlassian's https://bitbucket.org/atlassian/docker-node-chrome-firefox

# Dockerfile for Node/Karma tests in Chrome and Firefox

This Dockerfile contains:

* SCM tools
* Node 6.x
* Google Chrome latest
* Firefox ESR latest
* Bzip2 (for PhantomJS install)

## How to build the image
```
docker build -t node-chrome-firefox .
```

then use `docker images` to find the image ID.

With `docker run -it <IMAGE_ID>` you can test if your changes are the desired ones.

Then tag it: `docker tag <IMAGE_ID> <YOUR-USER>/node-chrome-firefox:latest`

and finally publish it: `docker push <YOUR-USER>/node-chrome-firefox`
