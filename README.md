# ubuntu20_PPA_404

## First, restore the default focal repositories using these commands:


```
mkdir ~/solution
cd ~/solution/
wget https://raw.githubusercontent.com/sky0193/ubuntuPPA_404/main/sources.list
cp /etc/apt/sources.list sources.list_backup
sudo rm -r /etc/apt/sources.list
sudo cp -r ~/solution/sources.list /etc/apt/sources.list
```


##  Remove all the PPAs in your system:

```
sudo mv /etc/apt/sources.list.d/* ~/solution/PPAs
```

## Update the repositories:

```
sudo apt update
```

