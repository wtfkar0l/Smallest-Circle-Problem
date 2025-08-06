Criado por ANA KAROLINA COSTA DA SILVA em *27/09/2024*.

**Instituto Tecgraf | PUC-RIO | VISGRAF**

# Círculo Mínimo - Algoritmo de Welzl

Este projeto implementa o algoritmo de Welzl para encontrar o círculo mínimo que circunscreve um conjunto de pontos em um plano 2D. O código também inclui funções auxiliares para testes em diferentes cenários, como pontos coincidentes, colineares, pontos aleatórios, e círculos conhecidos para validação da precisão do algoritmo.

## Funcionalidades

- **Cálculo do Círculo Mínimo**: Encontra o menor círculo que contém um conjunto de pontos em \\( \\mathbb{R}^2 \\).
- **Casos de Teste**: Testa o algoritmo com:
  - Pontos coincidentes
  - Pontos colineares
  - Pontos formando triângulos
  - Pontos aleatórios
- **Heurística Aproximada**: Implementação de uma heurística simples para encontrar um círculo mínimo de forma eficiente em grandes conjuntos de dados.
- **Testes com Grandes Conjuntos de Pontos**: Testa o desempenho do algoritmo em conjuntos de milhares de pontos.

## Estrutura do Projeto

O projeto contém as seguintes funções principais:

- **`distancia(p1, p2)`**: Calcula a distância euclidiana entre dois pontos.
- **`ponto_medio(p1, p2)`**: Calcula o ponto médio entre dois pontos.
- **`circulo_heuristico(pontos)`**: Implementa uma solução heurística para encontrar o círculo mínimo em um conjunto de pontos.
- **`find_min_circle(pontos)`**: Implementa o algoritmo de Welzl para encontrar o círculo mínimo de forma exata.

### Casos de Teste:

- **`teste_pontos_simples()`**: Testa o algoritmo em casos com 1, 2 e 3 pontos.
- **`teste_pontos_aleatorios()`**: Gera pontos aleatórios dentro de um círculo conhecido e verifica a precisão do algoritmo.
- **`teste_muitos_pontos()`**: Testa a eficiência do algoritmo com grandes conjuntos de pontos.
- **`teste_casos_degenerados()`**: Avalia o comportamento do algoritmo em casos especiais como pontos coincidentes e colineares.

## Instalação

Clone este repositório:

```bash
git clone https://github.com/karolyneehcs/Smallest-Circle-Problem.git
```
2. Instale as dependências necessárias (se houver).

3. Execute os testes ou scripts de exemplo diretamente no ambiente Python ou em plataformas como Google Colab.

## Exemplos de Uso

### Cálculo do Círculo Mínimo

Você pode utilizar a função `find_min_circle` para calcular o círculo mínimo para um conjunto de pontos:
```python
pontos = [(0, 0), (4, 0), (2, 3)]
centro, raio = find_min_circle(pontos)
print(f"Centro: {centro}, Raio: {raio}")
```

### Testes de Pontos Aleatórios

```python
teste_pontos_aleatorios()
```

## Testes

Este projeto inclui vários testes para verificar a precisão do algoritmo em diferentes cenários:

- Testes simples com 1, 2 e 3 pontos.
- Testes com pontos aleatórios dentro de círculos conhecidos.
- Testes de casos degenerados como pontos coincidentes e colineares.
- Testes com grandes conjuntos de pontos.

Para rodar os testes em um jupyter notebook:

```bash
jupyter execute min_circle.ipynb
```

Caso voce seja iniciante, não tem problema, segue esse tutorial aqui para **Linux**: 

```bash
# crie um arquivo com o nome min_circle.py
touch min_circle.py

# abre o arquivo e cola o código dentro do arquivo
open min_circle.py
CTRL+V

#salva o arquivo
CRTL+S

#executa o código usando
python min_circle.py
```

Caso queira alterar o código, é possível alterar na chamada da função de testes. Depois, só partir pro abraço xD. 

## Contribuição

Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias, correções ou novos recursos. Não garanto aprovação :) 
e-mail: anakarolina1966@gmail.com
