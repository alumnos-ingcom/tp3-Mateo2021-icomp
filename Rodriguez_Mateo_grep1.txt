echo "Trabajo Practico 3"

echo "(1) Imprima todas las lineas que contengan un numero de telefono con una extension seguida de cuatro digitos"

grep -Ei "^[[:digit:]]{3}-[[:digit:]]{3}-[[:digit:]]{4}[[:space:]][x]" grepdata.txt

echo "(2) Imprima todas las lineas que comiencen con tres digitos seguidos de un espacio en blanco"

grep -E "[[:digit:]]{3}[[:space:]]" grepdata.txt

echo "(3) Imprima todas las lineas que contienen una fecha"

grep -Ei "[[:alpha:]]{3}[.][[:space:]][[:digit:]]" grepdata.txt

echo "(4) Imprima todas las lineas que contienen una vocal (a,e,i,o,u) seguidas de un solo caracter seguido de la misma vocal nuevamente"

grep -iE "[a][[:alpha:]][a]" grepdata.txt

grep -iE "[e][[:alpha:]][e]" grepdata.txt

grep -iE "[i][[:alpha:]][i]" grepdata.txt

grep -iE "[o][[:alpha:]][o]" grepdata.txt

grep -iE "[u][[:alpha:]][u]" grepdata.txt

echo "(5) Imprima todas las lineas que no comiencen con una S mayuscula"

grep -Ev "^[S]" grepdata.txt

echo "(6) Imprima todas las lineas que contengan una direccion de correo electronica"

grep -E "[@]" grepdata.txt





