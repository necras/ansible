## Ansible playbook for my PDE
This is my current personal development environment, combined with my dotfiles is intended to be maintained enough to run from a newly installed debian based OS.

```sh
# run everything
ansible-playbook local.yml --ask-become-pass

# exclude tags
ansible-playbook local.yml --ask-become-pass --skip-tags "dev, neovim"

# run specific tags
ansible-playbook local.yml --ask-become-pass --tags "core"
```

### TODO
- [ ] Add peek ppa
- [ ] Make dwm installation with config idempotent, instead of removing the suckless folder
- [ ] Go installation
