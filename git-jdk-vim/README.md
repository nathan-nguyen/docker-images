# git-jdk-vim

## Build image
```sh
podman build -t git-jdk-vim .

mkdir -p home
podman run -it --user 1000:1000 -v ./home:/home/ubuntu git-jdk-vim:latest

ssh-keygen -t ed25519 -C "<email>"
```
