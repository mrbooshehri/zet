# Generate random number and sign

## Number

```bash
echo $((RANDOM % 9000 + 1000))
#for i in {1..10}; do echo $((RANDOM % 9000 + 1000)); done
```

## Sign

```bash
echo $(tr -dc '[:punct:]' < /dev/urandom | tr -d '[:digit:]' | head -c 3)
#for i in {1..10}; do echo $(tr -dc '[:punct:]' < /dev/urandom | tr -d '[:digit:]' | head -c 3); done0
```

Tags:
```
#linux #password #pass #random
```
