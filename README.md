# docker-run-commands
## [docker run tags](https://docs.docker.com/engine/reference/commandline/run/)
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
- `--cgroup-parent` = 	Optional parent cgroup for the container
    > Read more here : [Docker limit resource utilization using cgroup-parent](https://medium.com/@asishrs/docker-limit-resource-utilization-using-cgroup-parent-72a646651f9d)
- `--cpu-period` = Limit CPU CFS (Completely Fair Scheduler) period
- `--cpu-quota` = Limit CPU CFS (Completely Fair Scheduler) quota
    > Read more here: [cpu.cfs_period_us & cpu.cfs_quota_us](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/resource_management_guide/sec-cpu)
- `--cgroupns` = Cgroup namespace to use (host|private)

    'host': Run the container in the Docker host's cgroup namespace

    'private': Run the container in its own private cgroup namespace

    '': Use the cgroup namespace as configured by the
    default-cgroupns-mode option on the daemon (default)
- `--cidfile` = Write the container ID to the file
- `--cpu-rt-period` = Limit CPU real-time period in microseconds
- `--cpu-rt-runtime` = Limit CPU real-time runtime in microseconds
- `--cpu-shares` or `-c` = CPU shares (relative weight)
- `--cpus` = Number of CPUs
    > Read more here : [Docker Container CPU Limits Explained](https://www.thorsten-hans.com/docker-container-cpu-limits-explained/)
- `--cpuset-cpus` = CPUs in which to allow execution (0-3, 0,1)
- `--cpuset-mems` = MEMs in which to allow execution (0-3, 0,1)
- `--detach` or `-d` = Run container in background and print container ID
- `--detach-keys` = Override the key sequence for detaching a container
- `--device	` = Add a host device to the container
- `--device-cgroup-rule` = Add a rule to the cgroup allowed devices list
- `--device-read-bps` = Limit read rate (bytes per second) from a device
- `--device-read-iops` = Limit read rate (IO per second) from a device
- `--device-write-bps` = Limit write rate (bytes per second) to a device
- `--device-write-iops` = Limit write rate (IO per second) to a device
- `--disable-content-trust` = Skip image verification
    > Read more here : [Content trust in Docker](https://docs.docker.com/engine/security/trust/#:~:text=Content%20trust%20is%20disabled%20by,unless%20they%20contain%20a%20signature.)
- `--dns` = Set custom DNS servers
- `--dns-opt` = Set DNS options
- `--dns-option` = Set DNS options
- `--dns-search	` = Set custom DNS search domains
- `--domainname` = Container NIS domain name
- `--entrypoint` = Overwrite the default ENTRYPOINT of the image
- `--env` or -`e` = Set environment variables
- `--env-file` = Read in a file of environment variables
- `--expose` = Export a port or a range of ports
- `--gpus` = GPU devices to add to the container ('all' to pass all GPUs)
- `--group-add` = Add additional groups to join
- `--health-cmd` = Command to run to check health
- `--health-interval` = Time between running the check (ms|s|m|h) (default 0s)
- `--health-retries` = Consecutive failures needed to report unhealthy
- `--health-start-period` = Start period for the container to initialize before starting health-retries countdown (ms|s|m|h) (default 0s)
- `--health-timeout` = Maximum time to allow one check to run (ms|s|m|h) (default 0s)
- `--help` = Print usage
- `--hostname` or `-h` = Container host name
- `--init` = Run an init inside the container that forwards signals and reaps processes
- `--interactive` or `-i` = Keep STDIN open if not attached
- `--ip` = IPv4 address
    > Read more here : [Static IP in containers](https://stackoverflow.com/questions/27937185/assign-static-ip-to-docker-container)
- `--ip6` = IPv6 address
- `--ipc` = IPC mode to use (host or shareable or container:name)
    > Read more here : [What Is Ipc In Docker Container Command With Code Examples](https://linuxhint.com/what-is-ipc-in-docker-container-command-with-code-examples/)
- `--isolation` = Container isolation technology
- `--kernal-memory` = Kernel memory limit
    > Read more here : [What is docker --kernel-memory](https://stackoverflow.com/questions/68991039/what-is-docker-kernel-memory)
- `label` or `-l` = Set meta data on a container
    > Read more here : [Docker Labels and How to Use Them](https://forketyfork.medium.com/docker-labels-and-how-to-use-them-614ee1a4c190)
- `--label-file` = Read in a line delimited file of labels
- `--link` = Add link to another container
    > Read more here : [Legacy container links](https://docs.docker.com/network/links/)
- `--link-local-ip` = Container IPv4/IPv6 link-local addresses
- `--log-driver` = Logging driver for the container
    > Read more here : (Configure logging drivers)[https://gdevillele.github.io/engine/admin/logging/overview/]
- `--log-opt` = Log driver options
- `--mac-address` = Container MAC Address
- `--memory` or `-m` = Memory limit (ram and swap memory)
    > Read more here : (How to Limit Docker Memory and CPU Usage)[https://phoenixnap.com/kb/docker-memory-and-cpu-limit#:~:text=The%20%2D%2Dmemory%20option%20sets,not%20stop%20the%20container's%20services.]
- `--memory-reservation` = Memory soft limit (Just warns if ram is used further)
- `--memory-swap` = Swap limit equal to memory plus swap: '-1' to enable unlimited swap
- `--memory-swappiness` or `-1` = Tune container memory swappiness (0 to 100)
- `--mount` = Attach a filesystem mount to the container
- `--name` = Assign a name to the container
- `--net` = Connect a container to a network
- `--net-alias` = Add network-scoped alias for the container
- `--network` = Connect a container to a network
- `--network-alias` = Add network-scoped alias for the container
- `--no-healthcheck` = Disable any container-specified HEALTHCHECK
- `--oom-kill-disable` = Disable OOM Killer
    > Read more here : [Linux Out of Memory killer](https://neo4j.com/developer/kb/linux-out-of-memory-killer/#:~:text=The%20Out%20Of%20Memory%20Killer,allocated%20memory%20to%20its%20processes.)
- `--oom-score-adj` = Tune host's OOM preferences (-1000 to 1000)
    > Read more here : (Memory references)[https://docs.docker.com/engine/reference/run/#runtime-constraints-on-resources:~:text=The%20container%20has,scores%20more%20likely.]
- `--pid` = PID namespace to use
- `--pids-limit` = Tune container pids limit (set -1 for unlimited)
- `--platform` = Set platform if sersver is multi-platform capable
    > Read more here : [Multi platform images](https://docs.docker.com/build/building/multi-platform/#:~:text=The%20%2D%2Dplatform%20flag%20informs,the%20images%20to%20Docker%20Hub.)
- `--privileged` = Give extended privileges to this container
- `--publish` or `-p` = Publish a container's port(s) to the host
- `--publish-all` or `-P` = Publish all exposed ports to random ports
- `--pull` = Pull image before running(always, missing, never)
- `--quiet` or `-q` = Suppress the pull output
- `--read-only` = Mount the container's root filesystem as read only
- `--rm` = Automatically remove the container when it exits
- `--runtime` = Runtime to use for this container
- `--security-opt` = Security Options
    > Read more here : [Add no new privileges flag](https://cheatsheetseries.owasp.org/cheatsheets/Docker_Security_Cheat_Sheet.html#:~:text=Security%20Policies.-,RULE%20%234%20%2D%20Add%20%E2%80%93no%2Dnew%2Dprivileges%20flag,%C2%B6,-Always%20run%20your)
- `--shm-size` = Size of /dev/shm
    > Read more here : [Shared Memory & Docker](https://datawookie.dev/blog/2021/11/shared-memory-docker/)
- `--sig-proxy` = Proxy received signals to the process
    > Read more here : [Configure Docker to use a proxy server](https://docs.docker.com/network/proxy/)
- `--stop-signal` = Signal to stop the container
    > Read more here : [What does Docker STOPSIGNAL do?](https://stackoverflow.com/questions/50898134/what-does-docker-stopsignal-do)
- `--stop-timeout` = Timeout(in seconds) to stop a container
    > Read more here : [How to limit "docker run" execution time?](https://stackoverflow.com/questions/48299352/how-to-limit-docker-run-execution-time)
- `--storage-opt` = Storage driver options for the container
    > Read more here : [What does Docker run --storage-opt size=XYZ means?](https://stackoverflow.com/questions/44575197/what-does-docker-run-storage-opt-size-xyz-means)
- `--sysctl` = Sysctl options
- `--tmpfs` = Mount a tmpfs directory
- `--tty` or `-t` = Allocate a pseudo-TTY
-  `--ulimit` = Ulimit options
- `--user` or `-u` = Username or UID (format: <name|uid>[:<group|gid>])
- `--userns` = User namespace to use
- `--uts` = UTS namespace to use
- `--volume` or `-v` = Bind mount a volume
- `--volume-driver` = Optional volume driver for the container
- `--volumes-from` = Mount volumes from the specified container(s)
- `--workdir` or `-w` = Working directory inside the container
