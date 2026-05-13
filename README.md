# VI ERMAC_AIOE

Repositório acadêmico do algoritmo AIOE para submissão ao VI ERMAC 2026 (Salvador-BA). Contém PDF, animações e códigos.

Repositório oficial para o trabalho submetido ao **VI Encontro Regional de Matemática Aplicada e Computacional (ERMAC-BA)**, realizado em Salvador.

## 📝 Resumo
Este projeto apresenta o **Algorithm for Integer Optimization in Ellipsoids (AIOE)**. O foco da pesquisa é a otimização global em conjuntos convexos discretos utilizando fatiamento inteligente orientado pelos semieixos de menor magnitude.

### Diferenciais Técnicos:
* **Estratégia de Fatiamento**: Redução de dimensão $n \to 2$ priorizando eixos menores.
* **Complexidade**: $O(n \lfloor a_2 \rfloor^{n-1})$.
* **Visualização**: Implementação de funções de fronteira fₐ e gₐ para varredura de vizinhança.

## 🎥 Demonstração Visual
Abaixo, a animação que ilustra a estratégia de busca começando pelo eixo menor ($x_2$), minimizando o número de iterações:

![Animação AIOE](animacoes/animacao_aioe.gif)

## 👤 Autores
* **Marcos Vinícius Barreto dos Santos** (UFRB)
* **Lucas Ivonovith Peixoto Vilas Boas** (UFRB)
* **Dr. Eleazar Gerardo Madriz Lozada** (Orientador - UFRB)
