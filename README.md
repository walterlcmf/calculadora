#!/bin/bash
 
echo "Digite o primeiro número:"
read num1
 
echo "Digite o segundo número:"
read num2
 
if [ $num1 -eq 0 ] || [ $num2 -eq 0 ]; then
    echo "Não calculamos divisão por zero."
elif [ $num1 -lt $num2 ]; then
    echo "O primeiro número deve ser maior que o segundo para evitar números decimais na divisão>
else
    soma=$((num1 + num2))
    sub=$((num1 - num2))
    multi=$((num1 * num2))
    div=$((num1 / num2))
 
    echo "O resultado da soma é: $soma"
    echo "O resultado da subtração é: $sub"
    echo "O resultado da multiplicação é: $multi"
    echo "O resultado da divisão é: $div"
fi
