---
# create-users role

Adding new users with the supplementary group `wheel`.. Example vars:

```
users:
  - username: "user1"
    password: "$2b$06$5/Ov3f4sfa..."
    shell: "/bin/zsh"
    supplementary_groups:
        - wheel
        - docker
    oh_my_zsh:
    ¦ theme: robbyrussell
    ¦ plugins:
    ¦   - git
    pub_keys:
    ¦ - ssh-rsa AAAAB3NzaC1yc2EAAAADA...
    ¦ - ssh-rsa AAAAB3NzaC1yc2EAAAADA...
  - username: "user2"
    password: "$2b$08$Oq8c1Uf4..."
    shell: "/bin/bash"
```

Perfectly applied in conjunction with the [ansible-role-oh-my-zsh](https://github.com/gantsign/ansible-role-oh-my-zsh) role.
