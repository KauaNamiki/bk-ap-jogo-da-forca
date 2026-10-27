# 🕹️ Jogo da Forca em C# (Console)

Projeto desenvolvido em **C#** para console, criado com o objetivo de consolidar conceitos fundamentais de lógica de programação, manipulação de vetores, estruturas de repetição e tratamento de coleções dinâmicas.

---

## 🚀 Tecnologias Utilizadas

* **Linguagem:** C# (.NET)
* **Ambiente:** Console Application (CLI)

---

## ⚙️ Funcionalidades

O jogo seleciona aleatoriamente uma palavra de um tema predefinido e desafia o usuário a adivinhá-la letra por letra:

1. **Sorteio Aleatório:** Utiliza a classe `Random` para escolher de forma randômica uma palavra secreta de um array pré-carregado.
2. **Máscara Dinâmica:** Exibe o progresso do usuário através de um vetor de caracteres (`_`) que são revelados à medida que o jogador acerta os palpites.
3. **Controle de Tentativas:** Gerencia o número máximo de erros permitidos (5 tentativas) e mantém um histórico visível de letras incorretas já digitadas.
4. **Validação de Entrada:** Impede que o usuário perca tentativas ao repetir uma letra já testada e converte automaticamente a entrada para letras maiúsculas para manter a consistência.

---

## 🛠️ Arquitetura e Decisões de Código

O código foi construído dentro do método `Main` utilizando boas práticas de manipulação de fluxo e estruturas de dados:

* **Manipulação de Arrays e Strings:** Conversão de strings para vetores de caracteres (`ToCharArray()`) e uso do método `SequenceEqual` para verificar se o estado atual da forca corresponde à palavra secreta.
* **Coleções (`List<char>`):** Utilização de listas dinâmicas para armazenar e rastrear as letras erradas inseridas pelo usuário durante a execução.
* **Laço de Jogo (`while`):** O fluxo principal roda condicionado a duas regras de parada: o esgotamento das tentativas ou a vitória por completo preenchimento da palavra.

---

## 📦 Como Executar o Projeto

Certifique-se de ter o [.NET SDK](https://dotnet.microsoft.com/) instalado em sua máquina.

1. Clone o repositório:
   ```bash
   git clone <URL-DO-SEU-REPOSITORIO> 
