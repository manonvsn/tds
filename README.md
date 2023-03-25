# TD1.2 : Use Basic Linux commands

Exercice 1
``` 
1) cd /
2) ls -l
3) pwd
4) mkdir test
5) cd /home
6) cd ~
7) cd ..
9) cd home
10) mkdir test
11) cd test
11)pwd
``` 

Exercice 2
``` 
1) cd ~
2) pwd
3)mkdir linux_ex1
4)cd linux_ex1
5) > manon_voisin.txt
6) mkdir notes
7)mv manon_voisin.txt notes/
8)mv notes/manon_voisin.txt notes/manon_voisin_2023.txt
9)cp -r notes notes_2022
10)rm -rv notes

```
Exercice 3

``` 
1) nano linux_ex_1/script_1.sh
2)echo "Script running please wait ..."
echo "Done."
3) ctrl x
4) cat linux_ex_1/script_1.sh
5) source linux_ex_1/script_1.sh
``` 

Exercice 4.1

```
1) echo "blabla" > linux_ex_1/credentials
cat linux_ex_1/credentials
ls -l linux_ex_1/credentials

2) chmod u-w linux_ex_1/credentials
ls -l linux_ex_1/credentials
nano linux_ex_1/credentials
cat linux_ex_1/credentials

3)chmod a+rw linux_ex_1/credentials
```
```
1) chmod a+x linux_ex_1/credentials
2) chmod a-r linux_ex_1/credentials
3)chmod a+rwx linux_ex_1/credentials
```
Exercice 4.2

```
1)cd /

2) sudo nano .private_file
sudo cat .private_file
sudo ls -la /

3)nano .private_file
cat .private_file

4)sudo nano .private_file
sudo cat .private_file

5) sudo chmod a+rwx .private_file

```

Exercice 4.4

```
1) sudo apt update
2) sudo apt upgrade
3) sudo apt install cmatrix
4) cmatrix
6) sudo apt install tmux
7) tmux
11)tmux new-session -s session1
14) tmux ls
15)tmux attach-session -t session0
17)tmux attach-session -t session1
18)tmux ls
19)tmux kill-server
20)tmux ls

```

# TD1.2 : Fundamental Linux functionalities

Exercice 1

```
1) sudo apt update && sudo apt upgrade

2)uname -a
top
htop
nproc
lscpu
df -h
mount
lsusb
hostname
```

Exercice 2

```
1) x="piri pimpin"
2) echo $x
3) x=$x" piri pimpon"
4) mkdir my_programs
cd my_programs
5) echo "pilou pilou" > pilou.sh
6) ./pilou.sh
7)chmod +x pilou.sh
9) echo $PATH
10)export PATH=$PATH:$(pwd)
12)cd ~
12)pilou
13)nano .profiles
export PATH=$PATH:/home/my_programs/pilou.sh
```
# TD2.1 : Linux Grep

exercice 1
``` 
1) ls -l /
```
```
2) ls-l / | grep bin
```
```
3) ls -l / | grep bin | awk '{print $5}'
```
```
4) ls -l / | grep bin | awk '{print $6 $7 $8}'
```

```
5) ls -l / | grep bin | awk '{print $8 "-" $6 "-" $7}'
```

Exercice 2
``` 
1)curl https ://en.wikipedia.org/wiki/List_of_cyberattacks > cyberattacks.txt
```
```
2) cat cyberattacks.txt | grep "meta"
```
```
3) grep -o -E "meta [[:alpha:]]+" cyberattacks.txt
```
```
4) grep -o -E "meta [[:alpha:]]+" cyberattacks.txt | awk '{print$2}'
```
```
5)cat cyberattacks.txt | grep -P ’A cyberattack is’
cat cyberattacks.txt | grep -P ’A <a href="/wiki/Cyberattack" title="Cyberattack">cyberattack</a> is any type’
cat cyberattacks.txt | grep -A1 ’mw-content-text’ | grep -v ’mw-content-t
```
```
6) grep -oP '<title>\K.*(?= - Wikipedia</title>)' cyberattacks.txt
```

# TD 3: Git Local

Exercice 1
``` 
1) git --version
2) git config --global user.name "manon"
git config --global user.email "manon.voisin@edu.ece.fr
3) git config --list
```
Exercice 2
``` 
1) mkdir repo
cd repo
git init
2) ls -a
3) git status
4) echo "# test repository" > readme.md
5) git status
6) git add readme.md
7) git status
8) git commit -m "Add readme.md file"
9) git status
10) git log
```

Exercice 3
``` 
1) > main.py
functions.py
2) git status
3) git add main.py
4) git status
5) git commit -m "Add main.py file"
6) git add functions.py
git commit -m "Add functions.py file"
9) git log
```
Exercice 4
``` 
1) > requirements.txt
> .gitignore
> .private
2) git status
3) git add .
5) git commit -m "Add 3 files"
7) git log --oneline
```
Exercice 5
``` 
1) > temp.ipynb
2) git status
3) echo "temp.ipynb" >> .gitignore
5) > temp.aux
> temp.log
7) echo "temp*" >> .gitignore
9) echo ".private/" >> .git/info/exclude
```

Exercice 6
``` 
1) echo "# My Test Repository" > readme.md
2) git add readme.md
3) git diff HEAD
4) git commit -m "Add description to readme.md"
5) git diff HEAD~1 HEAD
6) git diff HEAD~1
7)nano readme.md
8)git diff HEAD
```


