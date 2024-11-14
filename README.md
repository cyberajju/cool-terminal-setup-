# cool-terminal-setup-
A guide to customize your terminal with Zsh, Oh My Zsh, Powerlevel10k, and cool fonts.

# Cool Terminal Setup Guide

**Author:** CYB3R T3CH AJJU

This guide will show you how to customize your Linux or macOS terminal using **Powerlevel10k** and the **Zsh** shell for a more personalized and efficient experience.

![Terminal Screenshot](https://github.com/user-attachments/assets/be4ca301-e242-4703-b66c-5f4a28f8c193)

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

Follow the prompts to customize your terminal's appearance.

---

## Video Demo

For a step-by-step video tutorial, check out this demo:

[![P10K Demo](https://img.youtube.com/vi/j9IAvIAOVSc/0.jpg)](https://www.youtube.com/watch?v=j9IAvIAOVSc)

### Subscribe for More!

For more tutorials, subscribe to [TechChip YouTube Channel](http://youtube.com/techchipnet).

---

Happy customizing! 😊
