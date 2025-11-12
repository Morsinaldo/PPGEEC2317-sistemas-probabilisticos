# 📗 PPGEEC2317 — Sistemas Probabilísticos — Parte 2  

### Professor: Allan de Medeiros Martins  
### Autor: Morsinaldo de Azevedo Medeiros  

Esta segunda parte da disciplina **PPGEEC2317 — Sistemas Probabilísticos**, oferecida pelo **Programa de Pós-Graduação em Engenharia Elétrica e Computação (PPgEEC/UFRN)**, é dedicada à **visualização geométrica e experimental de conceitos probabilísticos avançados**.  

Os notebooks desenvolvidos nesta etapa tratam da aplicação prática dos conceitos de **mudança de variáveis aleatórias**, **jacobiano**, e da **convergência de distribuições** conforme o **Teorema Central do Limite (TCL)**.

---

## 🧩 Estrutura Geral
```
Parte_2/
├── braco_biarticulado_densidade.ipynb
├── teorema_limite_central.ipynb
└── README.md
```

---

## 🎯 Objetivos da Segunda Parte

- Aplicar os conceitos de **mudança de variáveis aleatórias** e cálculo de **densidades transformadas**.  
- Investigar empiricamente o **Teorema Central do Limite** através de simulação Monte Carlo.  
- Desenvolver **intuição geométrica** sobre distribuições e transformações em múltiplas dimensões.  
- Visualizar o efeito de transformações não lineares no **suporte e na forma da densidade**.  

---

## 🧠 Notebooks Desenvolvidos

### 🔹 1. `braco_biarticulado_densidade.ipynb` — *Mudança de Variáveis Aleatórias e Densidade Espacial*

Este notebook estuda a **cinemática direta** de um **braço robótico biarticulado** e a transformação das variáveis angulares \((\theta_1, \theta_2)\) em coordenadas cartesianas \((x, y)\).  

#### ✳️ Conteúdo abordado:
- Derivação da transformação:  
  \[
  \begin{cases}
  x = L_1\cos(\theta_1) + L_2\cos(\theta_1 + \theta_2) \\
  y = L_1\sin(\theta_1) + L_2\sin(\theta_1 + \theta_2)
  \end{cases}
  \]
- Cálculo do **determinante jacobiano** \( |J| = L_1 L_2 \sin(\theta_2) \).  
- Identificação do **suporte da densidade** no espaço \((x, y)\).  
- Simulação numérica para verificar que **ângulos uniformes** não resultam em **densidade uniforme** no espaço cartesiano.  

#### 💡 Conclusões:
- A densidade tende a se **concentrar nas regiões colineares** do braço (\(|\sin(\theta_2)| \approx 0\)).  
- A formulação demonstra a **não uniformidade induzida** por transformações não lineares.  

> Este estudo conecta conceitos de **probabilidade multivariada**, **geometria diferencial** e **robótica**.

---

### 🔹 2. `teorema_limite_central.ipynb` — *Convergência à Normal e Alinhamento de Variâncias*

O notebook apresenta um experimento computacional para ilustrar o **Teorema Central do Limite (TCL)**, mostrando que a soma de variáveis aleatórias independentes e identicamente distribuídas tende à distribuição Normal conforme o número de termos aumenta.

#### ✳️ Distribuições simuladas:
- **Uniforme** \((-2, 2)\)  
- **Exponencial centrada** \((\lambda = 2)\)  
- **Laplace (0, 2)**  

#### ✳️ Principais etapas do experimento:
1. **Geração e visualização** das distribuições originais.  
2. **Cálculo das variâncias** individuais e dos **fatores de correção** para alinhamento de variâncias:  
   \[
   \text{Fator de escala} = \frac{1}{\sqrt{v}}
   \]
3. **Somas sucessivas (convoluções)** de variáveis i.i.d. para \( n = 5, 10, 20, 30 \).  
4. **Visualização da convergência** das distribuições normalizadas para a **Normal padrão**.  

#### 💡 Conclusões:
- As somas de variáveis independentes **tendem a uma Normal**, independentemente da distribuição original.  
- O **alinhamento de variâncias** torna as comparações entre distribuições mais consistentes.  
- O experimento reforça a **universalidade do TCL** em contextos de simulação e análise estatística.

---

## 🔍 Resultados Gerais

| Conceito | Fenômeno Observado | Abordagem |
|-----------|--------------------|------------|
| Mudança de Variáveis | Densidade não uniforme após transformação angular-cartesiana | Geométrica e Analítica |
| Teorema do Limite Central | Convergência da soma para uma Normal | Simulação Monte Carlo |
| Jacobiano | Relação entre áreas em espaços de probabilidade | Dedução e Verificação Numérica |
| Alinhamento de Variância | Normalização da escala entre distribuições | Cálculo e Visualização |

---

## 🧩 Síntese da Segunda Parte

Esta parte da disciplina evidencia que:
- Transformações não lineares modificam drasticamente a **estrutura da densidade de probabilidade**.  
- A convergência descrita pelo **Teorema Central do Limite** pode ser observada empiricamente mesmo em distribuições assimétricas.  
- A simulação computacional é uma ferramenta poderosa para **intuir propriedades estatísticas complexas**.  

---

📅 *Natal, 2025*  
✍️ *Morsinaldo de Azevedo Medeiros*  
PPgEEC — Universidade Federal do Rio Grande do Norte  
