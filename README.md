# VI ERMAC_AIOE

Repositório oficial para o trabalho submetido ao **VI Encontro Regional de Matemática Aplicada e Computacional (ERMAC-BA)**, Salvador-BA.

## 📝 Resumo
Este projeto apresenta o **Algorithm for Integer Optimization in Ellipsoids (AIOE)**. A pesquisa foca na otimização global em conjuntos convexos discretos utilizando fatiamento inteligente orientado pelos semieixos de menor magnitude.

---

## 📺 Demonstrações Visuais

Abaixo, apresentamos o funcionamento do algoritmo sob duas perspectivas: uma didática, para facilitar a introdução ao tema, e outra técnica, detalhando a mecânica interna de busca.

### 1. Entendendo o Objetivo (Perspectiva Didática)
Esta animação foi desenvolvida para facilitar a compreensão de quem está iniciando na área de Otimização Discreta. Ela ilustra como a reta da Função Objetivo desliza pela região factível até encontrar o ponto ótimo (4,1).
* ▶️ [**Assista à Explicação do Objetivo no YouTube**](https://youtu.be/bKN_NNsvDd0?si=3sigzNJXPA29Twyz)

### 2. Dinâmica do Algoritmo (Perspectiva Técnica)
Após o processo de **fatiamento** (n → 2), o algoritmo executa a busca na fronteira através das funções fₐ e gₐ.
* ▶️ [**Assista à Animação do Deslocamento no YouTube**](https://youtu.be/K7HpVdJK1hY?si=EuyrtPGT7hsRbw5P)

---

## 📐 Metodologia

### Fatiamento: Redução de Dimensão (n → 2)
O processo inicial consiste em isolar subespaços bidimensionais para viabilizar a busca exata. Abaixo, a projeção no $\mathbb{R}^3$:

![Fatiamento em R3](Fatiamento.png)

### Diferenciais Técnicos:
* **Estratégia**: Priorização de eixos menores para minimizar iterações.
* **Complexidade**: T(n,a) = O(n⌊a₂⌋ⁿ⁻¹).
* **Comportamento**: Caracterizado como **pseudopolinomial** para dimensões fixas.

## 👤 Autores
* **Marcos Vinícius Barreto dos Santos** (UFRB)
* **Lucas Ivonovith Peixoto Vilas Boas** (UFRB)
* **Dr. Eleazar Gerardo Madriz Lozada** (Orientador - UFRB)

---