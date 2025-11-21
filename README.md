# Guia de Aula – DR e DPS (Dispositivo Diferencial-Residual e Dispositivo de Proteção contra Surtos)

## 1. Introdução Geral

As instalações elétricas modernas precisam garantir segurança para as pessoas e proteção para os equipamentos.  
Para isso, a NBR 5410 estabelece o uso de dispositivos indispensáveis:

- **DR (Dispositivo Diferencial-Residual)** – protege pessoas contra choque elétrico.  
- **DPS (Dispositivo de Proteção contra Surtos)** – protege equipamentos contra sobretensões transitórias.

Esses dispositivos atuam em fenômenos diferentes e não substituem disjuntores.  
Eles complementam a proteção da instalação e são obrigatórios em diversos contextos.

---

## 2. Princípio de Funcionamento dos Dispositivos

### 2.1. DR – Princípio de Funcionamento

O DR atua com base no equilíbrio das correntes:  
**a corrente que entra no circuito deve sair pelo mesmo caminho**.

Ele utiliza um **transformador toroidal** que monitora a corrente da fase e do neutro.

#### Como funciona:

1. Em condições normais, as correntes somam zero.  
2. Em caso de fuga (choque, isolamento danificado), parte da corrente escapa para o terra.  
3. A soma deixa de ser zero, gerando diferença (corrente residual).  
4. Se essa diferença for maior que o limite (ex.: 30 mA), o DR **desarma instantaneamente**.

#### Em resumo:

- Corrente equilibrada → funcionamento normal  
- Corrente desequilibrada → **DR desarma e protege o usuário**

---

### 2.2. DPS – Princípio de Funcionamento

O DPS **não desliga** o circuito.  
Ele protege desviando **surtos de tensão** para o terra antes que danifiquem os equipamentos.

Ele opera com **varistores (MOV)** ou **centelhadores**.

#### Como funciona:

1. Em condições normais: DPS tem alta impedância.  
2. Quando ocorre um surto: a tensão sobe subitamente.  
3. O DPS diminui sua resistência e desvia o surto para o terra.  
4. Após o evento, retorna à condição normal (MOV) ou precisa ser substituído (centelhador).

#### Em resumo:

- Tensão normal → DPS não interfere  
- Surto → **DPS atua desviando a sobretensão**

---

## 3. Tipos de DR (Detalhado)

Os DR são classificados conforme o tipo de corrente diferencial que conseguem detectar:

### **DR Tipo AC**
- Detecta apenas **correntes residuais senoidais puras (AC)**.
- Usado em cargas simples.
- **Menos recomendado** para instalações residenciais modernas.

### **DR Tipo A**
- Detecta correntes residuais:
  - senoidais (AC)
  - pulsantes (meia onda)
- Compatível com eletrodomésticos modernos com eletrônica.
- **É o tipo recomendado para residências.**

### **DR Tipo F**
- Detecta correntes:
  - senoidais  
  - pulsantes  
  - de frequência mista  
- Suporta cargas com motores controlados por inversores, soft-starters, etc.

### **DR Tipo B**
- Detecta:
  - AC  
  - DC  
  - correntes residuais de alta frequência  
  - harmônicas  
- Usado em:
  - sistemas fotovoltaicos  
  - carregadores de veículos elétricos  
  - inversores industriais  

---

## 4. Tipos de DPS (Detalhado)

Os DPS são classificados segundo sua capacidade de suportar e desviar surtos:

### **DPS Tipo 1**
- Projetado para suportar **correntes impulsivas** muito altas.  
- Necessário quando há **SPDA (para-raios)** na edificação.  
- Protege contra descargas atmosféricas **diretas** na instalação.

### **DPS Tipo 2**
- Mais utilizado em residências.  
- Deve ser instalado no **quadro principal**.  
- Protege contra:
  - surtos induzidos por raios próximos  
  - chaveamentos da concessionária  
  - manobras de grandes cargas

### **DPS Tipo 3**
- Proteção fina e complementar.  
- Instalado próximo a equipamentos sensíveis (TV, computadores, roteadores).  
- Geralmente aparece em:
  - filtros de linha
  - módulos protetores para tomadas

---

## 5. Comparação – DR x DPS

| Função | DR | DPS |
|--------|-----|------|
| Proteção de pessoas | ✔️ | ❌ |
| Proteção de equipamentos | ❓ | ✔️ |
| Atua em corrente de fuga | ✔️ | ❌ |
| Atua em surtos | ❌ | ✔️ |
| Desarma | ✔️ | ❌ |

---

## 6. Exemplo Prático – Residência

1. Disjuntor geral  
2. DPS tipo 2  
3. DR 30 mA  
4. Disjuntores dos circuitos  

---

## 7. Dicas de Segurança

- Nunca usar neutro como terra  
- Usar tomadas com pino terra  
- Evitar benjamins/Ts  
- Quadro sempre limpo  
