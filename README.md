# cool-terminal-setup-
A guide to customize your terminal with Zsh, Oh My Zsh, Powerlevel10k, and cool fonts.

# Cool Terminal Setup Guide

**Author:** CYB3R T3CH AJJU

This guide will show you how to customize your Linux or macOS terminal using **Powerlevel10k** and the **Zsh** shell for a more personalized and efficient experience.

![image](https://github.com/user-attachments/assets/c34117ea-f21a-422a-81a8-3379f6c9f8f6)


---

## Zsh

For this customization, you'll need **Zsh**. If you're using Kali Linux or macOS, Zsh is installed by default. To check if Zsh is your current shell, use the following command:

```bash
echo $SHELL
```

If Zsh is not installed, run the following command on your Debian-based Linux OS:

```bash
sudo apt install zsh
```

After installation, set Zsh as the default shell:

```bash
chsh -s /usr/bin/zsh
```

Now Zsh is installed. Close your terminal and reopen it with Zsh.

---

## Install Oh My Zsh

To set up Zsh themes, install **Oh My Zsh** by running:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

---

## Install Powerlevel10k

Once Oh My Zsh is installed, install the **Powerlevel10k** theme:

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

Edit your `.zshrc` file to set Powerlevel10k as the theme:

```bash
nano ~/.zshrc
```

Change the `ZSH_THEME` line to:

```bash
ZSH_THEME="powerlevel10k/powerlevel10k"
```

Save the file and restart your terminal.

---

## Install Fonts

### Install Powerline Fonts

```bash
sudo apt install fonts-powerline
```

### Install Nerd Fonts

1. Create a fonts directory:
   ```bash
   mkdir -p ~/.local/share/fonts
   ```
2. Navigate to this directory:
   ```bash
   cd ~/.local/share/fonts
   ```
3. Download a Nerd Font:
   ```bash
   curl -fLO https://github.com/ryanoasis/nerd-fonts/raw/HEAD/patched-fonts/DroidSansMono/DroidSansMNerdFont-Regular.otf
   ```

---

## Configure Powerlevel10k

Restart your terminal. The Powerlevel10k configuration wizard should start automatically. If it doesn’t, run:

```bash
p10k configure
```

## Enable Command Suggestions

To enhance your terminal experience, you can enable **command suggestions** and **syntax highlighting**.

### Step 1: Install Zsh Autosuggestions
This plugin suggests commands based on your history as you type.

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
```

### Step 2: Install Zsh Syntax Highlighting
This plugin highlights commands and syntax for easier readability.

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.zsh/zsh-syntax-highlighting
```

### Step 3: Update .zshrc
Open your `.zshrc` file and add the following lines:

```bash
# Enable Zsh Autosuggestions
source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh

# Enable Zsh Syntax Highlighting
source ~/.zsh/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```

Ensure these lines are **below** the Powerlevel10k initialization line:

```bash
[[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh
```

### Step 4: Apply Changes
Reload your terminal configuration:

```bash
source ~/.zshrc
```

### Step 5: Verify Command Suggestions
- **Command Suggestions:** Start typing a previously used command to see it suggested in a lighter color.
- **Syntax Highlighting:** Watch for colorful syntax highlighting while typing commands.

Enjoy a smarter terminal experience! 🎉
Follow the prompts to customize your terminal's appearance.

---

### Subscribe for More!

For more tutorials, subscribe to [Cyber Tech Ajju YouTube Channel]([http://youtube.com/techchipnet](https://youtube.com/@cybertechajju?si=rpQqtCgZ4eE12Rsa)).

---

Happy customizing! 😊
