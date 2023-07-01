# sample-project
sample-project repository

This repository was created just to demo the CI/CD of a web application into a web server via Jenkins.
Steps:
In a Jenkins setup, create the followign two Freestyle jobs and connect them to be part of a pipeline.
1) Build job --> This job pulls the code from this repository and creates a tar ball in the Build Actions stage.
  In the Post Build Actions stage, it will transfer the built tar file to a remote server (which runs a web server).
2) Deploy job --> This job will untar the tar file in the remote server, and copy the contents to the /var/www/html/ location of the httpd web server.
Finally, launch the web server IP address witht he copied folder name (as endpoint) and verify the deployment result.
  
