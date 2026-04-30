# Análise de Fator de Segurança em Vasos de Pressão

## Objetivo do projeto

Este projeto tem como objetivo calcular o fator de segurança em um vaso de pressão de parede fina, a partir de parâmetros geométricos, propriedades do material e pressão interna, verificando se o sistema opera dentro de condições seguras.

---

## Conceitos teóricos

Para vasos de pressão cilíndricos de parede fina, as principais tensões atuantes são:

* Tensão circunferencial
* Tensão longitudinal

As expressões usadas são:

* σ_c = (P · r) / t
* σ_l = (P · r) / (2t)

Onde:

* P = pressão interna
* r = raio interno
* t = espessura da parede

O fator de segurança é dado por:

* FS = σ_escoamento / σ_max

---

## Funcionamento

O código realiza as seguintes etapas:

1. Entrada dos dados:

   * Pressão interna (convertida de bar para MPa)
   * Raio interno
   * Espessura
   * Tensão de escoamento do material

2. Cálculo das tensões:

   * Circunferencial
   * Longitudinal

3. Determinação da tensão crítica:

   * Seleção da maior tensão atuante

4. Cálculo do fator de segurança

5. Verificação de segurança:

   * Comparação entre tensões e limite admissível

---

## Saídas do Programa

O programa apresenta ao final do funcionamento as seguintes informações:

* Tensão circunferencial
* Tensão longitudinal
* Fator de segurança
* Diagnóstico do sistema (seguro ou não seguro)

---

## Como Executar?

1. Usar um software com codificaçãoo para Python
2. Execute o arquivo:

```bash
python main.py
```

3. Insira os valores solicitados no terminal

---

## Exemplo de Uso

Entrada:

* Pressão interna: 50 bar
* Raio: 0.5 m
* Espessura: 0.01 m
* Tensão de escoamento: 250 MPa

Saída:

* Tensões calculadas
* Fator de segurança
* Verificação estrutural

---

## Limitações

* Considera vaso de parede fina
* Não considera efeitos térmicos
* Não inclui carregamentos dinâmicos
* Não avalia critérios avançados de falha (ex: von Mises)

---

## Possíveis Extensões futuras

* Implementação do critério de falha de von Mises
* Interface gráfica para entrada de dados
* Integração com simulações numéricas
* Análise paramétrica automática

---

## Contexto Acadêmico

Este projeto foi desenvolvido como aplicação prática de conceitos de resistência dos materiais e mecânica dos sólidos, com foco em análise de tensões e critérios de segurança em engenharia, sendo utilizado para verificação de segurança em relação à projeção de motores para a equipe de foguetemodelismo da universidade, EPTA - Equipe de Propulsão e Tecnologia Aeroespacial.

---

## Tecnologias Utilizadas

* Python
* Lógica de programação aplicada à engenharia

---
