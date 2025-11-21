<td style="width: 10%;"><img src="https://github.com/Epaminondaslage/Lab-IoT-ELE-CEFET/blob/master/img/Logo_CEFET-MG.png" width="10%" /></td>

## **CENTRO FEDERAL DE EDUCAÇÃO TECNOLÓGICA DE MINAS GERAIS**  
## **Departamento de Engenharia Elétrica - CEFET-MG**  
## **Coordenação do Curso de Eletrotécnica**  

## Disciplina: **PLIP - Prática de Laboratório de Instalações Prediais**
## Guia de Aula – DR e DPS (Dispositivo Diferencial-Residual e Dispositivo de Proteção contra Surtos)

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

O **DPS (Dispositivo de Proteção contra Surtos)** não desliga o circuito.  
Sua função é **desviar e limitar surtos de tensão**, impedindo que eles atinjam e danifiquem equipamentos eletrônicos.

Esses surtos podem ser causados por:

- descargas atmosféricas (raios);
- chaveamentos na rede pública;
- manobras da concessionária;
- motores e cargas indutivas ligando/desligando;
- variações bruscas dentro da própria instalação.

Mesmo surtos muito rápidos (microssegundos) podem danificar equipamentos sensíveis como TVs, roteadores, computadores e sistemas de automação.

---

###  Como o DPS trabalha internamente

O DPS funciona como um “caminho alternativo” para a sobretensão.  
Em vez de permitir que o pico atinja os equipamentos, ele **desvia o excesso de energia para o terra**.

Para isso, utiliza dois componentes principais:

---

###  2.3.1. Varistores (MOV – Metal Oxide Varistor)

O varistor é o componente mais comum em DPS residenciais (Tipo 2 e Tipo 3).

### Funcionamento:

- **Condição normal:** resistência muito alta (quase aberto).
- **Durante o surto:** a tensão sobe rapidamente.
- O varistor **reduz sua resistência**, conduzindo o excesso para o terra.
- Após o surto, volta ao estado normal, mas sofre desgaste e pode precisar ser substituído.

---

### 2.3.2. Centelhadores (Spark Gap / GDT – Gas Discharge Tube)

Comum em DPS Tipo 1 e aplicações industriais.

### Funcionamento:

- **Condição normal:** circuito aberto, sem condução.
- **Durante surtos fortes:** a alta tensão ioniza o gás interno.
- O centelhador **fecha o circuito**, desviando grandes correntes para o terra.
- Após o surto, o arco elétrico se extingue e o dispositivo volta ao estado normal.

---

### 2.3.2. O que o DPS faz e não faz

#### O DPS faz:
- desvia surtos para o terra;
- limita picos de tensão em níveis seguros;
- protege equipamentos eletrônicos sensíveis;
- atua em microssegundos.

#### O DPS não faz:
- não desarma o circuito;
- não protege contra sobrecarga;
- não protege contra curto-circuito;
- não substitui o DR ou o disjuntor.

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

|## 5. Comparação Técnica – DR x DPS

| Critério Técnico | DR (Dispositivo Diferencial-Residual) | DPS (Dispositivo de Proteção contra Surtos) |
|------------------|----------------------------------------|----------------------------------------------|
| **Finalidade principal** | Proteção contra choques elétricos por corrente de fuga | Proteção contra sobretensões transitórias (surtos) |
| **Proteção de pessoas** | ✔️ Sim — evita fibrilação cardíaca e choques indiretos | ❌ Não — não detecta corrente através do corpo |
| **Proteção de equipamentos** | ⚠️ Parcial — apenas em casos de fuga que poderia causar incêndio | ✔️ Sim — protege contra surtos de alta tensão |
| **Fenômeno elétrico monitorado** | Corrente diferencial entre fase e neutro | Elevação instantânea de tensão acima do valor nominal |
| **Elemento de atuação** | Transformador toroidal + mecanismo de disparo | Varistor (MOV), centelhador (GDT) ou Spark Gap |
| **Tipo de grandeza que dispara a atuação** | Corrente residual (mA) | Sobretensão (kV) |
| **Tempo de resposta** | Milissegundos | Microssegundos |
| **Modo de proteção** | Abre o circuito (desligamento) | Desvia energia para o terra (sem desligar) |
| **Desarma o circuito?** | ✔️ Sim | ❌ Não — apenas limita/ desvia tensão |
| **Obrigatoriedade NBR 5410** | Obrigatório em áreas molhadas e circuitos específicos | Recomendado/obrigatório conforme análise de risco |
| **Instalação** | Em série com o circuito | Em paralelo com o circuito (entre fase-neutro/terra) |

---
## 6. Diferença entre DR e DDR

### DR – Dispositivo Diferencial-Residual
Também conhecido como **IDR (Interruptor Diferencial Residual)**.

**Função principal:** proteger pessoas contra choques elétricos.  
O DR atua quando detecta **corrente de fuga**, ou seja, diferença entre a corrente que sai pela fase e retorna pelo neutro.

#### Características:
- ✔ Protege contra choque elétrico  
- ❌ Não protege contra sobrecarga  
- ❌ Não protege contra curto-circuito  
- Contém **somente o módulo diferencial residual**

O DR **desarma apenas por fuga de corrente**.

---

### DDR – Disjuntor Diferencial Residual
É a combinação de dois dispositivos em um só:

- **DR** (proteção diferencial)  
- **Disjuntor termomagnético** (proteção contra sobrecorrente)

#### Características:
- ✔ Protege contra choque elétrico  
- ✔ Protege contra sobrecarga  
- ✔ Protege contra curto-circuito  
- Substitui o disjuntor do circuito  
- Equivale ao **RCBO** nas normas internacionais

O DDR possui **todas as proteções em um único dispositivo**.

---

### Resumo Comparativo

| Característica | DR | DDR |
|----------------|-----|------|
| Proteção contra choque | ✔ | ✔ |
| Proteção contra sobrecarga | ✖ | ✔ |
| Proteção contra curto-circuito | ✖ | ✔ |
| Substitui o disjuntor termomagnético? | ✖ Não | ✔ Sim |
| Conteúdo interno | Apenas diferencial residual | Diferencial + termomagnético |
| Nome técnico (IEC) | IDR | RCBO |

---

### Forma simples de lembrar

- **DR = protege pessoas**  
- **DDR = protege pessoas + protege cabos/equipamentos**

---

## 7. Dicas de Segurança

- Nunca usar neutro como terra  
- Usar tomadas com pino terra  
- Evitar benjamins/Ts  
- Quadro sempre limpo  

---

## 8. Atividade Prática

