# Desafio 01 | Conceitos do react

## Objetivo
O desafio consiste em criar as seguintes funcionalidades no arquivo `components/TaskList.tsx`:
  #### *handleCreateNewTask*:
  Deve ser possível adicionar uma nova task no estado de `tasks`, com os campos `id` que deve ser gerado de forma aleatória, `title` que deve ser um texto e `isComplete` que deve iniciar como false.
  
  As tasks criadas:
- devem ser exibidas em tela;
- devem conter os atributos seguindo o padrão da interface, que é:

      ```tsx
      interface Task {
        id: number;
        title: string;
        isComplete: boolean;
      }
      ```
  
#### *handleToggleTaskCompletion*:
Deve alterar o status de `isComplete` para uma task com um ID específico que é recebido por parâmetro.

#### *handleRemoveTask*:
Deve receber um ID por parâmetro e remover a task que contém esse ID do estado.
  

## Especificação dos testes

Para esse desafio, temos os seguintes testes:

#### **Arquivo**:  `TaskList.spec.tsx`

### Casos de teste
#### should be able to add a task
    Dado um input
    Quando clicar em ok
    Então deverá ser criada uma task com id aleatório, não completa(isComplete: false) e com o título informado;

#### should not be able to add a task with an empty title
    Dado um input vazio
    Quando clicar em ok
    Então não deverá ser criada uma task.


#### should be able to remove a task
    Dado uma task listada
    Quando clicar no botão com ícone de uma lixeira ao lado direito da task
    Então a task deverá ser removida da listagem.


#### should be able to check a task
    Dado uma task listada ainda não concluída
    Quando clicar no checkbox ao lado da task
    Então ela deverá ser marcada como concluída;

    Dado uma task lista completa
    Quando clicar no checkbox ao lado da task
    Então ela deverá ser marcada como não concluída;


## Como deve ficar a aplicação ao final?

<video src='https://github.com/ncgc/desafio01_conceitos_do_react/blob/a6f1c828d8be2481021999292ed417738242be6a/challenge2.mp4' />

