# Plano de Codificação e Testes

Considerando a aplicação da modelagem funcional no desenvolvimento do software, a codificação será realizada combinando os paradigmas de programação funcional e orientada a objetos.

Optaremos pela linguagem de programação Python para a codificação, uma vez que ela se destaca como a mais adequada para o desenvolvimento ágil de aplicações de pequena escala com interface de linha de comando.

Adotaremos o método de "REPL-driven development" durante o processo de codificação, utilizando o ambiente de desenvolvimento integrado Jupyter Lab para facilitar a sua implementação.

Posteriormente, após a codificação com RDD, procederemos à elaboração de testes unitários automatizados, utilizando a ferramenta pytest, a fim de proporcionar uma camada adicional de segurança em relação à correção do código.

Para representar os pontos em um sistema de coordenadas cartesianas necessários para a plotagem de gráficos de funções, faremos uso da biblioteca NumPy em Python. Para a plotagem efetiva dos gráficos, utilizaremos a biblioteca Matplotlib, também em Python.

## Módulo entrada/saida - es.py

### 1. Requisito 1b

Plotar o gráfico

função impressora(grafico: objeto gráfico) -> null
Esta função imprime na tela o gráfico da função escolhida pelo usuário.

### 2. Requisito 2

Deve haver um menu com as quatro funções capazes de serem plotadas pelo aplicativo.

função leitor_funcao() -> string
Imprime um menu na tela contendo as funções afim, quadrática, logarítmica e exponencial para o usuário escolher qual delas plotar.

### 3. Requisitos 3 e 4

 Caso o usuário escolha a função afim, na sequência, ele deverá poder informar os coeficientes da função.

- Idêntico ao requisito 2, mas sendo válido para função quadrática.

função leitor_coeficiente(nome_funcao: string) -> lista
Lê os coeficientes no caso de o usuário escolher plotar uma função afim ou quadrática.

## Módulo de processamento de gráficos (designer)

Este módulo deverá prover uma função para plotar o gráfico da função escolhida pelo usuário.

### 1. Requisito 1a

Determinar o gráfico

função design(tipo_funcao: str, coeficientes: lista) -> objeto gráfico
Esta função recebe o tipo de função a ser desenhada e a lista de coeficientes (se for necessário) e desenha o gráfico da função correspondente.
