# Apt key automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-aptkey
  name: ansible-role-aptkey
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-aptkey

- Import role and override role variables, e.g.
```
- name: Download and install keys
  roles:
    - role: ansible-role-aptkey
```

- All available role vars can be found in `defaults`
