# Calculando Limites, Derivadas e Integrais com SymPy em Python

Este projeto demonstra como utilizar a biblioteca SymPy para calcular limites, derivadas e integrais em Python. 
O SymPy é uma poderosa biblioteca de álgebra simbólica que permite manipular expressões matemáticas de forma simbólica e realizar cálculos exatos.

## Pré-requisitos
Antes de executar o código, certifique-se de que o Python está instalado no seu sistema. 
Além disso, você precisará instalar a biblioteca SymPy. Para instalar, execute o seguinte comando:
pip install sympy

## Funcionalidades do Código
O script apresentado realiza os seguintes cálculos matemáticos utilizando o SymPy:
1. Definição de Variáveis Simbólicas:
   - O código define as variáveis simbólicas x e y para trabalhar com expressões simbólicas.
2. Cálculo de Limite:
   - Calcula o limite da expressão (x**2 - 1)/(x - 1) quando x se aproxima de 1. O SymPy retorna o resultado simbólico do limite.
3. Cálculo de Derivada:
   - Calcula a derivada da função f(x) = x**3 + 2*x**2 + 3*x + 4 em relação a x. O SymPy fornece a expressão da derivada como resultado.
4. Cálculo de Integral:
   - Calcula a integral indefinida da expressão x**2 + x + 1 em relação a x. O resultado é apresentado como uma expressão simbólica.

Estrutura do Código
O código segue a seguinte estrutura:

import sympy as sp

Definição de variáveis simbólicas
x, y = sp.symbols('x y')

Cálculo do limite
lim = sp.limit((x**2 - 1)/(x - 1), x, 1)
print(lim)

Cálculo da derivada
f = x**3 + 2*x**2 + 3*x + 4
derivada = sp.diff(f, x)
print(derivada)

Cálculo da integral
integral = sp.integrate(x**2 + x + 1, x)
print(integral)


## Saída Esperada
1. Ao executar o código, o terminal exibirá os seguintes resultados:
   - Resultado do limite: 2
   - Resultado da derivada: 3*x**2 + 4*x + 3
   - Resultado da integral: x**3/3 + x**2/2 + x + C (onde C é a constante de integração).
## Observações
   - O SymPy retorna os resultados em formato simbólico. Caso deseje obter valores numéricos, você pode substituir valores específicos nas variáveis usando o método .subs() ou converter expressões para valores numéricos com .evalf().
   - Este exemplo foi elaborado para fins educacionais e pode ser expandido para incluir cálculos mais avançados ou aplicações específicas.

