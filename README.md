### Setupmac

This is a [Ansible](https://www.ansible.com/) playbook to quickly setup a Mac.

To setup run the following command :
```
./start.sh
```

The start.sh script installs `pip` and then `ansible` with pip.
Then git clone this repository and execute the `ansible` playbook which does
all the heavy lifting of setting your mac.

If you already have ansible installed or prefer running it directly, execure the following :
```
ansible-playbook -i ./hosts playbook.yml --verbose
```


The applications it cannot install through homebrew get's downloaded to
`$HOME/Downloads`, it's up to you to install them from the Downloads directory.


#### Uninstall

Undo all the changes from this playbook

```
start.sh uninstall
```
