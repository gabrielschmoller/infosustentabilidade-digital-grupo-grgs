# 🗂️ Modelo de Dados — InfoSustentabilidade

O diagrama abaixo representa as entidades utilizadas no sistema de gerenciamento de informações sobre sustentabilidade e descarte de resíduos eletrônicos.

## 🧩 Descrição das Entidades

### `pontos_coleta`
Armazena informações dos locais de coleta de resíduos eletrônicos.

| Campo | Descrição |
|---|---|
| id | Identificador único |
| nome | Nome do ponto de coleta |
| endereco | Endereço |
| bairro | Bairro |
| cidade | Cidade |
| contato | Telefone ou e-mail |
| link_maps | Link do Google Maps |
| observação | Informações adicionais |

---

### `materiais_aceitos`
Define quais materiais cada ponto aceita.

| Campo | Descrição |
|---|---|
| id_material | Identificador |
| id_ponto | Referência ao ponto de coleta |
| tipo_material | Tipo do material |
| aceita | Booleano indicando aceitação |
| observação | Observações |

---

### `procedimentos_descarte`
Informações sobre o processo de descarte.

| Campo | Descrição |
|---|---|
| id | Identificador |
| id_ponto | Referência ao ponto |
| horário | Horário de funcionamento |
| agendamento | Necessita agendamento |
| custo | Existe custo |
| modalidade | Tipo de coleta |
| descrição | Detalhes do descarte |

---

### `evidencias`
Registra evidências e verificações dos pontos.

| Campo | Descrição |
|---|---|
| id | Identificador |
| id_ponto | Referência ao ponto |
| tipo | Tipo de evidência |
| descrição | Descrição |
| arquivo/link | Arquivo ou URL |
| data_verificação | Data da verificação |

---

### `analises_criticas`
Armazena análises e avaliações sobre o sistema.

| Campo | Descrição |
|---|---|
| id | Identificador |
| cidade | Cidade analisada |
| facilidade | Facilidade de descarte |
| dificuldades | Problemas encontrados |
| divulgação | Nível de divulgação |
| melhorias | Sugestões de melhorias |

---

## 🌱 Objetivo do Modelo

Este modelo foi desenvolvido para auxiliar no mapeamento e análise de pontos de descarte eletrônico, promovendo:

- Sustentabilidade;
- Consumo consciente;
- Gestão de resíduos eletrônicos;
- Educação ambiental;
- Organização de dados para pesquisas acadêmicas.
