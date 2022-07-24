# My work environment setup 

Here is a list of my favorite tools and programs for differents work environments. Enjoy it!

[ansible installation](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-ansible-on-ubuntu)

## OS
  - [Ubuntu Desktop LTS](https://ubuntu.com/download/desktop) (linux debian family)
  - [ubuntu for IoT](https://ubuntu.com/download/iot)
  - [OH-MY-ZSH and agnoster configuration](https://www.tecmint.com/install-oh-my-zsh-in-ubuntu/)
    - [custom theme - powerlevel10k](https://stackoverflow.com/questions/61176257/customizing-powerleve10k-prompt)
    * To see theme and hide user plus the host set the following values with 
    ```shell
      ZSH_THEME="agnoster" # set agnoster theme my favority one
      
      # Add auto suggestion for command or text you typed before
      plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

      source $ZSH/oh-my-zsh.sh
      
      export DEFAULT_USER=$USER #add to hide user and host
    ```
   - [Install jq JASON processor for command line](https://stackoverflow.com/questions/33184780/install-jq-json-processor-on-ubuntu-10-04)
    `sudo apt-get install jq`

## IDEs
- [VSCode](https://code.visualstudio.com/)
- [Jetbrains Mono](https://www.jetbrains.com/lp/mono/#how-to-install)
  > Always install as default in `/usr/share/fonts`
  
  Customization / Extensions
  - [Night Owl](https://marketplace.visualstudio.com/items?itemName=sdras.night-owl), with dark mode and no italic.
  - [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2)
  - [.ENV](https://github.com/zaynali53/DotENV)
  - [ES6 code snippets](https://marketplace.visualstudio.com/items?itemName=jmsv.JavaScriptSnippetsStandard)
  - [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
  - [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
  - [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
  - [C#](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)
  - [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
  - [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur)
  - [Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
  - [Vue 3 Snippets](https://marketplace.visualstudio.com/items?itemName=hollowtree.vue-snippets)
  - [git lens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
  - [git graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
 - [Jetbrains Rider](https://www.jetbrains.com/rider/)
 
 API Testing tools
  - [Insomnia](https://insomnia.rest/download)

 ## Vidoe and Audio
 - [Celluloid](https://celluloid-player.github.io/installation.html)
  - [flatpack isntallation](https://flatpak.org/setup/Ubuntu)
 
 ## Enviroment setup
 
 ### backend / API
 
 - [nodeJS](https://nodejs.org/en/) 
 - [nodeJS installation step by step](https://linuxize.com/post/how-to-install-node-js-on-ubuntu-20-04/)
 - [.NET 5 SDK](https://docs.microsoft.com/en-us/dotnet/core/install/linux)
 - [Insomnia](https://insomnia.rest/download)
 
 ### frontend
 
 - [Vue.js 3](https://v3.vuejs.org/)
 - [react](https://reactjs.org/), mostly cause of [react nactive](https://reactnative.dev/)
 - [JEST](https://jestjs.io/) Unit and integration test of JS code
 
 ## UX design
 - [figma](https://www.figma.com/)
 - [whimsical](https://whimsical.com)
 
 ## backend deployment 
  
 - [AWS ECS and EC2](https://aws.amazon.com/ecs/)
 
 ## frontend deployment
 - [Netlify](https://www.netlify.com/)
 
 ## Organizations and productivity
 - [notion](https://www.notion.so/)
 
 ## CICD
 - [github action](https://github.com/features/actions)
 - [docker container](https://www.docker.com/resources/what-container)
 - [docker installation on ubuntu](https://docs.docker.com/engine/install/ubuntu/)
 - [nginx](https://www.nginx.com/)
 - [Helm](https://helm.sh/)
 - [k8slens](https://k8slens.dev/) - kubernetes IDE 4 pods debbunging 
 - [minikube](https://minikube.sigs.k8s.io/docs/start/) local k8s cluster
 
 ## Database
 - [Beekeeper Studio - debian](https://docs.beekeeperstudio.io/installation/#linux-installation)
 - [DBeaver](https://dbeaver.io/download/)

## Usefull commands

  ### Docker
  * [docker WSL failing to start](https://askubuntu.com/questions/1379425/system-has-not-been-booted-with-systemd-as-init-system-pid-1-cant-operate)
  ```shell
    sudo -b unshare --pid --fork --mount-proc /lib/systemd/systemd --system-unit=basic.target
  ```
  * remove all untagged images
  ```shell
    docker rmi $(docker images -f dangling=true -q) --force
  ```
  
  ### Clear npm cache
  ```bash
    yarn cache clean --force
  ```
  
  ### strat docker on WSL 2
  ```shell
    sudo -b unshare --pid --fork --mount-proc /lib/systemd/systemd --system-unit=basic.target
  ```
  
  ### Ubuntu common issue solved
  ```shell
      # network icon disappear
      nmcli network on
      
      # Bluetooth fails to start and does not show the icon. This issue happens in most the case when you have a dual boot
      sudo rmmod btusb
      sudo modprobe btusb
  ```
  
  ### [AWS SAM installation](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install-linux.html)
  ### JAVA installation
  * [install java on ubuntu ](https://linuxize.com/post/install-java-on-ubuntu-20-04/)
  * [intall without using apt - lts](https://www.javahelps.com/2019/04/install-latest-oracle-jdk-on-linux.html)
  * [maven](https://linuxize.com/post/how-to-install-apache-maven-on-ubuntu-20-04/)
  * To change jave version (`sudo update-alternatives --config java`)
  * [updating maven](https://linuxize.com/post/how-to-install-apache-maven-on-ubuntu-20-04/#2-downloading-apache-maven)
  
  ## Install taskfile
  
  ```shell
    sudo sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin
  ```
  > Instaling manually 
  ```shell
    pushd /tmp
    wget https://github.com/go-task/task/releases/download/v3.7.0/task_linux_arm.tar.gz
    tar -xvf task_linux_arm.tar.gz
    sudo mv task /usr/local/bin/task
    sudo chmod +x /usr/local/bin/task
    popd
  ```
  
  
