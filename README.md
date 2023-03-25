# td1 : Use Basic Linux commands

exercice 1
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
# td2

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

