ansible-create-sudo-user
========

Create a user with sudo permissions and without prompting for sudo password.

Requirements
------------

Generate the user password as recommended by Ansible using the following command:

python -c "from passlib.hash import sha512_crypt; import getpass; print sha512_crypt.encrypt(getpass.getpass())"

After you type the password it will generate some blob. Copy this blob to defaults password variable

Role Variables
--------------

Inside defaults:

user (username you which to create)

password (password you generated above)


Author Information
------------------

Fernanda Martins (flmmartins@gmail.com)
Linkedin: https://www.linkedin.com/in/flmmartins
