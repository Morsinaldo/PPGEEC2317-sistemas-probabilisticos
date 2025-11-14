# 🎲 PPGEEC2317 — Sistemas Probabilísticos  
### Professor: Allan de Medeiros Martins  
### Autor: Morsinaldo de Azevedo Medeiros  

Repositório da disciplina **PPGEEC2317 – Sistemas Probabilísticos**, oferecida pelo **Programa de Pós-Graduação em Engenharia Elétrica e Computação (PPgEEC/UFRN)**.  

Este repositório reúne os **notebooks e projetos desenvolvidos ao longo do semestre**, com foco na compreensão e aplicação dos fundamentos da probabilidade e dos processos aleatórios em contextos de engenharia.

---

## 🗂️ Estrutura Geral
```
PPGEEC2317-sistemas-probabilisticos/
├── LICENSE
├── README.md
├── Parte_1/
│   ├── 151_euler_project.ipynb
│   ├── 205_project_euler.ipynb
│   ├── 329_project_euler.ipynb
│   ├── histogram.ipynb
│   ├── monty_hall.ipynb
│   └── README.md           ← explicação detalhada da primeira parte
├── Parte_2/
│   ├── braco_biarticulado_densidade.ipynb
│   ├── teorema_limite_central.ipynb
│   └── README.md           ← explicação detalhada da segunda parte
└── requirements.txt
```

---

## 📘 Parte 1 — Fundamentos e Exercícios Computacionais

A primeira parte da disciplina foi dedicada à **compreensão conceitual e prática dos fenômenos probabilísticos**. Os notebooks exploram problemas clássicos e aplicações de conceitos como valor esperado, probabilidade condicional e processos estocásticos.

### 🔹 `151_euler_project.ipynb`
Problema de **valor esperado** (Project Euler 151).  
Uma gráfica realiza cortes sucessivos de uma folha A1, devolvendo as não usadas a um envelope. O notebook estima o número esperado de vezes em que o envelope contém exatamente uma folha durante a semana.

---

### 🔹 `205_project_euler.ipynb`
Simulação e análise analítica do **Project Euler 205**, que compara distribuições discretas de somas de dados.  
Peter lança nove dados de 4 faces, Colin lança seis de 6 faces, e o notebook calcula a probabilidade de Peter vencer.

---

### 🔹 `329_project_euler.ipynb`
Modelagem de um **processo estocástico com observações probabilísticas**.  
Um sapo se move aleatoriamente entre 500 posições, emitindo sons “P” ou “N” com diferentes probabilidades, conforme a posição seja número primo ou não. O notebook calcula a probabilidade exata de uma sequência específica de sons ocorrer.

---

### 🔹 `histogram.ipynb`
Estudo da aproximação de **densidades empíricas de histogramas** às curvas teóricas.  
Inclui comparação entre as distribuições Uniforme, Exponencial e Normal, aplicando regras de binagem (Freedman–Diaconis, Scott, Sturges).

---

### 🔹 `monty_hall.ipynb`
Simulação clássica do **Problema de Monty Hall**, ilustrando probabilidade condicional e eventos dependentes.  
A convergência das frequências simuladas é comparada com o valor teórico \( P(\text{vitória | troca}) = 2/3 \).

---

## ⚙️ Parte 2 — Aplicações Avançadas e Visualização de Fenômenos Probabilísticos

A segunda parte da disciplina explora aplicações **geométricas e experimentais** dos conceitos de variáveis aleatórias e do **Teorema do Limite Central**, com uso intensivo de simulação, integração numérica e visualização interativa.

### 🔹 `braco_biarticulado_densidade.ipynb`
Estudo probabilístico do **braço robótico biarticulado**, relacionando os ângulos articulares \((\theta_1, \theta_2)\) com as coordenadas cartesianas \((x, y)\) via **cinemática direta**.  
São aplicados conceitos de **mudança de variáveis aleatórias**, **determinante jacobiano** e **suporte de densidade**.  
O notebook mostra que ângulos uniformes não geram densidade uniforme em \((x, y)\), com a massa concentrada próximo às configurações colineares.

---

### 🔹 `teorema_limite_central.ipynb`
Experimento computacional para demonstrar o **Teorema do Limite Central (TCL)**.  
O notebook gera e soma amostras independentes de diferentes distribuições (Uniforme, Exponencial, Laplace etc.), mostrando que a distribuição das somas tende a uma Normal conforme aumenta o número de variáveis somadas.  
Inclui seções dedicadas a:
- Alinhamento de variâncias das distribuições originais.  
- Visualização das convoluções empíricas.  
- Comparação da convergência para a Normal padrão.  

---

## 🚧 Projeto Final (em definição)
O projeto final da disciplina será definido nas próximas semanas.  
A proposta deverá integrar **modelagem probabilística, simulação e visualização**, aplicadas a um problema real de engenharia ou ciência de dados.

---

## 🧠 Objetivos de Aprendizagem

- Compreender o comportamento probabilístico de fenômenos físicos e computacionais.  
- Aplicar transformações de variáveis aleatórias e leis de probabilidade em contextos reais.  
- Implementar experimentos de Monte Carlo e processos estocásticos.  
- Explorar visualmente resultados probabilísticos através de gráficos e simulações.  

---

## ⚙️ Configuração do Ambiente

Criação do ambiente virtual e instalação das dependências:

```bash
conda create -n ppgeec2317 python=3.11.11 -y
conda activate ppgeec2317
pip install -r requirements.txt
```

---

📅 *Natal, 2025*  
✍️ *Morsinaldo de Azevedo Medeiros*  
PPgEEC — Universidade Federal do Rio Grande do Norte  
