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

O DR funciona com base no **princípio do equilíbrio das correntes**, isto é, toda a corrente que entra no circuito pela fase deve retornar pelo neutro. Para monitorar isso, o dispositivo utiliza um **transformador toroidal**, por onde passam os condutores de fase e neutro. Esse núcleo avalia continuamente a soma vetorial das correntes.

#### Como o DR atua:

- **Condição normal:**  
  A corrente que sai pela fase retorna integralmente pelo neutro. A soma dessas correntes é igual a zero, o que mantém o DR estabilizado e ligado.

- **Fuga de corrente:**  
  Quando ocorre choque elétrico, falha de isolação ou contato com partes energizadas, parte da corrente deixa de retornar pelo neutro e escapa pelo terra ou através do corpo humano. Isso provoca um desequilíbrio detectável.

- **Detecção:**  
  O desequilíbrio gera um campo magnético residual no toróide, induzindo um sinal no seu enrolamento secundário.

- **Atuação:**  
  Se essa corrente diferencial-residual ultrapassar o limite de sensibilidade (como **30 mA**, usado para proteção humana), o sistema de disparo interna­mente aciona o mecanismo de abertura, desligando o circuito **em poucos milissegundos**, interrompendo o risco de choque ou incêndio.

#### Em resumo:

- Corrente equilibrada → funcionamento normal  
- Corrente desequilibrada → **DR desarma e protege o usuário**

### 2.2 Disjuntores Diferenciais Residuais (DDR / DR)

Os **disjuntores diferenciais residuais (DDR)** — também conhecidos como **DR** ou **IDR (Interruptor Diferencial Residual)** — são dispositivos essenciais em instalações elétricas, pois **protegem pessoas contra choques elétricos** e **protegem os circuitos contra sobrecargas e curto-circuitos** quando integrados ao disjuntor termomagnético.

Eles combinam duas funções em um único equipamento:

- **Função diferencial (DR):** detecta fugas de corrente e protege contra choques.
- **Função termomagnética:** protege o circuito contra sobrecarga e curto-circuito.

---

###  O que é fuga de corrente?

Fuga de corrente é quando parte da corrente elétrica escapa do circuito e passa por um caminho não previsto, como:

- o corpo de uma pessoa;
- o sistema de aterramento;
- fios com isolação danificada;
- um equipamento com falha interna.

Correntes tão pequenas quanto **30 mA** já podem ser fatais.  
O DDR identifica essa fuga e **desliga o circuito imediatamente**, evitando acidentes graves.

---

###  Funcionamento do Disjuntor Diferencial Residual

O DDR contém um **transformador toroidal** por onde passam os condutores de fase e neutro. Ele monitora se:

- a corrente que **entra** pela fase retorna **integralmente** pelo neutro;
- ou se parte dela está escapando (fuga).

####  Operação normal
Corrente da fase = corrente do neutro.  
A soma das correntes é zero, e o DDR permanece ligado.

####  Situação de fuga
Parte da corrente “se perde” pelo terra ou pelo corpo humano → ocorre desequilíbrio.  
O DR detecta a corrente diferencial residual e **desarma em milissegundos**.

---

###  Vantagens do DDR

- Proteção contra choques diretos e indiretos  
- Prevenção de incêndios provocados por fuga de corrente  
- Detecção de falhas de isolamento  
- Em modelos integrados, substitui DR + disjuntor  
- Obrigatório em áreas de risco conforme NBR 5410  

---

###  Tipos de DR

#### Por sensibilidade
- **30 mA:** proteção de pessoas  
- **100 mA:** proteção complementar  
- **300 mA:** proteção contra incêndios (uso industrial)

#### Por forma da corrente de fuga detectada
| Tipo | Características | Aplicação |
|------|----------------|-----------|
| **AC** | detecta correntes residuais senoidais | cargas simples |
| **A** | detecta AC + pulsantes | eletrodomésticos modernos |
| **F** | detecta correntes mistas | motores controlados |
| **B** | detecta AC + DC + harmônicas | fotovoltaico, VFD, veículos elétricos |

#### Por número de polos
- **Bipolar:** fase + neutro  
- **Tetrapolar:** trifásico + neutro  

---


###  Regras importantes de instalação

- O neutro **não pode ser aterrado após o DR**  
- Não deve haver **neutro compartilhado** entre circuitos protegidos  
- O DR deve estar antes das derivações que alimentam os circuitos  
- O sistema deve possuir aterramento adequado  



---

### 2.3. DPS – Princípio de Funcionamento

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

## 3. Tipos de DR 

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

## 4. Tipos de DPS 

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

---

## 8. Atividade Prática

