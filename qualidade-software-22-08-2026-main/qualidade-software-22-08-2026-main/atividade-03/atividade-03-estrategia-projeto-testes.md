# Atividade 3: Estratégia e Projeto de Testes do LocalEats

> Substituam os campos entre colchetes pelas respostas da equipe e removam as instruções antes da entrega.

## 1. Identificação

**Turma:** ADS5M26-2C
**Equipe:** Alessandro e Ramon.  
**Data:** 07/09/2026

### Integrantes

|           Nome           |     Usuário no GitHub    |
|--------------------------|--------------------------|
| Alessandro Reis da Silva | @AlessandroReisDaSilva |
|      Ramon nogueira      |         @Ramonnogueira83         |

**Elemento de Competência:** Planejar e projetar testes selecionando técnicas adequadas.

**Aplicação:** <https://local-eats-unisenac.vercel.app/>

---

## 2. Tarefa 1: Planejamento dos testes

### 2.1 Objetivo dos testes

[Verificar se o LocalEats permite que os usuários encontrem restaurantes de acordo com a culinária desejada e gerenciem corretamente seus restaurantes favoritos, garantindo que as funcionalidades de busca por culinária e de favoritar e desfavoritar restaurantes apresentem resultados e comportamentos esperados nas diferentes situações de uso.]

### 2.2 Escopo

#### Funcionalidades incluídas

| Integrante | Funcionalidade incluída | O que será verificado |
|---|---|---|
| [Ramon] | [filtrar restaurantes por especialidade] | [Todas as opções que o Usuário pode filtrar para encontrar o restaurante desejado ] |
| [Alessandro] | [favoritar e desfavoritar restaurantes] | [Todas as formas de favoritar e desfavoritar nas páginas do Local Eats] |

> Acrescentem ou removam linhas conforme o número de integrantes.

#### Funcionalidade não incluída

| Funcionalidade não incluída | Justificativa |
|---|---|
| [Consultar pedidos] | [Já está funcionando corretamente] |

### 2.3 Abordagem

| Item | Decisão da equipe | Justificativa |
|---|---|---|
| Níveis de teste | [Teste de sistema] | [As funcionalidades serão analisadas no funcionamento completo da aplicação, considerando a interação do usuário com o LocalEats.] |
| Tipos de teste | [Teste funcional] | [O objetivo é verificar se a busca por culinária e as ações de favoritar e desfavoritar apresentam os comportamentos esperados de acordo com suas funcionalidades.] |
| Perspectiva caixa-preta ou caixa-branca | [Caixa-preta] | [Os testes serão elaborados a partir das entradas fornecidas pelo usuário e dos resultados apresentados pelo sistema, sem analisar o código interno da aplicação.] |
| Técnicas de teste | [Particionamento de equivalência e transição de estados] | [O particionamento de equivalência pode ser utilizado para analisar diferentes entradas na busca por culinária, enquanto a transição de estados é adequada para verificar as mudanças entre restaurante não favoritado e favoritado.] |

### 2.4 Ambiente e responsabilidades

| Item | Definição |
|---|---|
| Ambiente necessário | [Aplicação LocalEats disponível no navegador, computador ou dispositivo com acesso à internet, conta de usuário cadastrada e restaurantes disponíveis para realizar as buscas e testes de favoritos.] |
| Responsáveis pelo planejamento | [Ramon e Alessandro.] |
| Responsáveis pela especificação dos casos | [Ramon será responsável pela especificação dos casos relacionados à busca de restaurantes por culinária, e Alessandro será responsável pelos casos relacionados a favoritar e desfavoritar restaurantes.] |
| Responsáveis pela futura execução | [Ramon e Alessandro, cada um responsável pela execução dos casos relacionados à sua respectiva funcionalidade.] |

### 2.5 Critérios

| Critério | Definição da equipe |
|---|---|
| Entrada | [Aplicação LocalEats disponível, acesso à internet, usuário cadastrado e restaurantes disponíveis para realizar a busca por culinária e os testes de favoritar e desfavoritar.] |
| Saída | [Todos os casos de teste planejados para as funcionalidades de busca por culinária e de favoritar/desfavoritar estiverem especificados e relacionados aos respectivos riscos e técnicas.] |
| Suspensão | [Indisponibilidade da aplicação, impossibilidade de realizar login ou ausência de restaurantes e dados necessários para executar os casos de teste.] |

---

## 3. Tarefa 2: Riscos e técnicas de teste

### 3.1 Análise dos riscos

> Cada integrante deve analisar pelo menos um risco relacionado à funcionalidade escolhida. No trabalho individual, devem ser analisados dois riscos.

| ID | Integrante | Funcionalidade | Risco | Consequência | Probabilidade | Impacto | Prioridade | Justificativa |
|---|---|---|---|---|:---:|:---:|:---:|---|
| R01 | [Alessandro] | [Favoritar e Desfavoritar] | [Não registrar o favoritos ou o desfavorito] | [Cliente perde acesso aos restaurantes favoritados pelo mau funcionamento do sistema de favoritos] | [Baixa] | [Médio] | [Baixa] | [Se o sistema de favoritos não funcionar, pode acabar com a experiência do usuário, fazendo o usuário usar o serviço da concorrência] |
| R02 | [Ramon] | [Buscar restaurantes por culinária] | [O sistema apresentar restaurantes que não correspondem à culinária pesquisada.] | [O usuário poderá encontrar resultados incorretos e ter dificuldade para localizar restaurantes da culinária desejada.] | [Média] | [Alto] | [Média] | [A busca é utilizada para localizar restaurantes específicos, portanto resultados incorretos podem comprometer diretamente a utilização da funcionalidade.] |

> Acrescentem as linhas necessárias e mantenham identificadores únicos: R01, R02, R03 etc.

### 3.2 Aplicação das técnicas

> Cada integrante deve aplicar pelo menos uma técnica adequada à funcionalidade e ao risco analisado. A equipe deve utilizar, no conjunto da atividade, pelo menos duas técnicas diferentes.

#### Análise do integrante 1

**Integrante:** [nome]  
**Funcionalidade:** [preencher]  
**Risco relacionado:** [R01]  
**Técnica escolhida:** [particionamento de equivalência, análise de valor limite, tabela de decisão ou transição de estados]

**Por que a técnica foi escolhida:**  
[Expliquem por que a técnica é adequada à regra ou ao risco analisado.]

**Aplicação da técnica:**  
[Apresentem as classes, limites, combinações ou transições identificadas. Utilizem uma tabela ou lista quando necessário.]

**Casos derivados:** [CT01 e CT02]

#### Análise do integrante 2

**Integrante:** [nome]  
**Funcionalidade:** [preencher]  
**Risco relacionado:** [R02]  
**Técnica escolhida:** [preencher]

**Por que a técnica foi escolhida:**  
[preencher]

**Aplicação da técnica:**  
[preencher]

**Casos derivados:** [preencher]

> Repitam ou removam a seção de análise conforme o número de integrantes.

---

## 4. Tarefa 3: Casos de teste e rastreabilidade

### 4.1 Casos de teste

> No trabalho individual, elabore três casos. No trabalho em equipe, cada integrante deve elaborar pelo menos dois casos relacionados à própria funcionalidade.

### CT01: [Título do caso]

**Integrante responsável:** [nome]  
**Funcionalidade:** [preencher]  
**Risco ou requisito relacionado:** [R01 ou descrição do requisito]  
**Técnica utilizada:** [preencher]

**Pré-condição:**  
[O que precisa existir ou estar preparado antes da execução.]

**Dados de entrada:**  
[Valores ou dados necessários. Caso não sejam necessários, registrem “Não se aplica”.]

**Passos:**

1. [Primeiro passo.]
2. [Segundo passo.]
3. [Terceiro passo.]

**Resultado esperado:**  
[Comportamento observável que indicará que o teste passou.]

---

### CT02: [Título do caso]

**Integrante responsável:** [nome]  
**Funcionalidade:** [preencher]  
**Risco ou requisito relacionado:** [preencher]  
**Técnica utilizada:** [preencher]

**Pré-condição:**  
[preencher]

**Dados de entrada:**  
[preencher]

**Passos:**

1. [Primeiro passo.]
2. [Segundo passo.]
3. [Terceiro passo.]

**Resultado esperado:**  
[preencher]

---

> Copiem o modelo acima e continuem a numeração para criar os demais casos: CT03, CT04, CT05 etc.

### 4.2 Matriz de rastreabilidade

| Integrante | Funcionalidade | Risco ou requisito | Técnica utilizada | Casos de teste |
|---|---|---|---|---|
| [nome] | [funcionalidade] | [R01 ou requisito] | [técnica] | [CT01 e CT02] |
| [nome] | [funcionalidade] | [R02 ou requisito] | [técnica] | [CT03 e CT04] |

> Acrescentem as linhas necessárias. Verifiquem se todos os riscos selecionados possuem casos de teste relacionados.

---

## 5. Uso de inteligência artificial

**Ferramenta utilizada:**  
[Informar a ferramenta ou registrar “não utilizada”.]

**Como foi utilizada:**  
[Descrever brevemente.]

**Uma sugestão que precisou ser alterada ou rejeitada:**  
[Descrever brevemente. Caso nenhuma sugestão tenha sido rejeitada, expliquem como as sugestões foram analisadas criticamente.]

**Como as respostas foram verificadas:**  
[Descrever brevemente.]
