# bug_packer_ansible

## issue

[packer_issue](https://github.com/hashicorp/packer/issues/6438)

## build

    virtualenv venv
    source venv/bin/activate
    (venv) pip install ansible
    (venv) ./packer build windows_10.json

## output

    "msg": "Invalid settings supplied for use_tty: 'connection'"
