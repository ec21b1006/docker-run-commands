# Docker
## docker run tags
- `--add-host` = Add a custom host-to-IP mapping (host:ip) 
    > Know more about adding host(s) here : [Add a Host Entry to a Docker Container](https://codeopolis.com/posts/add-a-host-entry-to-a-docker-container/)
    > Know more about host(s) in linux here : [What Is the /etc/hosts File in Linux](https://blog.purestorage.com/purely-informational/what-is-the-etc-hosts-file-in-linux/)
- `--annotation` = Add an annotation to the container (passed through to the OCI runtime)
- `--attach`, `-a` = Attach to STDIN, STDOUT or STDERR
- `--blkio-weight` = Block IO (relative weight), between 10 and 1000, or 0 to disable (default 0)
    > Read more here : [Control container resource usage with limits](https://medium.com/@arton.demaku/master-docker-like-a-pro-5-essential-tips-and-tricks-for-devops-engineers-30ef68920188#:~:text=Note%3A%20%2D%2Dblkio,to%20a%20container%3A)
- `-blkio-weight-device` = Block IO weight (relative device weight)
- `--cap-add` = Add Linux capabilities
- `--cap-drop` = Drop Linux capabilities
    > Read more about Linux capabilities here: [capabilities(7) — Linux manual page](https://man7.org/linux/man-pages/man7/capabilities.7.html)
- 