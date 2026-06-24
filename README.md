# ansible-my-machine

Platform engineer workstation provisioning via Ansible.

## Quick Start

```bash
ansible-playbook playbook.yml --ask-become-pass
```

## What it installs

### APT Packages
- **Base:** git, curl, wget, make, build-essential, gnupg, unzip
- **Python:** python3, pip3, python3-venv
- **K8s/Cloud:** kubectl, google-cloud-cli, helm, docker-ce
- **Terminal:** zsh, fzf, jq, btop, htop, tree, tmux, terminator, nmap, shellcheck
- **Ansible**

### Snap Packages
- **Classic:** code (VS Code), go, aws-cli, slack
- **Strict:** spotify, yq, kustomize, terraform-docs

### Binary Downloads (to /usr/local/bin)
- **K8s tools:** kubectx, kubens, argocd, istioctl, stern, velero, crane, kind
- **IaC:** terragrunt
- **Dev productivity:** lazygit, delta (git diff), shfmt (shell formatter)

### APT Packages (additional)
- bat (cat with syntax highlighting)

### asdf Version Manager
- Plugins: terraform, terragrunt, lefthook

### Oh My Zsh + Plugins
- zsh-autosuggestions, zsh-syntax-highlighting, zsh-history-substring-search, kube-ps1

### pip Modules
- docker, boto3, botocore

## Tools managed outside this playbook
- **k9s:** installed from source at `~/personal_repos/k9s/execs/k9s`
- **Terraform/Terragrunt versions:** managed via asdf
