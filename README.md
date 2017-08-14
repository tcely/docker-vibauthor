# docker-vibauthor
A docker image for creating VMware *.vib files

*Examples*:

- docker build --force-rm --pull -t "vibauthor:$(date +%Y%m%d)" vibauthor && docker tag "vibauthor:$(date +%Y%m%d)" vibauthor:latest

- docker run --rm -v "${PWD}:/data" vibauthor | less -XF

- docker run --rm -v "${PWD}:/data" vibauthor -i -v fwrule-ntpServer-1.0.0-1.vib | less -XF

- docker run --rm -v "${PWD}:/data" --entrypoint '/bin/bash' -it vibauthor
