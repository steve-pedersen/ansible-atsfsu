# Ansible Playbook for Academic Technology (at.sfsu.edu)


# Example deploy commands:

To deploy the Fresca application to its test server:
$ ansible-playbook master.yml -i inventory --limit "fresca-test" --ask-vault-pass
$ ansible-playbook master.yml -i inventory --limit "fresca-test" --ask-vault-pass --check