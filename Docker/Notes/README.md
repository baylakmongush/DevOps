# 🔴 Docker Arhitecture
<br> <center> <img src="../Images/Arch.png" height="200"> </center> </br>

Docker is a client-server application with these major components:</br>
✔️ A server which is a type of long-running program called a daemon process (the dockerd command).</br>
✔️ A REST API which specifies interfaces that programs can use to talk to the daemon and instruct it what to do.</br>
✔️ A command line interface (CLI) client (the docker command).</br>

❗️Docker doesn't have kernel. Uses host kernel directly. Docker uses a technology called containerization. Containers are isolated.
## Docker container

When we run Docker container we create new namespace

**Namespace** is a feature of the Linux kernel that isolates a set of system resources from the rest of the system.</br>
A namespace provides a layer of abstraction between the resources of the host system and the resources of the container. </br>
<br>_The resources that can be isolated are:_

🚩 cgroups - control groups - limit, measure and control the resource usage (CPU, memory, disk I/O, network, etc.) of a collection of processes </br>
🚩 IPC - interprocess communication - isolate the system V IPC and POSIX message queues </br>
🚩 Mount - mount filesystem - isolate the mount table </br>
🚩 Network - network devices, stacks, ports, etc. - isolate network devices, stacks, ports, etc. </br>
🚩 Pid - process id - isolate the process tree </br>
🚩 User - user id and group id - isolate the user and group id </br>
🚩 UTS - unix time sharing - isolate kernel and version identifiers






