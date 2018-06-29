# bug_packer_ansible

## Packer issue

[packer_issue](https://github.com/hashicorp/packer/issues/6438)

## Build

    virtualenv venv
    source venv/bin/activate
    (venv) pip install ansible==2.6.0 pywinrm
    (venv) ./packer build windows_10.json

This should output:

    "msg": "Invalid settings supplied for use_tty: 'connection'"

## Note

I provided another template named `windows_10_ansible_local.json`.

It is running `ansible-playbook` as `shell-local` provisioner, without using the packer communicator plugin.
