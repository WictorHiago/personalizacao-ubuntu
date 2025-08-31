# Personalização Ubuntu

Bem-vindo! Este guia reúne dicas e comandos para personalizar seu Ubuntu, instalar ferramentas essenciais e configurar seu ambiente de desenvolvimento.

## Índice

- [Temas GTK3/4](#temas-gtk34)
- [Instalação do NVM (Node Version Manager)](#instalação-nvm)
- [Gerar chave SSH para GitHub](#gerar-chave-ssh-para-github)
- [Instalar Neofetch](#instalar-neofetch)
- [Instalar Git](#instalar-git)
- [Personalização do Ubuntu](#personalização-do-ubuntu)
- [Descompactador de arquivos](#descompactador)
- [Lista de Temas](#lista-de-temas)
- [Lista de Ícones](#lista-de-ícones)

---

## Temas GTK3/4

- Midnight
- Kripton
- Sweet-Red
- Flat Remix
- Lavanda Sea
- WhiteG
- WhiteSur
- Orchis
- Andromeda
- Breeze-Gently

---

## Instalação NVM

### 1️⃣ Executar o script de instalação

Escolha uma das opções abaixo no terminal:

**Usando cURL:**
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
```

**Usando Wget:**
```bash
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
```

O script irá clonar o repositório do NVM para `~/.nvm` e adicionar as linhas de configuração ao seu arquivo de perfil (`~/.bashrc`, `~/.zshrc`, etc.).

### 2️⃣ Configurar manualmente o NVM

Se necessário, adicione manualmente ao final do seu arquivo de perfil:

```bash
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
```

Abra o arquivo de perfil do seu shell:

- Bash: `nano ~/.bashrc`
- Zsh: `nano ~/.zshrc`

Cole o snippet acima, salve e feche.

### 3️⃣ Aplicar as alterações

```bash
source ~/.bashrc   # ou
source ~/.zshrc
```

### 4️⃣ Instalar versões do Node.js

```bash
nvm install 20   # Instala a versão 20.x
nvm install 18   # Instala a versão 18.x
nvm use 20       # Usa a versão 20.x na sessão atual
nvm alias default 20  # Define a versão 20 como padrão
```

---

## Gerar chave SSH para GitHub

```bash
ssh-keygen -t ed25519 -C "seu-email@exemplo.com"
```
- Substitua `"seu-email@exemplo.com"` pelo seu email do GitHub.
- Caminho padrão: `~/.ssh/id_ed25519`
- Ou escolha outro nome, por exemplo: `/home/usuario/.ssh/id_ed25519_github`

---

## Instalar Neofetch

```bash
sudo apt install neofetch
```

---

## Instalar Git

```bash
sudo apt install git-all
```

---

## Personalização do Ubuntu

### 1. Instalar pacotes essenciais

```bash
sudo apt update
sudo apt install gnome-tweaks gnome-shell-extensions gnome-shell-extension-manager
```
- **gnome-tweaks**: Ajusta temas, fontes, ícones e animações.
- **gnome-shell-extensions**: Extensões oficiais do GNOME.
- **gnome-shell-extension-manager**: Gerencia extensões do GNOME Shell.

### 2. Ativar a extensão "User Themes"

```bash
gnome-extensions enable user-theme@gnome-shell-extensions.gcampax.github.com
```
- Depois, acesse GNOME Tweaks → Aparência → Shell para escolher o tema.

### 3. Instalar pacotes para temas GTK

```bash
sudo apt install gtk2-engines-murrine gtk2-engines-pixbuf gnome-themes-extra
```

---

## Descompactador

### Para arquivos 7z (7-Zip)

```bash
sudo apt install p7zip-full p7zip-rar
```
- **p7zip-full**: Suporta 7z, tar, gzip, bzip2, xz e mais.
- **p7zip-rar**: Suporte a arquivos .rar (somente extração).

**Exemplo de uso:**
```bash
7z x arquivo.7z             # Extrair
7z a arquivo.7z pasta/      # Compactar
```

---

## Lista de Temas

- [Kripton](https://www.gnome-look.org/p/1365372)
- [Midnight GTK Themes](https://www.gnome-look.org/p/1273208)

---

## Lista de Ícones

-