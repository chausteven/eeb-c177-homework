# #1
```
cut -d "," -f 3 nobel.csv | tail -n +2 | sort -d | grep -w "chemistry" | wc -l
cut -d "," -f 3 nobel.csv | tail -n +2 | sort -d | grep -w "economics" | wc -l
cut -d "," -f 3 nobel.csv | tail -n +2 | sort -d | grep -w "literature" | wc -l
cut -d "," -f 3 nobel.csv | tail -n +2 | sort -d | grep -w "medicine" | wc -l
cut -d "," -f 3 nobel.csv | tail -n +2 | sort -d | grep -w "peace" | wc -l
cut -d "," -f 3 nobel.csv | tail -n +2 | sort -d | grep -w "physics" | wc -l
```

# #2
```
cut -d "," -f 5-6 nobel.csv | sort -d | uniq -d 
```

# #3
```
cut -d "," -f 6 nobel.csv | sort -d | uniq -c | sort -n | tail -n 2
```

# #4
Most Awarded
```
cut -d "," -f 3 nobel.csv | tail -n +2 | sort -n | uniq -c | sort -n | tail -n 1
```
Least Awarded
```
cut -d "," -f 3 nobel.csv | tail -n +2 | sort -n | uniq -c | sort -n | head -n 1
```
