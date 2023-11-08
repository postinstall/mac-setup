# Install Fonts

    cd ~/Downloads
    git clone https://github.com/romkatv/dotfiles-public.git
    open -b com.apple.FontBook dotfiles-public/.local/share/fonts/NerdFonts/*.ttf
    rm -rf dotfiles-public

# Install Homebrew

    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    (echo; echo 'eval "$(/usr/local/bin/brew shellenv)"') >> /Users/sascha/.zprofile
    eval "$(/usr/local/bin/brew shellenv)"

# Install iTerm2

    brew install iterm2 —cask
    brew install visual-studio-code --cask
    brew install python@3.12
    brew install nextcloud --cask
    brew install keepingyouawake --cask
    brew install rectangle --cask

# Install oh-my-zsh

    sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Install devops-theme

    cd ~/Downloads
    git clone https://github.com/postinstall/devops-zsh-theme.git
    cp devops-zsh-theme/devops.zsh-theme ~/.oh-my-zsh/custom/themes
    vim .zshrc
    rm -rf devops-zsh-theme

# Generate SSH-Keys

    ssh-keygen -t ed25519 -C "name@machine.local"

# Additional Software
