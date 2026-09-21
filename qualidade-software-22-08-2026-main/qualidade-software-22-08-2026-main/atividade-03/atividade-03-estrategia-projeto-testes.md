# Atividade 3: Estratégia e Projeto de Testes do LocalEats

> Substituam os campos entre colchetes pelas respostas da equipe e removam as instruções antes da entrega.

## 1. Identificação

**Turma:** ADS5M26-2C
**Equipe:** Alessandro e Ramon.  
**Data:** 20/09/2026

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

**Integrante:** [Alessandro]  
**Funcionalidade:** [Favoritar e desfavoritar restaurantes]  
**Risco relacionado:** [R02]  
**Técnica escolhida:** [tabela de decisão]

**Por que a técnica foi escolhida:**  
[Transição de estados foi escolhida pois o sistema de favoritos é um valor booleano e de listas.]

**Aplicação da técnica:**  
| Regra | [Tá logado] | [Foi favoritado] | [Resultado] |
|:---|:---:|:---:|:---|
| Regra | [Sim] | [Não] | [Não foi registrado no favorito] |
| Regra | [Não] | [Sim] | [Requer entrar na conta] |
| Regra | [Sim] | [Sim] | [Foi registrado o favorito] |
| Regra | [Não] | [Não] | [Requer entrar na conta] |

**Casos derivados:** [CT01 e CT02]

#### Análise do integrante 2

**Integrante:** [Ramon]  
**Funcionalidade:** [Buscar restaurantes por culinária]  
**Risco relacionado:** [R01]  
**Técnica escolhida:** [Particionamento de equivalência]

**Por que a técnica foi escolhida:**  
[A técnica de particionamento de equivalência foi escolhida porque permite dividir as entradas da busca por culinária em diferentes classes, considerando situações em que a pesquisa deve retornar restaurantes e situações em que não deve apresentar resultados correspondentes.]

**Aplicação da técnica:**  
| Classe | Entrada | Resultado esperado |
|:---|:---|:---|
| Classe válida | Culinária existente, como “Pizza” | O sistema deve apresentar restaurantes correspondentes à culinária pesquisada. |
| Classe inválida | Culinária sem restaurantes correspondentes | O sistema não deve apresentar restaurantes que não correspondam à pesquisa e deve informar que não foram encontrados resultados. |

**Casos derivados:** [CT03 e CT04]


---

## 4. Tarefa 3: Casos de teste e rastreabilidade

### 4.1 Casos de teste

> No trabalho individual, elabore três casos. No trabalho em equipe, cada integrante deve elaborar pelo menos dois casos relacionados à própria funcionalidade.

### CT01: [Favoritar]

**Integrante responsável:** [Alessandro]  
**Funcionalidade:** [Favoritar]  
**Risco ou requisito relacionado:** [R01]  
**Técnica utilizada:** [transição de estados]

**Pré-condição:**  
[Criação de conta ou a existencia de uma conta]

**Dados de entrada:**  
[Valor verdadeiro no favorito do restaurante]

**Passos:**
┌─────────┐<br>
│Tá logado│<br>
└─────────┘<br>
↓ ┌─────────┐<br>
↓→│Deslogado│<br>
↓ └─────────┘<br>
┌────────────────────────┐<br>
│Tá página do restaurante│<br>
└────────────────────────┘<br>
↓<br>
┌─────────────────────┐<br>
│Favoritar restaurante│<br>
└─────────────────────┘<br>
↓<br>
┌─────────┐<br>
│Concluido│<br>
└─────────┘<br>

**Resultado esperado:**  
[Tirar o restaurante dos registros dos Meus Favoritos]

---

### CT02: [Desfavoritar]

**Integrante responsável:** [Alessandro]  
**Funcionalidade:** [Desfavoritar]  
**Risco ou requisito relacionado:** [R02]  
**Técnica utilizada:** [transição de estados]

**Pré-condição:**  
[Criação de conta ou a existencia de uma conta]

**Dados de entrada:**  
[Valor verdadeiro no favorito do restaurante]

**Passos:**
┌─────────┐<br>
│Tá logado│<br>
└─────────┘<br>
↓ ┌─────────┐<br>
↓→│Deslogado│<br>
↓ └─────────┘<br>
┌───────────────────────────┐<br>
│Tá na página Meus Favoritos│<br>
└───────────────────────────┘<br>
↓<br>
┌────────────────────────┐<br>
│Desfavoritar restaurante│<br>
└────────────────────────┘<br>
↓<br>
┌─────────┐<br>
│Concluido│<br>
└─────────┘<br>

**Resultado esperado:**  
[Registrar o restaurante nos Meus Favoritos]

---

### CT03: [Buscar por restaurante por uma culinária existente]

**Integrante responsável:** [Ramon]  
**Funcionalidade:** [Buscar restaurantes por culinária]  
**Risco ou requisito relacionado:** [R01 , o sistema apresentar restaurantes que não correspondem a culinária pesquisada]  
**Técnica utilizada:** [Particionamento de equivalência]

**Pré-condição:**  
[O usuário deve estar com o LocalEats disponivel no navegador e deve existir pelo menos um restaurante cadastrado para a culinária que será pesquisada]

**Dados de entrada:**  
[Culinária: "Pizza"]

**Passos:**

1. [Acessar o LocalEats e realizar login na conta do usuário.]
2. [Acessar a funcionalidade de busca e informar uma culinária existente, como “Pizza”.]
3. [Realizar a busca e verificar os restaurantes apresentados.]

**Resultado esperado:**  
[O sistema deve apresentar restaurantes que correspondam à culinária pesquisada, permitindo que o usuário encontre opções relacionadas à busca realizada.]

---
---

### CT04: [Buscar restaurantes por uma culinária sem correspondência]

**Integrante responsável:** [Ramon]  
**Funcionalidade:** [Buscar restaurantes por culinária]  
**Risco ou requisito relacionado:** [R01 — O sistema apresentar restaurantes que não correspondem à culinária pesquisada.]  
**Técnica utilizada:** [Particionamento de equivalência]

**Pré-condição:**  
[O usuário deve estar com o LocalEats disponível no navegador e deve existir pelo menos um restaurante cadastrado no sistema, mas nenhum restaurante deve corresponder à culinária pesquisada.]

**Dados de entrada:**  
[Culinária: “Culinária inexistente”.]

**Passos:**

1. [Acessar o LocalEats e realizar login na conta do usuário.]
2. [Acessar a funcionalidade de busca e informar uma culinária que não possua restaurantes correspondente]
3. [Realizar a busca e verificar os resultados apresentados pelo sistema.]

**Resultado esperado:**  
[O sistema não deve apresentar restaurantes que não correspondam à culinária pesquisada e deve informar ao usuário que não foram encontrados restaurantes correspondentes à busca.]

---

> Copiem o modelo acima e continuem a numeração para criar os demais casos: CT03, CT04, CT05 etc.

### 4.2 Matriz de rastreabilidade

| Integrante | Funcionalidade | Risco ou requisito | Técnica utilizada | Casos de teste |
|---|---|---|---|---|
| [nome] | [funcionalidade] | [R01] | [Tabela de decisão] | [CT01] |
| [nome] | [funcionalidade] | [R01] | [Transição de estados] | [CT02] |
| [Ramon] | [Buscar restaurantes por culinária] | [R01] | [Particionamento de equivalência] | [CT03 e CT04] |

> Acrescentem as linhas necessárias. Verifiquem se todos os riscos selecionados possuem casos de teste relacionados.

---

## 5. Uso de inteligência artificial

**Ferramenta utilizada:**  
[Gemini e LanguageTool]

**Como foi utilizada:**  
[O Gemini foi usado para corrigir a transição de estados feita com caracteres especiais e também as tabelas quebradas no .md.
O LanguageTool foi usado para corrigir o texto.]

**Uma sugestão que precisou ser alterada ou rejeitada:**  
[Foram alteradas estruturas de tabelas, gráficos quebrados ou escritos com erros de português.]

**Como as respostas foram verificadas:**  
[Não teve verificação do texto para saber se estamos certos ou não, mas usamos IA para corrigir textos e estruturas que, na prévia, ficavam quebradas.]
