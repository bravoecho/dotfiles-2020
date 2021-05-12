## Installation

Only for Ubuntu / Debian, and only the versions supported by the Node.js apt
repositories.

1. Make sure `git` is already installed.
1. Golang: `./scripts/golang`. It will remove the current `go` runtime if
   present. Run it before `./scripts/setup` if you want to have vim-go support
   correctly set up.
1. Google Cloud SDK: `./scripts/google-cloud-sdk`: if a local GCP SDK is
   present for the current user in the standard location, it will update it and
   install additional modules, otherwise it will install it.
1. Install basic packages and symlink dotfiles: `./scripts/setup` (it will
   backup existing dotfiles if any).
1. Install docker and docker-compose
   * `./scripts/docker` will install Docker from the official Docker apt
     repository, so later it will be updated by `apt-get upgrade`
   * `./scripts/docker-compose` will install the latest docker-compose from
     the website, and the same script will be used for updating later
