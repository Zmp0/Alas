#### Installation

move the alas file into /usr/local/bin,but for make it ,it need root permission, so automate it with this code

```
git clone https://github.com/Zmp0/Alas.git && cd Alas && sudo cp alas /usr/local/bin && sudo chown $USERNAME /usr/local/bin/alas && chmod +x /usr/local/bin/alas
```
if you want to modify it:

```

$ nano /usr/local/bin/alas

```

#### Description

- a simple command to add aliases to the .bashrc file and source it afterwards

- this works only for bash shell, if you have zsh or fish modify a little the code 

- it have 2 modes,one for add an alias and one for remove it


the first one is 

```

$ alas alias_name "alias_command"

```

for example:

```

$ alas p "clear"

```

and for more phrases:

```

$ alas upd "sudo apt update && sudo apt upgrade -y"

```

and for the remove mode:

```

$ alas -r alias_name

```

for example: 

```

$ alas -r upd 
$ alas -r p

```

make a source .bashrc alias because the source config file into the script doesn't work,so if you wanna speed up create a alias for source the bash config file

i have this alias and i add also clear ,but make as you wish 

```

alias sb='source ~./bashrc && clear'

```
