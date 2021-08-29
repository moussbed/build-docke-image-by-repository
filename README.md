# build-docke-image-by-repository

The docker build command builds an image from a Dockerfile and a context. The build’s context is the set of files at a specified location PATH or URL. The PATH is a directory on your local filesystem. The URL is a Git repository location.

PATH

The build context is processed recursively. So, a PATH includes any subdirectories and the URL includes the repository and its submodules. This example shows a build command that uses the current directory (.) as build context:

$  docker build .


URL 

You can specify a repository and tag at which to save the new image if the build succeeds:

docker build -t moussbed/build-docke-image-by-repository .