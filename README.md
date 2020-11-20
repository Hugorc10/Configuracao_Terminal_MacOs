# Configuração Terminal
Terminal com Oh My Zsh, Spaceship, Dracula e mais

Instalando Zsh

Antes de conseguirmos iniciar com qualquer configuração precisamos instalar o Zsh. Como existem várias formas de instalação dependendo do sistema operacional que você está, leia esse guia: https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH

Com o Zsh instalado deve ser possível você executar:

zsh --version
E receber algo como: zsh x.x (x86_64-apple-darwin20.0)

Instalando Oh My Zsh

Para instalar o Oh My Zsh você precisa executar o comando abaixo (você deve ter o cURL instalado para executa-lo):

sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
A partir de agora todas configurações que você quer fazer como adicionar variáveis ambientes ou configurar seu terminal de qualquer forma utilize o arquivo ~/.zshrc e não mais o ~/.bash_profile ou derivados.

Utilizando Dracula

Dracula é um padrão de cores disponível para muitas aplicações de desenvolvimento e hoje utilizo esse esquema em boa parte dos apps em que desenvolvo.

O Dracula está disponível para muitos terminais e você pode conferir todos aqui: https://draculatheme.com na seção "Terminal".

Se você estiver no Mac usando o Terminal padrão, provavelmente irá usar: https://draculatheme.com/terminal/

Se você estiver no Linux com uma distribuição que usa Gnome, vai utilizar: https://github.com/dracula/gnome-terminal
