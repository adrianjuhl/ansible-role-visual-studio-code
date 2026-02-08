# Ansible role: visual_studio_code

Installs [Visual Studio Code](https://code.visualstudio.com), an open source code editor.

## Requirements

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

None.

## Role Variables

Role variables and their defaults.

The following role vairables are the ones that most often need a value provided that is different from their default.

See 'defaults/main.yml' for all role variables.

**blah**

    adrianjuhl__visual_studio_code__blah: "blah"

Desciption.

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

None.

## Example Playbook
```
- hosts: "servers"
  roles:
    - role: "adrianjuhl.visual_studio_code"

or

- hosts: "servers"
  tasks:
    - name: "Install Visual Studio Code"
      ansible.builtin.include_role:
        name: "adrianjuhl.visual_studio_code"

or (install into the user's ~/.local/bin directory)

- hosts: "servers"
  tasks:
    - name: "Install Visual Studio Code"
      ansible.builtin.include_role:
        name: "adrianjuhl.visual_studio_code"
      vars:
        adrianjuhl__visual_studio_code__blah: "blah"
```

## Extras

### Install script

For convenience, a bash script is also supplied that facilitates easy installation of Visual Studio Code on localhost (the script executes ansible-galaxy to install the role and then executes ansible-playbook to run a playbook that includes the visual_studio_code role).

The script can be run like this:
```
$ git clone git@github.com:adrianjuhl/ansible-role-visual-studio-code.git
$ cd ansible-role-visual-studio-code
$ .extras/bin/install_visual_studio_code.sh
```

## License

MIT

## Author Information

[Adrian Juhl](http://github.com/adrianjuhl)

## Ansible Galaxy adrianjuhl.yq role

[https://galaxy.ansible.com/ui/standalone/roles/adrianjuhl/visual_studio_code/versions/](https://galaxy.ansible.com/ui/standalone/roles/adrianjuhl/visual_studio_code/versions/)

## Source Code

[https://github.com/adrianjuhl/ansible-role-visual-studio-code](https://github.com/adrianjuhl/ansible-role-visual-studio-code)

