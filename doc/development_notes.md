
Ansible galaxy init command:

```
$ ansible-galaxy init adrianjuhl.visual_studio_code
```

Ansible galaxy role deployment command:

```
ansible-galaxy role import --role-name="$(yq '.galaxy_info.role_name' meta/main.yml)" adrianjuhl "$(basename "$(git remote get-url origin)" ".git")"
```

