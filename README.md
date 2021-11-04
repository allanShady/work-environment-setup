# My work environment setup 

Here is a list of my favorite tools and programs for different work environments. Enjoy it!

## OS
  - [Ubuntu Desktop LTS](https://ubuntu.com/download/desktop) (linux debian family)
  - [ubuntu for IoT](https://ubuntu.com/download/iot)
  - [OH-MY-ZSH and agnoster configuration](https://www.tecmint.com/install-oh-my-zsh-in-ubuntu/)
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
 
 ## Enviroment setup
 
 ### backend / API
 
 - [nodeJS](https://nodejs.org/en/)
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
 - [nginx](https://www.nginx.com/)
 - [Helm](https://helm.sh/)
 
 ## Database
 - [Beekeeper Studio - debian](https://docs.beekeeperstudio.io/installation/#linux-installation)
 - [DBeaver](https://dbeaver.io/download/)

## Usefull commands

  ### Docker
  * remove all untagged images
  ```shell
    docker rmi $(docker images -f dangling=true -q) --force
  ```
  
  ### Clear npm cache
  ```bash
    yarn cache clean --force
  ```
  
  ### [AWS SAM installation](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install-linux.html)
  ### JAVA installation
  * [install java on ubuntu ](https://linuxize.com/post/install-java-on-ubuntu-20-04/)
  * [maven](https://linuxize.com/post/how-to-install-apache-maven-on-ubuntu-20-04/)
  * [updating maven](https://linuxize.com/post/how-to-install-apache-maven-on-ubuntu-20-04/#2-downloading-apache-maven)
  
