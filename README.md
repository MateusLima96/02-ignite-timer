# Módulo do curso Aprofundando conhecimento em Hooks pela @RocketSeat

# Context API no React

A **Context API** do React é uma ferramenta poderosa para compartilhar dados entre componentes em uma aplicação React, evitando a necessidade de passar props manualmente em cada nível da árvore de componentes. Isso ajuda a resolver o problema conhecido como **prop drilling**.

## O que é Prop Drilling?

**Prop drilling** ocorre quando você precisa passar dados de um componente pai para um componente filho distante na hierarquia de componentes, atravessando vários níveis intermediários que não utilizam esses dados diretamente. Esse padrão torna o código difícil de manter e propenso a erros.

## Como a Context API Ajuda?

A **Context API** permite criar um contexto que pode ser acessado por qualquer componente, em qualquer nível da árvore, sem a necessidade de passar props manualmente. Isso é feito através de dois componentes principais: o **Provider** e o **Consumer**.

### Passos para Usar a Context API

1. **Criação do Contexto:** Crie um contexto usando `React.createContext()`.
2. **Provider:** Utilize o `Provider` para envolver a parte da árvore de componentes onde o contexto deve ser acessível e forneça o valor a ser compartilhado.
3. **Consumer:** Utilize o `Consumer` ou o hook `useContext` para acessar o contexto em componentes filhos.

### Exemplo de Código
 
[CyclesContext.tsx](src/contexts/CyclesContext.tsx) criação do contexto.

![image](https://github.com/user-attachments/assets/74047a24-9b0f-42cc-968c-e72e2b4d19f8)

![image](https://github.com/user-attachments/assets/0fc90750-1c3d-416e-b2e7-6ec44ec73aa8)


[App.tsx](src/App.tsx) fazendo o contexto ser reconhecido na aplicação englobando todas as rotas.

![image](https://github.com/user-attachments/assets/4fb1a7d6-d467-437f-9223-ed4217a5d78b)

