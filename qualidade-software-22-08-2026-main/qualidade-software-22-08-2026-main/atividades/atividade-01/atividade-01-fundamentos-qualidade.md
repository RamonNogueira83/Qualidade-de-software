# Atividade 1: Fundamentos e Características da Qualidade no LocalEats

> Substituam os campos entre colchetes pelas respostas da equipe e removam as instruções antes da entrega.

## 1. Identificação

**Turma:** ADS5M26-2C
**Equipe:** Alessandro e Ramon.
**Data:** 22/08/2026

### Integrantes

| Nome                     | Usuário no GitHub      |
| ------------------------ | ---------------------- |
| Alessandro Reis da Silva | @AlessandroReisDaSilva |
| Ramon Nogueira           | @Ramonnogueira83       |

**Elemento de Competência:** Compreender os fundamentos de qualidade de software e sua aplicação no desenvolvimento de sistemas.

**Aplicação:** https://local-eats-unisenac.vercel.app/

---

## 2. Tarefa 1: Fundamentos da qualidade

### 2.1 Necessidades explícitas e implícitas

| Tipo      | Necessidade                                                                                                                 | Interessado           | Consequência se não for atendida                                                                                                                                                               |
| --------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Explícita | Permitir que o usuário faça pedidos.                                                                                        | Usuário               | O usuário não conseguirá realizar pedidos pelo sistema.                                                                                                                                        |
| Explícita | Permitir que o usuário favorite e desfavorite restaurantes.                                                                 | Usuário               | O usuário não conseguirá adicionar restaurantes aos seus favoritos ou removê-los posteriormente.                                                                                               |
| Implícita | Permitir que o usuário favorite e desfavorite restaurantes de forma simples e consistente na própria página do restaurante. | Usuário               | O usuário poderá ter dificuldade para desfazer uma ação realizada anteriormente, sendo necessário acessar outra página para remover o restaurante dos favoritos, prejudicando sua experiência. |
| Implícita | Apresentar informações claras que auxiliem o usuário na escolha de um restaurante.                                          | Usuário e restaurante | O usuário poderá ter dificuldade para escolher um restaurante e o estabelecimento poderá ter sua apresentação prejudicada dentro da aplicação.                                                 |

### 2.2 Questão sobre os fundamentos da qualidade

**Um sistema que implementa todas as funcionalidades explicitamente solicitadas pode, ainda assim, apresentar baixa qualidade? Justifiquem utilizando pelo menos uma necessidade implícita identificada pela equipe.**

Sim. Um sistema pode implementar todas as funcionalidades solicitadas e ainda apresentar problemas de qualidade. No LocalEats, por exemplo, é possível favoritar um restaurante pela sua página, porém não é possível desfavoritá-lo pelo mesmo botão na página do restaurante. Para remover o restaurante dos favoritos, é necessário acessar a página de favoritos, tornando a utilização menos fluida e prejudicando a experiência do usuário.

---

## 3. Tarefa 2: Exploração da aplicação

> Cada integrante deve explorar uma funcionalidade, realizando uma utilização esperada e uma utilização alternativa, inválida ou incompleta. Acrescentem ou removam linhas conforme o número de integrantes.

| Integrante               | Funcionalidade       | O que foi realizado                                                                                                                                                                                                                                             | O que foi observado                                                                                                                                                                                              | Evidência                                                    |
| ------------------------ | -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| Alessandro Reis da Silva | Favoritos            | Foi realizado o processo de favoritar um restaurante pela página do restaurante e, posteriormente, foi realizada uma tentativa de desfavoritar o mesmo restaurante pela própria página. Também foi realizada a remoção do restaurante pela página de favoritos. | Ao salvar o restaurante como favorito pela página do restaurante, não foi possível desfazer a ação pelo mesmo botão. Para remover o restaurante dos favoritos, foi necessário acessar a página de favoritos.     | [ver evidência](Evidencias/Favoritar.mkv)                    |
| Ramon Nogueira           | Buscar por culinária | Foi realizada uma pesquisa utilizando uma culinária desejada por meio da barra de pesquisa. Também foi utilizado o filtro de culinária disponível na aplicação para comparar os resultados.                                                                     | Ao pesquisar pela culinária desejada utilizando a barra de pesquisa, o sistema não retornou o resultado esperado. O comportamento observado foi diferente do resultado obtido ao utilizar o filtro de culinária. | [ver evidência](Evidencias/Pesquisa-de-estilo-culinario.png) |

---

## 4. Tarefa 3: Requisitos e características de qualidade

> Cada integrante deve formular um requisito de qualidade relacionado à mesma funcionalidade explorada na Tarefa 2. Acrescentem ou removam linhas conforme o número de integrantes.

| Integrante               | Requisito de Qualidade                                                                                                                                                                                           | Característica ou subcaracterística      | Justificativa                                                                                                                                                                                                                                                                                                          | Como avaliar                                                                                                                                                                                                                                                                   |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Alessandro Reis da Silva | O sistema deve permitir que o usuário adicione e remova restaurantes dos favoritos de forma simples e consistente, permitindo realizar a ação de favoritar ou desfavoritar diretamente na página do restaurante. | Usabilidade — operabilidade              | A funcionalidade de favoritos deve permitir que o usuário controle facilmente o estado do restaurante. Durante a exploração, foi observado que era possível favoritar o restaurante pela página do restaurante, mas não era possível desfazer a ação pelo mesmo local, sendo necessário acessar a página de favoritos. | Favoritar um restaurante pela página do restaurante e, em seguida, tentar desfavoritá-lo pelo mesmo local. Observar se a ação pode ser realizada diretamente e comparar a quantidade de etapas necessárias para adicionar e remover o favorito.                                |
| Ramon Nogueira           | O sistema deve apresentar resultados de pesquisa compatíveis com a culinária ou localização informada pelo usuário.                                                                                              | Adequação funcional — correção funcional | A pesquisa é utilizada para localizar restaurantes de acordo com os critérios informados pelo usuário. Durante a exploração, foi observado que a pesquisa pela barra de pesquisa não apresentou o resultado esperado em comparação com o filtro de culinária.                                                          | Realizar pesquisas utilizando diferentes culinárias e localizações e comparar os resultados apresentados com os critérios informados. Também pode ser realizada uma comparação entre os resultados da barra de pesquisa e os resultados obtidos pelos filtros correspondentes. |

---

## 5. Uso de inteligência artificial

**Ferramenta utilizada:**
ChatGPT.

**Como foi utilizada:**
A ferramenta foi utilizada como apoio para organizar as informações, revisar a estrutura do documento.

**Como as respostas foram verificadas:**
As sugestões foram comparadas com as orientações da atividade e verificadas pelos integrantes durante a exploração da aplicação LocalEats.
