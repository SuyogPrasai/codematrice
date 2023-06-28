# Transforming Ubuntu to the Next Level

In this post, I will be continuing the installation of Ubuntu WSL on Windows. I will be now transforming it to the next level. The software that I will be using will be Windows Terminal, Ubuntu, and Fish Shell.
<!--more-->

### Preparation

- First of all, we must update the Ubuntu Package lists and also the software that's installed in the default installation. So, to do that run the following command: 
```shell 
sudo apt update && sudo apt upgrade
```
- It's going to take a while as we are updating the Ubuntu Package lists along with the all packages in the system.

### Windows terminal

In this installation, I will primarily use Windows Terminal to use WSL and any other kind of shell. It is my preferred choice for doing any shell work in Windows. Here are some reasons to run Windows Terminal:
    
- Windows Terminal is a highly customizable application for using any kind of shell in Windows  
- It is quite fast and has a lot of features which make it very tempting. 
- It has quite a good and simple configuration which makes it very easy to configure. 

### Downloading and Installing Nerd Fonts 

By default, Windows Terminal uses the Consolas font. It is good but it does not have the required graphics and options that are required in this installation. A really good option for all the graphics and symbols is using the [Nerd Fonts](https://nerdfonts.com).

- You can go to their [website](https://nerdfonst.com/font-downloads) and download your favourite font. In this installation, I will be installing the [CodeNewRoman](https://github.com/ryanoasis/nerd-fonts/releases/download/v3.0.2/CodeNewRoman.zip) Nerd Font. You can choose the font of choice. 

{{< image src="nerd_font_installation.jpg" caption="Nerd Font Installation" alt="Nerd Font Installation">}}

- You must install the font for **all the users** in your system to avoid problems. You must do it by extracting the zip file you downloaded using 7zip or Winrar. Then you must go inside the folder where you extracted the files. Then you must select all the font files. 
They are generally with extension ".ttf" or ".otf". Then right-click and click on "Install for all the users".

- After, Installing the font you must go to the settings of your Windows terminal. From there you must go into your appearance settings for your Ubuntu Profile. 

{{< image src="profile_setting.jpg"  caption="Settings" alt="Settings Image" >}}

- From the appearance settings, you must select the font that you just downloaded in the font selection menu. 

{{< image src="fonts_selection.jpg" caption="Fonts Selection" alt="fonts_selection Image">}}

- If all goes well then you have successfully installed the fonts required. Now you can proceed to the next steps. The fun part begins now.

### Installing the Fish shell 

Fish Shell is a really powerful shell that has a lot of inbuilt features like auto-suggestion, syntax highlighting, and tab completions that work with no configuration required. So, I will be installing the fish shell. 

- First of all, we must add the Fish repository in Ubuntu as it allows us to grab the latest version of Fish.

```shell
sudo apt-add-repository ppa:fish-shell/release-3
```

- Then, we must Install the fish shell. 
```shell 
sudo apt install fish
```

- Then, we must make fish shell the default shell 
    - First, we have to know the path of the fish shells. Just run
    `which fish` and it should give you the path to the fish shell.
    - Then, we have to make it our default shell
    ```shell
    sudo chsh -s <path-to-fish-shell>
    ```

- Then we have to install [oh-my-fish](https://github.com/oh-my-fish/oh-my-fish). Just run the following command to install it.
```shell
curl https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install | fish
```
- Now with oh-my-fish, you can choose various plugins and themes for your fish installation. Just type `omf theme` and it should give you a bunch of options. 

{{< image src="omf_theme.jpg" caption="omf_theme" >}}
- For this installation, I will be installing the `sashimi` theme. 
```shell
omf theme sashimi
```

- Then you have to configure the fish shell with various aliases and shortcuts. You can see how you can configure fish shell [here](https://fishshell.com/docs/current/index.html)

- You can also see my configuration on my [GitHub](https://github.com/SuyogPrasai/dotfiles/blob/master/fish/.config/fish/config.fish)

### Conclusion 
In this post, we have continued the installation of Ubuntu WSL on Windows, taking it to the next level. By utilizing Windows Terminal, Nerd Fonts, and the Fish Shell, we have enhanced the shell experience. With a highly customizable and feature-rich environment, we have created a seamless and visually appealing workspace. By following the outlined steps, readers can transform their Ubuntu WSL installation, unlocking greater productivity and convenience.

