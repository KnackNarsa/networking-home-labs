# Welcome!
This repo contains labs to help you learn networking concepts from the comfort of your home. Each lab contains step-by-step instructions, explaining the purpose of your steps to help you gain the understanding of what you are actually doing.

# IMPORTANT

These projects require docker to set-up the lab environments!

## UBUNTU SETUP

Install packages to allow apt to use repository over HTTPS

``bash
sudo apt update
``

Add Docker's Official GPG KEY

``bash
sudo apt install ca-certificates curl gnupg
``

Add Docker repository to apt sources

```bash
    echo \
      "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
      "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
      sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

Update apt

``bash
sudo apt update
``

Install Docker Engine, ``containerd``, and docker compose

``bash
    sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
``

Verify Docker was installed

``bash
docker --version
``

Expected output: ``Docker version 29.0.2, build 8108357``


## License

All labs in this repository are released under the [MIT License](LICENSE).
YOu are free to use, modify, and share them for learning or personal projects
