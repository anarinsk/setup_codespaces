# setup_codespaces

## Codespaces 생성 
- 브랜치별로 따로따로 생성할 수 있다. 어쨌든 생성하자. 

## Post generation 

- 생성 이후에는 Ubuntu의 일반적인 절차를 따르면 된다. 
- https://github.com/anarinsk/setup-wsl-daily_use

### Update and upgrade 

```bash
> sudo apt-get update
> sudo apt-get upgrade -y 
> sudo apt-get update && sudo apt-get full-upgrade -y # All in One! 
```

- 리포 소스를 굳이 카카오로 바꿀 필요는 없을 듯? 

### zsh and ...

- zsh이 기본으로 잡혀 있는 듯 싶다. 아니라면 아래 참고. 

```bash
 install required packages
> sudo apt install zsh git curl -y

# verify zsh installation
> zsh --version

# Set the default shell to zsh
> sudo chsh -s $(which zsh) $(whoami)

# Install oh-my-zsh: https://ohmyz.sh
> sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Install Powerlevel10k: https://github.com/romkatv/powerlevel10k
> git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

- p10k까지 깔아야할까? 

### Brew 

- brew를 설치하고, pixi 등은 이 녀석으로 깔자. 

### Non Brew 

- 