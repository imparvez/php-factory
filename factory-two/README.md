# Documentation:
`/var/www/html` is just the default root folder of the web server.

# Command to build
`docker build -t <tag-name> .`
`<tag-name>` can be anything

Example:
`docker build -t php-demo .`

This example specifies that the PATH is `.`, and so all the files in the local directory get `tar`d and sent to the Docker daemon. The PATH specifies where to find the files for the “context” of the build on the Docker daemon.
`-t` is used just to tag an image.

# Command to run
`sudo docker run -p 80:80 php-demo`