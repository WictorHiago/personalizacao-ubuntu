# personalizacao-ubuntu

### TEMAS GTK3/4
Midnight
Kripton
Sweet-Red
Flat Remix
Lavanda Sea
WhiteG
WhiteSur
Orchis
Andromeda
Breeze-Gently

### INSTALAÇÃO NVM

1️⃣ Executar o script de instalação

Você tem duas opções: cURL ou Wget. Escolha uma delas. No terminal:

Usando cURL:

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash


Usando Wget:

wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash


O script vai clonar o repositório do NVM para ~/.nvm e adicionar automaticamente as linhas de configuração ao seu arquivo de perfil (~/.bashrc, ~/.zshrc, etc.), dependendo do shell que você estiver usando.

2️⃣ Configurar manualmente o NVM (caso o script não faça automaticamente)

Se por algum motivo o script não adicionar as linhas ao perfil, você pode adicionar manualmente:

export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm


Abra o arquivo de perfil do seu shell:

Bash: nano ~/.bashrc

Zsh: nano ~/.zshrc

Cole o snippet acima no final do arquivo.

Salve e feche (Ctrl + O, Enter, Ctrl + X no nano).

3️⃣ Aplicar as alterações

Após adicionar o snippet, execute no terminal:

source ~/.bashrc
# ou se for zsh
source ~/.zshrc


Isso recarrega o arquivo de perfil e deixa o NVM disponível na sessão atual.

5️⃣ Instalar versões do Node.js

Com o NVM funcionando, você pode instalar qualquer versão do Node.js:

nvm install 20   # Instala a versão 20.x
nvm install 18   # Instala a versão 18.x
nvm use 20       # Usa a versão 20.x na sessão atual
nvm alias default 20  # Define a versão 20 como padrão


### GERAR CHAVE SSH PARA GITHUB
ssh-keygen -t ed25519 -C "seu-email@exemplo.com"

Substitua "seu-email@exemplo.com" pelo seu email do GitHub.

Quando perguntar o caminho para salvar, você pode pressionar Enter para usar o padrão (~/.ssh/id_ed25519) ou fornecer outro nome, por exemplo:

/home/usuario/.ssh/id_ed25519_github


### NEOFETCH

sudo apt install neofetch

### INSTALAR GIT

sudo apt install git-all

### PERSONALIZAÇÃO DO UBUNTU

✅ 1. Instalar pacotes essenciais

Abra o terminal e execute:

sudo apt update
sudo apt install gnome-tweaks gnome-shell-extensions gnome-shell-extension-manager


gnome-tweaks: permite ajustar temas, fontes, ícones e animações.

gnome-shell-extensions: conjunto oficial de extensões do GNOME.

gnome-shell-extension-manager: ferramenta gráfica para gerenciar extensões do GNOME Shell.

✅ 2. Ativar a extensão "User Themes"

Para aplicar temas no GNOME Shell (barra superior, menus), ative a extensão "User Themes":

gnome-extensions enable user-theme@gnome-shell-extensions.gcampax.github.com


Após isso, no GNOME Tweaks → Aparência → Shell, você poderá escolher o tema desejado.

✅ 3. Instalar pacotes para temas GTK

Alguns temas requerem pacotes adicionais para garantir compatibilidade com temas GTK2/GTK3:

sudo apt install gtk2-engines-murrine gtk2-engines-pixbuf gnome-themes-extra


### DESCOMPACTADOR

2️⃣ Para arquivos 7z (7-Zip)
sudo apt install p7zip-full p7zip-rar


p7zip-full → suporta 7z, tar, gzip, bzip2, xz e mais

p7zip-rar → adiciona suporte a arquivos .rar (somente extração, rar é proprietário)

Exemplo de uso:

7z x arquivo.7z             # Extrair
7z a arquivo.7z pasta/      # Compactar


### LISTA DE TEMAS
KRIPTON: https://www.gnome-look.org/p/1365372
MIDNIGHT GTK THEMES: https://www.gnome-look.org/p/1273208

### LISTA DE ICONS
ARS DARK ICONS: https://www.gnome-look.org/p/2192428
SWEET FOLDERS: https://www.gnome-look.org/p/1284047