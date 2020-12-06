#

## Continue running after some command failed

`|| true`

e.g.

ssh symbls@192.168.1.10 "docker stop test && docker rm test" ||true