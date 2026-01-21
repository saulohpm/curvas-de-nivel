# Curvas de Nível e Campo de Gradientes de uma Função Bidimensional

Este repositório apresenta um exemplo de análise e visualização de uma função escalar de duas variáveis utilizando **Python**, com apoio das bibliotecas **SymPy**, **NumPy** e **Matplotlib**.

O foco do projeto é demonstrar:
- o uso de **cálculo simbólico** para obtenção automática de derivadas parciais;
- a conversão de expressões simbólicas em funções numéricas;
- a visualização conjunta de **curvas de nível** e do **campo de gradientes** no plano.

---

## Função analisada

A função escalar considerada é definida simbolicamente por (pode ser editada):

$$
f(x,y) = \sin(xy) + e^x \cos(y) - x^2 y
$$

A partir dessa função, são calculadas as derivadas parciais:

As derivadas parciais da função são:
$$
\frac{\partial f}{\partial x}
\quad \text{e} \quad
\frac{\partial f}{\partial y}
$$

utilizando diferenciação automática com o **SymPy**.

---

## Metodologia

O código segue as seguintes etapas:

1. Definição simbólica da função e das variáveis;
2. Cálculo das derivadas parciais em relação a $`x`$ e $`y`$;
3. Conversão das expressões simbólicas em funções numéricas com `lambdify`;
4. Construção de:
   - uma malha fina para o traçado das curvas de nível;
   - uma malha mais espaçada para o campo de gradientes;
5. Normalização dos vetores gradiente;
6. Geração do gráfico com:
   - curvas de nível;
   - mapa de cores da função;
   - vetores do campo de gradientes.

---

## Visualização

O gráfico final combina:
- **curvas de nível** da função escalar;
- **preenchimento em cores** para representar a variação dos valores de  $f(x,y)$;
- **vetores normalizados** do gradiente, indicando a direção de maior crescimento da função.

---

## Tecnologias utilizadas

- **Python 3**
- **SymPy** – cálculo simbólico e diferenciação automática
- **NumPy** – operações numéricas e geração de malhas
- **Matplotlib** – visualização gráfica

---

## Aplicações

Este exemplo é útil para fins didáticos e acadêmicos, especialmente em:
- Cálculo multivariável;
- Cálculo vetorial;
- Análise de gradientes;
- Visualização de campos escalares.

---

## Requisitos e Execução

As bibliotecas necessárias para executar o código são:

- NumPy
- SymPy
- Matplotlib

A instalação pode ser feita com:

```bash
pip install -r requirements.txt