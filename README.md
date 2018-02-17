# docker-vibauthor
A docker image for creating VMware *.vib files

*Examples*:

- docker run --rm -v "${PWD}:/data" vibauthor | less -XF

- docker run --rm -v "${PWD}:/data" vibauthor -i -v fwrule-ntpServer-1.0.0-1.vib | less -XF

- docker run --rm -v "${PWD}:/data" --entrypoint '/bin/bash' -it vibauthor

*Documentation*:
- https://download3.vmware.com/software/vmw-tools/vibauthor/vibauthor.pdf
