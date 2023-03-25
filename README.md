# td2



exercice 1
``` 
Question 1:
ls -l
```
Question 2:
ls-l | grep bin
```
Question 3:
ls -l / | grep bin | awk '{print $5}'
```
Question 4:
ls -l / | grep bin | awk '{print $6 $7 $8}'

```
Question 5:
ls -l / | grep bin | awk '{print $8 "-" $6 "-" $7}'
```
#exercice 2

``` 
Q1:
curl https ://en.wikipedia.org/wiki/List_of_cyberattacks > cyberattacks.txt
```
Q2:
cat cyberattacks.txt | grep "meta"
```
Q3:
grep -o -E "meta [[:alpha:]]+" cyberattacks.txt
```
Q4:
grep -o -E "meta [[:alpha:]]+" cyberattacks.txt | awk '{print$2}'
```
```
```
```
```
```

