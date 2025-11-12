# 📘 PPGEEC2317 — Sistemas Probabilísticos - Parte 1

### Professor: Allan de Medeiros Martins  
### Autor: Morsinaldo de Azevedo Medeiros  

Repositório referente à **primeira parte da disciplina PPGEEC2317 — Sistemas Probabilísticos**, oferecida pelo **Programa de Pós-Graduação em Engenharia Elétrica e Computação (PPgEEC/UFRN)**.  

Esta etapa concentrou-se na **fundamentação probabilística** e na **experimentação computacional**, explorando desde problemas clássicos de valor esperado até simulações de processos estocásticos e transformações de variáveis aleatórias.

---

## 🧩 Estrutura Geral
```
Parte_1/
├── 151_euler_project.ipynb
├── 205_project_euler.ipynb
├── 329_project_euler.ipynb
├── histogram.ipynb
├── monty_hall.ipynb
└── README.md
```

---

## 🎯 Objetivos da Primeira Parte

- Aplicar os **conceitos fundamentais de probabilidade** a problemas computacionais.  
- Explorar **processos aleatórios e distribuições de probabilidade** por meio de simulação e análise numérica.  
- Visualizar o comportamento de variáveis aleatórias contínuas e discretas.  
- Desenvolver raciocínio probabilístico e intuição sobre convergência e eventos condicionais.  

---

## 📗 Notebooks Desenvolvidos

### 🔹 1. `151_euler_project.ipynb` — *Valor Esperado e Processos de Corte*
Baseado no *Project Euler Problem 151*, este notebook investiga um **problema de valor esperado**.  
Uma gráfica inicia a semana com uma folha A1 e realiza cortes sucessivos para obter folhas menores, armazenando as sobras em um envelope.  
A cada novo trabalho, uma folha é retirada aleatoriamente; se necessário, novos cortes são feitos.  
O objetivo é determinar o **número esperado de vezes** em que o envelope contém exatamente uma folha — excetuando o primeiro e o último trabalho.  

> Conceitos explorados: valor esperado, distribuição condicional e simulação de processos discretos.

---

### 🔹 2. `205_project_euler.ipynb` — *Comparação de Distribuições Discretas*
Implementação do *Project Euler Problem 205*, que compara distribuições obtidas por **lançamento de dados**.  
Peter lança **nove dados de quatro faces**, enquanto Colin lança **seis dados de seis faces**.  
As somas são comparadas para determinar a **probabilidade de vitória de Peter**, isto é, \( P(S_P > S_C) \).  

> Inclui abordagens analítica e por simulação Monte Carlo, com validação cruzada dos resultados.

---

### 🔹 3. `329_project_euler.ipynb` — *Processo Estocástico e Probabilidade de Sequência*
Estudo do *Project Euler Problem 329*, formulado como um **processo estocástico com observações probabilísticas**.  
Um sapo se move aleatoriamente sobre **500 posições numeradas**, emitindo sons “P” ou “N” de acordo com se a posição atual é **primo ou não**.  
O notebook calcula, de forma analítica e simbólica, a **probabilidade de ocorrência** da sequência “PPPPNNPPPNPPNPN”, expressa como uma fração reduzida \( p/q \).

> Conceitos aplicados: cadeias de Markov, probabilidade condicional e decomposição de estados.

---

### 🔹 4. `histogram.ipynb` — *Densidades Empíricas e Transformações de Variáveis*
O objetivo deste notebook é aproximar **densidades empíricas** de histogramas às **curvas teóricas** das principais distribuições contínuas.  
O estudo está dividido em duas partes:

1. **Aproximação e análise empírica**  
   - Distribuições: **Uniforme**, **Exponencial** e **Normal (Gaussiana)**.  
   - Critérios de binagem aplicados: **Freedman–Diaconis**, **Scott** e **Sturges**.  
   - Comparação entre o histograma normalizado e a densidade teórica de cada caso.

2. **Exercícios resolvidos do livro *Papoulis & Pillai* (Capítulo 5 — Funções de Variável Aleatória)**  
   - **Ex. 5-6:** Transformação \( Y = -\ln X \), com \( X \sim U(0,1) \Rightarrow Y \sim \mathrm{Exp}(1) \).  
   - **Ex. 5-17:** Transformação \( Y = \sqrt{X} \), com \( X \sim \chi^2(n) \Rightarrow Y \sim \mathrm{Chi}(n) \).  
   - **Ex. 5-18:** Transformação \( Y = -2\ln X \), com \( X \sim U(0,1) \Rightarrow Y \sim \chi^2(2) \).  

> Enfatiza o uso de histogramas como ferramenta de estimativa visual de densidade e validação de transformações teóricas.

---

### 🔹 5. `monty_hall.ipynb` — *Probabilidade Condicional e Decisão Ótima*
Simulação clássica do **Problema de Monty Hall**, que ilustra a importância da **probabilidade condicional**.  
Um participante escolhe uma das três portas, uma delas contendo o prêmio. Após o apresentador revelar uma porta vazia, o jogador decide **manter ou trocar** sua escolha inicial.  
O experimento é repetido milhares de vezes, e as probabilidades empíricas convergem para o valor teórico:

\[
P(\text{vitória | troca}) = \frac{2}{3}, \quad P(\text{vitória | mantém}) = \frac{1}{3}.
\]

> Mostra de forma intuitiva como a atualização de crenças altera as probabilidades condicionais.

---

## 🧠 Conclusão da Primeira Parte

Os notebooks desta etapa permitiram consolidar:
- A **intuição sobre o comportamento aleatório** de sistemas e processos.  
- A importância da **simulação computacional** para validar hipóteses probabilísticas.  
- A integração entre **modelagem matemática e experimentação numérica**.  

---

📅 *Natal, 2025*  
✍️ *Morsinaldo de Azevedo Medeiros*  
PPgEEC — Universidade Federal do Rio Grande do Norte  
