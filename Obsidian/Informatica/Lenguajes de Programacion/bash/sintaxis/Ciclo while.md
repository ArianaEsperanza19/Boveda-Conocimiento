```bash
#!/bin/bash
contador=1 
while [ $contador -le 10 ]; 
do echo "Iteración: $contador" contador=$((contador + 1)) 
done
```