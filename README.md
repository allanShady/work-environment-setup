## 💻 Idea 
> [Ubuntu](https://ubuntu.com/download/desktop) dev environment setup automated with [ansible](https://www.ansible.com/). You can use any linux distro that is **linux debian family**


### [before we begin on ubuntu](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-ansible-on-ubuntu)

```sh
    # install ansible
    sudo apt update
    sudo apt install software-properties-common
    sudo apt-add-repository --yes --update ppa:ansible/ansible
    sudo apt install --yes ansible
```

### How to run
First, make sure you have configure your system, by updating the `vars/all.yml` and `setup.yml` files to suit your needs, by commenting things you don't want and the ones you want.

```sh
  #instal
  ansible-playbook setup.yml -e "local_username=$USER" -K
```

## 🚀 Techs

- [Ansible](https://www.ansible.com/)
- [Python3](https://www.python.org/downloads/release/python-397/)

## 🔖 Available playbooks

- [x] git
- [x] curl
- [x] dotnetcore
- [x] oh-my-zsh
- [x] rider
- [x] vscode
- [x] [nodejs](https://snapcraft.io/node)
- [ ] java
- [ ] maven
- [ ] yarn
- [ ] go-land
- [ ] docker daemon
- [ ] [OBS](https://snapcraft.io/obs-studio)
- [x] [MicroK8s](https://snapcraft.io/install/microk8s)
- [ ] [insomnia](https://snapcraft.io/install/insomnia)
- [ ] [Lens IDE](https://snapcraft.io/install/kontena-lens)
- [ ] [beekeeper studio](https://snapcraft.io/beekeeper-studio)
- [x] [dbeaver](https://snapcraft.io/dbeaver-ce)

## 🧘🏿‍ RoadMap

- [ ] Go CLI that allows selecting the desired tools
- [ ] GUI that allows selecting the desired tools
- [ ] Adapt for **Windows WSL2**
- [ ] Share achievements on social media

## :memo: Licence

This project is under MIT Licence. Please refer to [LICENSE](LICENSE.md) file for more details.

---

Build with 💜 by [**Alan Camilo**](https://allancamilo.com)