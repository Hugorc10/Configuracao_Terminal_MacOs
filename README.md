# Configurando Terminal
Terminal com Oh My Zsh, Spaceship, Dracula e mais.


## Instalando Zsh

Antes de conseguirmos iniciar com qualquer configuração precisamos instalar o Zsh. Como existem várias formas de instalação dependendo do sistema operacional que você está, leia esse guia: <i>https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH</i>

Com o Zsh instalado deve ser possível você executar:
```
zsh --version
```
E receber algo como: zsh x.x (x86_64-apple-darwin20.0)


## Instalando Spaceship

Agora vamos instalar o tema Spaceship que vai modificar um pouco as informações que são exibidas no terminal, com ele podemos mostrar a versão do Node atual, do Docker, etc.

https://github.com/spaceship-prompt/spaceship-prompt

### Antes de começar, certifique-se de que possui o seguinte instalado:

. Zsh (v5.2 ou mais recente) deve ser instalado. Execute o seguinte comanndo para verificar a sua versão do Zsh:

```
echo $ZSH_VERSION #> 5.8.1
```

Powerline Font ou Nerd Font (melhor ainda) devem ser instaladas e usadas em seu terminal. Fira Code é uma escolha popular. Para verificar se Powerline Font funciona para você, execute:

```
echo -e "\xee\x82\xa0" #> 
```

Antes de iniciar a configuração do Spaceship precisamos instalar a fonte Fira Code que possui diversos ícones dos quais são utilizados nesse tema. Baixe o zip da última versão da fonte: [FiraCode](https://github.com/tonsky/FiraCode).

Descompacte o arquivo baixado e na pasta TTF instale os arquivos de fonte para as fontes do seu sistema (cada sistema operacional possui uma forma de fazer isso).

### Instalando

### Agora que os requisitos foram atendidos, você pode instalar o Spaceship por meio de qualquer uma das seguintes abordagens:

Clone este repositório (é necessário ter instalado o Git pra isso):

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


## Instalando Oh My Zsh

Site do Oh My Zsh: <i>https://ohmyz.sh/#install</i>

Para instalar o Oh My Zsh você precisa executar o comando abaixo (você deve ter o cURL instalado para executa-lo):

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

A partir de agora todas configurações que você quer fazer como adicionar variáveis ambientes ou configurar seu terminal de qualquer forma utilize o arquivo ~/.zshrc e não mais o ~/.bash_profile ou derivados.

## Instalando zsh-syntax-highlighting

### [Oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

1. Clone this repository in oh-my-zsh's plugins directory:

    ```zsh
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    ```

2. Activate the plugin in `~/.zshrc`:

    ```zsh
    plugins=( [plugins...] zsh-syntax-highlighting)
    ```

3. Restart zsh (such as by opening a new instance of your terminal emulator).

## Instalando zsh-autosuggestions

### Oh My Zsh(https://github.com/robbyrussell/oh-my-zsh)

1. Clone this repository into `$ZSH_CUSTOM/plugins` (by default `~/.oh-my-zsh/custom/plugins`)

    ```sh
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    ```

2. Add the plugin to the list of plugins for Oh My Zsh to load (inside `~/.zshrc`):

    ```sh
    plugins=( 
        # other plugins...
        zsh-autosuggestions
    )
    ```

3. Start a new terminal session.


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
