# VI ERMAC_AIOE

Repositório oficial do trabalho submetido ao  
**VI Encontro Regional de Matemática Aplicada e Computacional (ERMAC-BA)** — Salvador, BA.

---

## 📝 Resumo

Este projeto apresenta o  
**Algorithm for Integer Optimization in Ellipsoids (AIOE)**,  
um algoritmo voltado para otimização inteira em regiões elipsoidais convexas.

A proposta do método consiste em reduzir iterativamente o problema em ℝⁿ para subproblemas bidimensionais, utilizando fatiamentos orientados pelos menores semieixos do hiperelipsoide.

A busca é conduzida sobre pontos inteiros próximos à fronteira da região viável, permitindo localizar candidatos ótimos de maneira eficiente.

---
## 📐 Metodologia

### Fatiamento: Redução Dimensional (n→2)

O núcleo do algoritmo consiste na redução da dimensão do espaço de busca por meio da fixação de (n-2) variáveis associadas aos semieixos de menor magnitude, restringindo o problema original a uma sequência ordenada de subespaços bidimensionais.

A figura abaixo ilustra geometricamente esse processo de fatiamento, utilizando um elipsoide restrito ao primeiro octante (ℝ₊³) como modelo didático:

![Fatiamento Inteligente](Redução_dimesional.png)

onde

ℝ₊³ := {(X₁,X₂,X₃) ∈ ℝ³ | X_i ≥ 0}.

Como os semieixos obedecem à ordenação

a₃ < a₂ < a₁

o algoritmo realiza o fatiamento ao longo do menor eixo (X₃), gerando seções elípticas planas para cada cota inteira no intervalo

[0 , ⌊a₃⌋].

Cada uma dessas seções bidimensionais define um subproblema plano, no qual uma busca exata local determina um candidato ótimo.

Ao final do processo, os candidatos obtidos em cada fatia são comparados, permitindo ao algoritmo selecionar a melhor solução inteira associada ao problema original.

---

## ⚙️ Diferenciais Técnicos

- **Estratégia:** priorização dos menores semieixos para reduzir o número de iterações;
- **Busca:** deslocamentos discretos orientados pela fronteira da região viável;
- **Complexidade:**  
  T(n,a)=O(n⌊a₂⌋ⁿ⁻¹);
- **Comportamento:** pseudopolinomial para dimensões fixas.

---

## 📺 Demonstrações Visuais

Apresentamos abaixo duas animações complementares do algoritmo: uma abordagem técnica e outra introdutória.

### 1. Dinâmica do Algoritmo (Perspectiva Técnica)

Após o processo de fatiamento (n→2), o algoritmo executa deslocamentos discretos na fronteira da região viável utilizando as funções (fₐ) e (gₐ).

▶️ [**Assistir animação técnica no YouTube**](https://youtu.be/K7HpVdJK1hY?si=EuyrtPGT7hsRbw5P)

---

### 2. Interpretação Geométrica da Solução (Perspectiva Didática)

Esta animação foi desenvolvida para introduzir conceitos básicos de Otimização Discreta.  
Ela ilustra geometricamente como a função objetivo percorre a região factível até atingir o ponto ótimo inteiro.

▶️ [**Assistir animação didática no YouTube**](https://youtu.be/bKN_NNsvDd0?si=3sigzNJXPA29Twyz)

---

## 👤 Autores

- **Marcos Vinícius Barreto dos Santos** — UFRB  
- **Lucas Ivonovith Peixoto Vilas Boas** — UFRB  
- **Dr. Eleazar Gerardo Madriz Lozada** — Orientador (UFRB)