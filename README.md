# VI ERMAC_AIOE

Repositório oficial do trabalho submetido ao  
**VI Encontro Regional de Matemática Aplicada e Computacional (ERMAC-BA)** — Salvador, BA.

---

## 📝 Resumo

Este projeto apresenta o  
**Algorithm for Integer Optimization in Ellipsoids (AIOE)**,  
um algoritmo voltado para otimização inteira em regiões elipsoidais convexas.

A proposta do método consiste em reduzir iterativamente o problema em ℝⁿ para subproblemas bidimensionais, utilizando fatiamentos orientados pelos menores semieixos da elipse/hiperelipsoide.

A busca é realizada sobre os pontos inteiros mais próximos da fronteira da região viável, permitindo localizar candidatos ótimos de maneira eficiente.

---

## 📐 Metodologia

### Fatiamento: Redução Dimensional (n→2)

O algoritmo fixa (n-2) variáveis, transformando o problema original em uma sequência de problemas bidimensionais.

A figura abaixo ilustra geometricamente o processo de fatiamento em \(ℝ³):

![Fatiamento Inteligente](Redução_dimesional.png)

Cada seção bidimensional gera um candidato ótimo local.  
Ao final do processo, o algoritmo compara os candidatos encontrados e determina a melhor solução inteira do problema original.

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