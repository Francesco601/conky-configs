# conky-configs

![Screenshot](https://github.com/Francesco601/conky-configs/blob/main/francesco.png)

## DESCRIPTION:

These are my configuration files for the Linux system monitor program `Conky`.
I have described the modifications and syntax updates in comments in the config files.
If you have any questions about basic Conky configuration or you have trouble using these files in a simple shell script, please let me know.
Any of you graphical wizards out there who have some tips are more than welcome to share ideas and images. 



## DOWNLOAD AND USE; 

To download and use or modify on your Linux box, you will need to install git if it is not already provided by your distribution.

On Arch or Arch-based systens: 
```bash
sudo pacman -S git
```
On openSusse:
```bash
sudo zypper in git
```
On Debian/Ubuntu/Mint and variants: 
```bash
sudo apt install git.
```
You will also need to install `conky` with the same commands that you used for git. 

Create a subdirectory in your home directory named .conky where you can place the config files.
```bash
mkdir .conky
```

Then type the following into the same terminal or just copy and paste (root powers not needed):
```bash  
 git clone https://github.com/Francesco601/conky-configs  
 ```
into some subdirectory of your home directory.

Finally, copy conky.config1 and conky2.config2 into the new subdirectory or
```bash
 cp conky.config1 conky2.config2 ~/.config
````
and
```
source conkey-configs/conky-startup.sh
```
Those nice fonts that I prefer can be downloaded from <a href="https://www.dafont.com/hobbiton-brush-hand.font"> here </a>
and <a href="https://www.dafont.com/it/chinacat.font"> here </a> 

Unzip and put in .fonts directory (must be made if it doesn't exist). 

Last but not least: we can get them to run on startup several ways but the simplest is to create a symlink:

```bash 
$ cd /etc/profile.d
$ ln -s ~/.conky/conky-startup.sh startup.sh
```




See <a href="https://conky.sourceforge.net/config_settings.html"> Config settings </a> for configration settings.

And variables here: <a href="https://conky.sourceforge.net/variables.html"> Variables </a>


