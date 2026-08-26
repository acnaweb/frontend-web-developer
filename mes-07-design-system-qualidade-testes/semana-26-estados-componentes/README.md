# Semana 26 — Estados e Acessibilidade de Componentes

## Objetivos

Garantir que componentes respondam corretamente aos estados de interação e permaneçam acessíveis.

Ao final desta semana, você deverá ser capaz de:

- explicar os principais conceitos com suas próprias palavras;
- relacionar os conceitos ao estudo de caso da NexusShop;
- interpretar o diagrama da solução;
- executar o laboratório proposto;
- registrar o resultado no GitHub.

---

## 1. Conceitos

### 1. Default

Estado normal do componente.

### 2. Hover

Feedback para dispositivos que suportam apontador.

### 3. Focus

Indica o elemento que receberá interação por teclado.

### 4. Active

Representa interação em andamento.

### 5. Disabled

Indica indisponibilidade; deve ser usado com cuidado.

### 6. Loading

Comunica que uma ação está sendo processada.

### 7. Error

Comunica falha de entrada ou operação.

### 8. Keyboard Interaction

Componentes precisam respeitar padrões esperados de teclado.

---

## 2. Estudo de Caso — NexusShop

Usuários que navegam por teclado não conseguem identificar o foco em alguns controles da NexusShop. Além disso, botões durante loading ainda podem ser pressionados novamente.

### O que devemos observar

O foco do estudo de caso não é apenas implementar uma solução, mas entender **por que** determinada técnica é utilizada, quais problemas ela resolve e como se conecta às demais etapas do roadmap.

---

## 3. Diagrama

```mermaid
stateDiagram-v2
    [*] --> Default
    Default --> Hover
    Default --> Focus
    Hover --> Active
    Focus --> Active
    Active --> Loading
    Loading --> Default: sucesso
    Loading --> Error: falha
    Default --> Disabled
```

---

## 4. Laboratório

### Objetivo do laboratório

Aplicar os conceitos da semana em uma evolução prática da NexusShop.

### Passo a passo

1. Defina todos os estados do Button.
2. Crie estilo de foco visível.
3. Implemente `aria-busy` quando apropriado.
4. Garanta que loading impeça múltiplos submits.
5. Teste a navegação usando apenas Tab, Shift+Tab, Enter e Space.
6. Revise contraste dos estados.

### Evidências esperadas

- código versionado;
- commits relacionados à atividade;
- documentação quando aplicável;
- captura de tela ou link quando a atividade envolver interface;
- README atualizado quando houver mudança importante na forma de executar o projeto.

### Entrega

Componentes com matriz de estados documentada e navegáveis por teclado.

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
