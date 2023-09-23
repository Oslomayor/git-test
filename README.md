# git test and note
2023-09-23

## useful command

### ssh key
```shell
ssh-keygen -t rsa
cat ~/.ssh/id_rsa.pub
```
github.com >> setting >> SSH and GPG key >> add new ssh  
test ssh key
```shell
ssh -T git@github.com
```
"Hi Oslomayor! You've successfully authenticated, but GitHub does not provide shell access."  

### config name,email
git config --global user.name Oslomayor  
git config --global user.email xxx@gmail.com  
git config -l  

### git init
```shell
mkdir github && cd github
git init
```

### update local file to github
```shell
touch filename
git status  
git add filename  
git commit -m "update file"  
git remote add aaa git@github.com:Oslomayor/git-test.git  
git push -u aaa main(or master)
```
