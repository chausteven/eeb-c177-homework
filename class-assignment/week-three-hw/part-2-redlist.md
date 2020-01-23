# #1 
```
cut -d "," -f 10 European_Red_List.csv | tail -n +2 | sort -d | uniq -c
```

# #2
```
cut -d "," -f 4,10 European_Red_List.csv | tail -n +2 | sort -d | grep -w "AVES"| uniq -c
```

# #3
```
cut -d "," -f 4-5,10 European_Red_List.csv | grep -w "AVES" | sort -d | grep -w 'EX\|RE\|CE' | uniq -c
```