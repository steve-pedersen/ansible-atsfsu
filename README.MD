# Ansible Playbook for Academic Technology (at.sfsu.edu)


# Example deploy commands:

To deploy the Fresca application to its test server:

$ ansible-playbook master.yml -i inventory --limit "fresca-test" --ask-vault-pass

$ ansible-playbook master.yml -i inventory --limit "fresca-test" --ask-vault-pass --check

$ ansible-playbook master.yml -i inventory --limit "fresca-test" --ask-vault-pass --tags "taggy"

After setting vault_password_file = ~/.vault_pass.txt in ansible.cfg and storing the password in a single line, the following command works and no longer requires --ask-vault-pass:
$ ansible-playbook -l fresca-test master.yml