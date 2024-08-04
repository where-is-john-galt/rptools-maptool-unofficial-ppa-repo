# rptools-maptool-unofficial-ppa-repo
Unfortunately RPTools dont publish their application on any PPA so I decided to create my own for my friend and me

# How to install

Add PGP key

```
curl -s --compressed "https://raw.githubusercontent.com/where-is-john-galt/rptools-maptool-unofficial-ppa-repo/main/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/rptools-maptool-unofficial-ppa-repo.gpg >/dev/null
```

Add repo

```
sudo curl -s --compressed -o /etc/apt/sources.list.d/rptools-maptool-unofficial-ppa-repo.list "https://raw.githubusercontent.com/where-is-john-galt/rptools-maptool-unofficial-ppa-repo/main/rptools-maptool-unofficial-ppa-repo.list"
```

Update repos

```
sudo apt update
```

install maptool

```
sudo apt install maptool
```