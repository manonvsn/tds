# td2

exercice 1
``` 
1) ls -l /
```
```
2) ls-l / | grep bin
```

3) ls -l / | grep bin | awk '{print $5}'
```
4) ls -l / | grep bin | awk '{print $6 $7 $8}'
```

5) ls -l / | grep bin | awk '{print $8 "-" $6 "-" $7}'
```

Exercice 2
``` 

1)curl https ://en.wikipedia.org/wiki/List_of_cyberattacks > cyberattacks.txt
```
2) cat cyberattacks.txt | grep "meta"
```

3) grep -o -E "meta [[:alpha:]]+" cyberattacks.txt
```
4) grep -o -E "meta [[:alpha:]]+" cyberattacks.txt | awk '{print$2}'
```
5)cat cyberattacks.txt | grep -P ’A cyberattack is’
cat cyberattacks.txt | grep -P ’A <a href="/wiki/Cyberattack" title="Cyberattack">cyberattack</a> is any type’
cat cyberattacks.txt | grep -A1 ’mw-content-text’ | grep -v ’mw-content-t
  
```
6) grep -oP '<title>\K.*(?= - Wikipedia</title>)' cyberattacks.txt
```

