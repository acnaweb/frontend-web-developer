# Semana 20 — React Router e Navegação

## Objetivos

Estruturar navegação cliente, parâmetros de rota e layouts compartilhados.

Ao final desta semana, você deverá ser capaz de:

- explicar os principais conceitos com suas próprias palavras;
- relacionar os conceitos ao estudo de caso da NexusShop;
- interpretar o diagrama da solução;
- executar o laboratório proposto;
- registrar o resultado no GitHub.

---

## 1. Conceitos

### 1. SPA

Aplicação que atualiza a interface sem solicitar um novo documento HTML completo a cada navegação.

### 2. Router

Mapeia URLs para componentes.

### 3. Route Params

Representam partes variáveis do caminho, como `/products/:id`.

### 4. Query Params

Representam filtros ou opções, como `?category=books`.

### 5. Nested Routes

Permitem rotas dentro de layouts ou seções.

### 6. Layout

Estrutura compartilhada entre diferentes páginas.

---

## 2. Estudo de Caso — NexusShop

A NexusShop agora terá Home, Catálogo, Detalhe do Produto, Carrinho e Checkout.

### O que devemos observar

O foco do estudo de caso não é apenas implementar uma solução, mas entender **por que** determinada técnica é utilizada, quais problemas ela resolve e como se conecta às demais etapas do roadmap.

---

## 3. Diagrama

```mermaid
flowchart TD
    ROOT[/] --> HOME[Home]
    ROOT --> PRODUCTS[/products]
    PRODUCTS --> DETAIL[/products/:id]
    ROOT --> CART[/cart]
    ROOT --> CHECKOUT[/checkout]
```

---

## 4. Laboratório

### Objetivo do laboratório

Aplicar os conceitos da semana em uma evolução prática da NexusShop.

### Passo a passo

1. Instale React Router.
2. Crie `BrowserRouter`.
3. Implemente as rotas principais.
4. Crie layout com Header e Footer compartilhados.
5. Use parâmetro `:id` no detalhe do produto.
6. Utilize query string para categoria no catálogo.
7. Crie página 404.

### Evidências esperadas

- código versionado;
- commits relacionados à atividade;
- documentação quando aplicável;
- captura de tela ou link quando a atividade envolver interface;
- README atualizado quando houver mudança importante na forma de executar o projeto.

### Entrega

Navegação completa da NexusShop por URLs significativas.

---

## 5. Perguntas para revisão

1. Qual problema principal os conceitos desta semana resolvem?
2. Qual é o erro mais comum ao aplicar esses conceitos?
3. Como o conteúdo desta semana se conecta à semana anterior?
4. Como você explicaria a solução implementada para outro desenvolvedor?
5. O que mudaria em um projeto real de maior escala?

---

## 6. Checklist da semana

- [ ] Estudei os conceitos.
- [ ] Entendi o estudo de caso.
- [ ] Interpretei o diagrama Mermaid.
- [ ] Executei o laboratório.
- [ ] Registrei as evidências no GitHub.
- [ ] Revisei os principais aprendizados.

---

[Voltar para o mês](../README.md) | [Voltar para o roadmap](../../README.md)
