# 🚀 Coleção de Exercícios em C#

Este repositório contém um conjunto de aplicações de console desenvolvidas em **C# (.NET)**. Os projetos abrangem desde lógica de programação básica, manipulação de arrays e listas com LINQ, até implementações de estruturas de dados clássicas como Pilhas Dinâmicas.

## 📁 Estrutura do Repositório

O repositório é composto pelos seguintes programas:

* **`MediaSalarial.cs`**: Gerenciador de salários com validações de valores mínimos e cálculo de médias.
* **`PilhaObjeto.cs`**: Implementação manual de uma estrutura de dados do tipo Pilha (LIFO) usando referências a objetos.
* **`playlistMusicas.cs`**: Sistema de análise de dados (*Data Analytics*) de uma playlist musical utilizando **LINQ** e expressões Lambda.
* **`FolhaDePagamento.cs`**: Simulador para cálculo de folha de pagamento com descontos dinâmicos de INSS e IRRF baseados em faixas salariais.

---

## 🛠️ Detalhes de Cada Projeto

### 1. Sistema de Média Salarial (`MediaSalarial.cs`)
Solicita o nome e o salário de um conjunto de funcionários. Possui regras de validação para impedir a inserção de salários abaixo do mínimo estipulado (R$ 1400) e, ao final, exibe quem está acima da média e qual é o maior salário cadastrado.
* **Conceitos aplicados:** Loops (`for`, `do-while`), tratamento de strings, manipulação de arrays e métodos de validação (`float.TryParse`).

### 2. Estrutura de Dados: Pilha (`PilhaObjeto.cs`)
Uma implementação de **Pilha (Stack)** sem o uso de coleções nativas do C#. O código constrói a estrutura de forma dinâmica, onde cada elemento conhece o seu sucessor na memória.
* **Operações suportadas:**
    * `Push`: Insere um elemento no topo da pilha.
    * `Pop`: Remove e retorna o elemento do topo (com tratamento de erro para pilha vazia).
    * `Consulta`: Visualiza o elemento do topo sem removê-lo.
    * `Listar`: Exibe todos os elementos empilhados.

### 3. Port-A-Song Data Analytics (`playlistMusicas.cs`)
Uma aplicação que simula um painel de análise de dados para um catálogo de músicas. Utiliza o poder do **LINQ (Language Integrated Query)** para realizar consultas rápidas e filtragens eficientes no banco de dados simulado em memória.
* **Funcionalidades:**
    * Filtrar músicas por gênero.
    * Listar o Top 3 de músicas mais reproduzidas.
    * Calcular a média de duração de todo o catálogo.
    * Verificar a existência de um artista específico por correspondência parcial de nome.

### 4. Calculadora de Folha de Pagamento (`FolhaDePagamento.cs`)
Calcula o salário líquido de um funcionário após aplicar as alíquotas de desconto do **INSS** e do **IRRF** de forma progressiva/por faixas.
* **Regras de Negócio aplicadas:**
    * Validação para impedir salários negativos ou zerados.
    * Desconto progressivo de INSS (7.5% a 14% dependendo do valor).
    * Desconto de IRRF (7.5% para salários acima de R$ 1900).

---

## 💻 Como Executar os Projetos

### Pré-requisitos
* [.NET SDK](https://dotnet.microsoft.com/download) instalado em sua máquina.
* Um editor de código como o [VS Code](https://code.visualstudio.com/) ou o [Visual Studio](https://visualstudio.microsoft.com/).

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)