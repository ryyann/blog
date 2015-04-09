# Why you should use Docker
Deployment really, really sucks. This is partially because of the tendency that many have as develpers to begin work on a project without first considering the environment it will eventually be deployed into, but it's also largely because the environments available are so varied, non-standardized, and difficult to interrogate.

This is why Docker is so exciting, it's an open platform that offers the ability to ensure your app operates in a controlled, easily configurable, and flexible environment of your choosing - not just the environment offered by your chosen PaaS provider.

## What the hell is it?
The core concept provided by Docker is the idea of containerization. Apps are packaged into a container which is then deployed to a server running Docker. The container will then be run with its own, isolated, and secure, environment.

## Wait, but that's just virtualization!
No, hypothetical internet person, you're super wrong! One of the key features of Docker apps is that they do not run their own instance of the host operating system

```
root@Personal:~# docker pull dockerfile/ghost
```