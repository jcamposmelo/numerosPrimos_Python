# numerosPrimos_Python
"Um número é classificado como primo se ele é maior do que um e é divisível apenas por um e por ele mesmo. Apenas números naturais são classificados como primos. Antes de saber mais sobre o número primo, é importante relembrar algumas regras de divisibilidade, que ajudam na identificação de quais números não são primos."

##

```
def eh_primo(numero):
    if numero < 2:
        return False
    for i in range(2, int(numero**0.5) + 1):
        if numero % i == 0:
            return False
    return True
numero = int(input("Digite um número: "))
if eh_primo(numero):
    print(f"{numero} é primo.")
else:
    print(f"{numero} não é primo.")
