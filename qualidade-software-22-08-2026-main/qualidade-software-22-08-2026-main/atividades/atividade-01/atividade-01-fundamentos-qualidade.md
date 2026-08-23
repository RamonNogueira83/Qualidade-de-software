# Atividade 1: Fundamentos e Características da Qualidade no LocalEats

> Substituam os campos entre colchetes pelas respostas da equipe e removam as instruções antes da entrega.

## 1. Identificação

**Turma:** ADS5M26-2C
**Equipe:** Alessandro e Ramon.  
**Data:** 22/08/2026

### Integrantes

|           Nome           |     Usuário no GitHub    |
|--------------------------|--------------------------|
| Alessandro Reis da Silva | @AlessandroReisDaSilva |
|      Ramon nogueira      |         @Ramonnogueira83         |

**Elemento de Competência:** Compreender os fundamentos de qualidade de software e sua aplicação no desenvolvimento de sistemas.

**Aplicação:** <https://local-eats-unisenac.vercel.app/>

---

## 2. Tarefa 1: Fundamentos da qualidade

### 2.1 Necessidades explícitas e implícitas

|    Tipo   |                             Necessidade                        | Interessado |                                             Consequência se não for atendida                                                        |
|-----------|----------------------------------------------------------------|-------------|-------------------------------------------------------------------------------------------------------------------------------------|
| Explícita |                        Fazer pedido                            |   Usuário   |                                              Não conseguira fazer pedidos                                                           |
| Explícita |             Favoritar e desfavoritar restaurantes              |   Usuário   |                               Não conseguira colocar nos meu favoritos e visualiza-los                                              |
| Implícita | Favoritar e desfavoritar restaurantes na página do restaurante |   Usuário   |   Ao salvar o restaurante como favorito, não é possível desfazer a ação pelo mesmo botão, somente indo até a pagina meus favoritos, isso prejudica a experiencia do usuário  |
| Implícita | Mostrar quantos usuários salvaram aquele restaurante           |  Usuário/Restaurante |  Para o usuário fica melhor, pois consegue ver quantos clientes recomendam ou quantos aprovam aquele restaurante. Já pelo lado do restaurante, os proprietarios conseguem saber, como está a imagem publica de seu restaurante dentro do aplicativo |

### 2.2 Questão sobre os fundamentos da qualidade

**Um sistema que implementa todas as funcionalidades explicitamente solicitadas pode, ainda assim, apresentar baixa qualidade? Justifiquem utilizando pelo menos uma necessidade implícita identificada pela equipe.**

[Resposta da equipe em até cinco linhas.]
Favoritar e desfavoritar possui um problema que ao favoritar na página do restaurante, onde ao interagir com o botão de favoritar, favoritara, mas ao fazer a mesma ação não desfavoritara o restaurante na página dele, fazendo o cliente ir aos meus favoritos. Deixando o sistema de favoritos menos fluido e mais desconfortável para o cliente.

---

## 3. Tarefa 2: Exploração da aplicação

> Cada integrante deve explorar uma funcionalidade, realizando uma utilização esperada e uma utilização alternativa, inválida ou incompleta. Acrescentem ou removam linhas conforme o número de integrantes.

| Integrante | Funcionalidade | O que foi realizado | O que foi observado | Evidência |
|-------------|----------------|---------------------|---------------------|-----------|
| Alessandro Reis da Silva | Fazer pedido | Foi feito o pedido esperando que o cliente aperte finalizar pedido | Ao cliente fazer o pedido o pedido vai na espera da conformação do cliente, depois de confirmar, o pedido é registrado nos meus pedidos no histórico | [ver evidência](qualidade-software-22-08-2026-main/qualidade-software-22-08-2026-main/atividades/atividade-01/Evidencias/Pedido.png) |
| Alessandro Reis da Silva | Meus pedidos | Visualizar o histórico de pedidos | Carregar os históricos de pedidos | [ver evidência](qualidade-software-22-08-2026-main/qualidade-software-22-08-2026-main/atividades/atividade-01/Evidencias/Meus_Pedidos.png) |
| Alessandro Reis da Silva | Favoritos | Favoritar e desfavoritar pela página do restaurante e remover dos favoritos o restaurante pela página meus favoritos | Ao salvar o restaurante como favorito, não é possível desfazer a ação pelo mesmo botão, somente indo até a pagina meus favoritos. | [ver evidência](https://github.com/RamonNogueira83/Qualidade-de-software/raw/refs/heads/main/qualidade-software-22-08-2026-main/qualidade-software-22-08-2026-main/atividades/atividade-01/Evidencias/Favoritar.mkv) |
| Ramon Nogueira | Buscar por culinária | Mostrar todos os restaurantes com a culinária que foi pesquisada pelo usuário, e mostrar as melhores avaliadas em primeiro | ao pesquisar pela culinária desejada o sistema não retornou o resultado esperado, por mais que tenha o filtro de pesquisa, é importante o funcionamento da barra de pesquisa. | [ver evidência](https://github.com/RamonNogueira83/Qualidade-de-software/raw/refs/heads/main/qualidade-software-22-08-2026-main/qualidade-software-22-08-2026-main/atividades/atividade-01/Evidencias/Pesquisa.png) |

---

## 4. Tarefa 3: Requisitos e características de qualidade

> Cada integrante deve formular um requisito de qualidade relacionado à mesma funcionalidade explorada na Tarefa 2. Acrescentem ou removam linhas conforme o número de integrantes.

| Integrante | Requisito de Qualidade | Característica ou subcaracterística | Justificativa | Como avaliar |
|------------|------------------------|-------------------------------------|---------------|--------------|
|  Alessandro Reis da Silva | Sistema de favoritos fluido | Usabilidade e registro | Melhorar a qualidade do sistema | Comparei o sistema de favoritos com as outras plataformas |
|  Alessandro Reis da Silva| funcionamento de fazer e finalizar pedido | Usabilidade e registro | Melhorar a qualidade do sistema. | Avalie como funciona os pedidos. |
| Ramon Nogueira | O sistema deve apresentar os resultados da pesquisa de restaurantes de forma clara, permitindo que o usuário compreenda facilmente quando existem resultados e quando não existem resultados correspondentes. | Usabilidade — capacidade de reconhecimento da adequação | A pesquisa é utilizada para localizar restaurantes por especialidade ou localização. O usuário precisa compreender facilmente o resultado obtido após realizar uma pesquisa. | Realizar pesquisas com termos válidos, inválidos e sem correspondência. Observar se os resultados apresentados são claros e se é possível identificar facilmente quando uma pesquisa não encontrou resultados. |
| Ramon Nogueira | O sistema deve manter os dados do pedido corretamente durante as etapas de seleção, confirmação e finalização, evitando alterações ou perda das informações selecionadas pelo usuário. | Confiabilidade — tolerância a falhas | Durante a realização de um pedido, o usuário espera que os itens selecionados e as informações da operação sejam mantidos corretamente até sua finalização. | Realizar um pedido selecionando diferentes itens e avançar pelas etapas até a finalização. Comparar os itens e informações apresentados em cada etapa e verificar se permanecem consistentes. |

---

## 5. Uso de inteligência artificial

**Ferramenta utilizada:**
ChatGPT.

**Como foi utilizada:**
A ferramenta foi utilizada como apoio para organizar as informações, revisar a estrutura do documento.

**Como as respostas foram verificadas:**
As sugestões foram comparadas com as orientações da atividade e verificadas pelos integrantes durante a exploração da aplicação LocalEats.
