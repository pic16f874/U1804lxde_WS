ansible-playbook -i hosts 01-centos7-setup.yml --user kivanov --become --become-method sudo
# Run playbook
#
# gpasswd -a demo wheel
# ВАШ_НИК ALL=(ALL:ALL) NOPASSWD: ALL
#

cd ~/Downloads/U1804lxde_WS/ansible/

ansible-playbook -i hosts 01_U18.04-lxde_setup.yml --user <user> --become --become-method sudo --ask-pass --ask-become-pass --step
ansible-playbook -i hosts 01_U18.04-lxde_setup.yml --user <user> --become --become-method sudo --ask-become-pass --step
