# 🚀 Coleção de Exercícios em C# (C-codes)

Este repositório contém um conjunto de aplicações de console desenvolvidas em **C# (.NET)**. Os projetos abrangem desde lógica de programação básica, validações e manipulação de listas com LINQ, até implementações manuais de estruturas de dados clássicas como Pilhas Dinâmicas.

## 📁 Estrutura do Repositório

O repositório é composto pelos seguintes programas:

* **`MediaSalarial.cs`**: Gerenciador que recebe dados de funcionários, valida limites mínimos de remuneração e calcula estatísticas sobre os salários.
* **`PilhaObjeto.cs`**: Implementação manual de uma estrutura de dados do tipo Pilha (LIFO - *Last In, First Out*) utilizando referências a objetos.
* **`playlistMusicas.cs`**: Painel de análise de dados (*Data Analytics*) de uma playlist musical utilizando **LINQ** e expressões Lambda.
* **`FolhaDePagamento.cs`**: Simulador para cálculo de salário líquido com descontos dinâmicos e progressivos de INSS e IRRF.

---

## 🛠️ Detalhes de Cada Projeto

### 1. Sistema de Média Salarial (`MediaSalarial.cs`)
Solicita o nome e o salário de um conjunto de funcionários. Possui uma estrutura de validação para impedir a inserção de valores abaixo do salário mínimo estipulado (R$ 1.400,00). Ao final, o programa calcula a média do grupo e exibe quais funcionários recebem acima dela, além de destacar o maior salário cadastrado.
* **Conceitos aplicados:** Loops (`for`, `do-while`), manipulação de arrays, tratamento de strings e validação de entrada de dados (`float.TryParse`).

### 2. Estrutura de Dados: Pilha (`PilhaObjeto.cs`)
Uma implementação de **Pilha (Stack)** feita de forma nativa e dinâmica, sem depender das coleções prontas do ecossistema .NET. Cada elemento funciona como um nó que armazena seu próprio valor e aponta para o próximo elemento na memória.
* **Operações suportadas:**
    * `Push`: Insere um novo elemento no topo da pilha.
    * `Pop`: Remove e retorna o elemento que está no topo (com tratamento de exceção caso a pilha esteja vazia).
    * `Consulta` (*Peek*): Visualiza o valor do topo atual sem removê-lo.
    * `Listar`: Percorre e exibe todos os elementos empilhados em tela.

### 3. Port-A-Song Data Analytics (`playlistMusicas.cs`)
Simula um painel analítico para um catálogo de músicas. O programa carrega uma lista de objetos em memória e disponibiliza um menu interativo que utiliza o poder do **LINQ (Language Integrated Query)** para processar as informações.
* **Funcionalidades do Menu:**
    1. Filtrar e listar músicas por um Gênero específico.
    2. Exibir o Top 3 de músicas mais ouvidas com base no número de reproduções.
    3. Calcular a média de duração (em segundos) de todo o catálogo.
    4. Verificar se um determinado artista existe na base por meio de busca parcial.

### 4. Calculadora de Folha de Pagamento (`FolhaDePagamento.cs`)
Uma ferramenta interativa que automatiza o cálculo do salário líquido de funcionários aplicando alíquotas de impostos retidos na fonte.
* **Regras de Negócio e Validações:**
    * Impede a inserção de salários menores ou iguais a zero.
    * Calcula o desconto progressivo do INSS em faixas que variam de 7,5% a 14%.
    * Aplica a retenção do IRRF (7,5%) para valores que ultrapassam o teto de R$ 1.900,00.
    * Exibe um demonstrativo completo contendo o Salário Bruto, os descontos aplicados e o valor Líquido final.

---

## 💻 Como Executar os Projetos

### Pré-requisitos
* Ter o [.NET SDK](https://dotnet.microsoft.com/download) instalado em sua máquina.
* Um editor de código (como o [Visual Studio Code](https://code.visualstudio.com/) ou o [Visual Studio](https://visualstudio.microsoft.com/)).

### Passo a Passo

1. **Clone este repositório:**
   ```bash
   git clone [https://github.com/luf3ds/C-codes.git](https://github.com/luf3ds/C-codes.git)