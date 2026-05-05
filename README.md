# Projeto de Prática Profissional em ADS
## Grupo 18

### Pré-requisitos
Ter o Python instalado no computador (versão 3.8 ou superior)

### Execução
Abra o terminal, navegue até a pasta onde o projeto foi salvo e execute o programa principal: 
``gerenciador_tarefas.py``
O sistema abrirá uma tela no navegador e estará pronto para usar. 

# Gerenciador de Tarefas (Aplicação Desktop com Tkinter)

## 1. Descrição

Aplicação desktop desenvolvida em Python com a biblioteca Tkinter para gerenciamento de tarefas pessoais. O sistema permite criar, editar, excluir e marcar tarefas como concluídas por meio de uma interface gráfica responsiva.

---

## 2. Funcionalidades

* Inserção de novas tarefas
* Edição de tarefas existentes
* Exclusão de tarefas com confirmação
* Marcação e desmarcação de tarefas como concluídas
* Interface com rolagem para listas extensas
* Atualização dinâmica da interface

---

## 3. Tecnologias Utilizadas

* Python 3
* Tkinter (biblioteca padrão para interfaces gráficas)

---

## 4. Pré-requisitos

* Python versão 3.8 ou superior instalado

Verificação da instalação:

```bash
python --version
```

ou

```bash
python3 --version
```

Não há dependências externas, pois o Tkinter é distribuído junto ao Python.

---

## 5. Instruções de Execução

### 5.1 Clonar o repositório

```bash
git clone https://github.com/victoriapacch/grp18/
```

### 5.2 Acessar o diretório do projeto

```bash
cd grp18
```

### 5.3 Executar a aplicação

```bash
python gerenciador_tarefas.py
```

ou

```bash
python3 gerenciador_tarefas.py
```

---

## 6. Uso da Aplicação

### 6.1 Adicionar tarefa

* Inserir o texto no campo de entrada
* Acionar o botão "Adicionar" ou pressionar Enter

### 6.2 Marcar tarefa como concluída

* Selecionar o checkbox correspondente

### 6.3 Editar tarefa

* Acionar o botão de edição
* Informar o novo texto na janela de diálogo

### 6.4 Excluir tarefa

* Acionar o botão de exclusão
* Confirmar a operação

---

## 7. Estrutura do Sistema

A aplicação é estruturada em uma classe principal:

* `GerenciadorTarefas`: responsável pela inicialização da interface, gerenciamento do estado e manipulação das tarefas

### Componentes principais:

* Interface gráfica construída com:

  * `Frame`
  * `Entry`
  * `Button`
  * `Label`
  * `Canvas` e `Scrollbar`
* Sistema de eventos (bindings) para interação do usuário
* Atualização dinâmica da interface via renderização da lista

---

## 8. Estrutura de Dados

As tarefas são armazenadas em memória como uma lista de dicionários:

```python
{
    "texto": "Descrição da tarefa",
    "feito": False
}
```

---

## 9. Persistência de Dados

A aplicação não implementa persistência. Os dados são mantidos apenas em memória durante a execução. Ao encerrar o programa, as informações são descartadas.

---

## 10. Limitações

* Ausência de armazenamento persistente
* Não há categorização ou priorização de tarefas
* Não possui suporte a múltiplos usuários

---

## 11. Possíveis Evoluções

* Implementação de persistência (arquivo JSON ou banco de dados)
* Inclusão de filtros de visualização
* Adição de campos como prioridade e data
* Internacionalização da interface
* Migração para arquitetura baseada em camadas (MVC)

---

## 12. Versionamento

* Tag `v2`: corresponde à implementação da Iteração 2 do projeto, incluindo melhorias na interface e nas funcionalidades básicas de manipulação de tarefas

---

## 13. Execução em Diferentes Sistemas

### Windows

Utilizar o comando:

```bash
python gerenciador_tarefas.py
```

### Linux

Caso o Tkinter não esteja instalado:

```bash
sudo apt-get install python3-tk
```

Execução:

```bash
python3 gerenciador_tarefas.py
```

### macOS

O Tkinter geralmente já acompanha o Python instalado. Caso necessário, instalar via Homebrew:

```bash
brew install python-tk
```

Execução:

```bash
python3 gerenciador_tarefas.py
```

---
