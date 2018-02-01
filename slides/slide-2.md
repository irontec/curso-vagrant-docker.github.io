##  Slide 2

Ejemplo bash
```bash
#!/bin/bash
if [ "$UID" -ne 0 ]
then
 echo "Superuser rights required"
 exit 2
fi

echo "ii" > /dev/null
```
