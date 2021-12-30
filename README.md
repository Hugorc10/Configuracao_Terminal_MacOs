# Configuração Terminal
Terminal com Oh My Zsh, Spaceship, Dracula e mais

## Instalando Zsh

Antes de conseguirmos iniciar com qualquer configuração precisamos instalar o Zsh. Como existem várias formas de instalação dependendo do sistema operacional que você está, leia esse guia: <i>https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH</i>

Com o Zsh instalado deve ser possível você executar:
```
zsh --version
```
E receber algo como: zsh x.x (x86_64-apple-darwin20.0)

## Instalando Oh My Zsh

Site do Oh My Zsh: <i>https://ohmyz.sh/#install</i>

Para instalar o Oh My Zsh você precisa executar o comando abaixo (você deve ter o cURL instalado para executa-lo):

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

A partir de agora todas configurações que você quer fazer como adicionar variáveis ambientes ou configurar seu terminal de qualquer forma utilize o arquivo ~/.zshrc e não mais o ~/.bash_profile ou derivados.

## Utilizando Dracula

Dracula é um padrão de cores disponível para muitas aplicações de desenvolvimento e hoje utilizo esse esquema em boa parte dos apps em que desenvolvo.

O Dracula está disponível para muitos terminais e você pode conferir todos aqui: https://draculatheme.com na seção "Terminal".

Se você estiver no Mac usando o Terminal padrão, provavelmente irá usar: https://draculatheme.com/terminal/

Se você estiver no Linux com uma distribuição que usa Gnome, vai utilizar: https://github.com/dracula/gnome-terminal

### Ativando tema
1. Terminal > Settings Tab
2. Click "Gear" icon
3. Click Import...
4. Select the Dracula.terminal file
5. Click Default

## Tema Spaceship

Agora vamos instalar o tema Spaceship que vai modificar um pouco as informações que são exibidas no terminal, com ele podemos mostrar a versão do Node atual, do Docker, etc.

https://github.com/spaceship-prompt/spaceship-prompt

## Instalando Spaceship

Vamos começar clonando o repositório do Spaceship em nossa pasta de themes do Oh My Zsh (é necessário ter instalado o Git pra isso):
```bash
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
```
Agora vamos criar um link simbólico para o arquivo do tema do Spaceship na pasta dos temas do Oh My Zsh:
```bash
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```
Agora dentro do arquivo `~/.zshrc` vamos alterar a variável ZSH_THEME ficando dessa forma:
```
ZSH_THEME="spaceship"
```
## Instalando FiraCode

Antes de iniciar a configuração do Spaceship precisamos instalar a fonte Fira Code que possui diversos ícones dos quais são utilizados nesse tema. Baixe o zip da última versão da fonte: [FiraCode](https://github.com/tonsky/FiraCode).

Descompacte o arquivo baixado e na pasta TTF instale os arquivos de fonte para as fontes do seu sistema (cada sistema operacional possui uma forma de fazer isso).
