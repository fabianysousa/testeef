<h1 align="center"> Entity Framework </h1>

<p align="center">
    <img src="https://ik.imagekit.io/fabianysousa/EF_8m1Qojwka.jpg" width="500" height="300">	
</p>


## 📑 Sobre

Nesse repositório feita a reprodução vídeo [API com ASP.NET Core 3 e EF Core](https://www.youtube.com/watch?v=but7jqjopKM) do canal [balta.io](https://www.youtube.com/watch?v=but7jqjopKM) afim de colocar em prática a utilização do **Entity Framework** e deixar documentado os conceitos básicos da EF aprendidos.

---

## 🧠 Conceitos aprendidos

Para começar é valido ressaltar logo de cara que o *Entity Framework* nasceu no service pack do *.NET framework*, então vale a pena estudar sobre ele e suas vantagens quando se estuda *.NET*.

### 1. Linhas principais de utilização

O EF tem  três metodologias para o desenvolvimento da sua camada de acesso a dados: 

|                  |                          Funcionamento                                |
|------------------|-----------------------------------------------------------------------|
| Database First   | { Banco de Dados existente } --> { Modelo de dados gerado (.edmx) }   |
| Model First      | { Modelo de dados (.edmx) } --> { Banco de dados Gerado }             |
| Code First       | { Classe do domínio } --> { EF } --> { Base de dados }                |
| Code First       | { Banco de dados existente } --> { Modelo de dados (Classes) gerado } |

- **Database First**: Com a base de dados pronta que cria classe para mapear essa base de dados.

- **Model First**: Modelagem do sistema antes da linha de comando.

- **Code First**: Possui diversas ferramentas que permite trabalhar com a base de dados em cima do código da classe.

Na contrução da API desse repositório foi utilizada a linha Code First: { Classe do domínio } --> { EF } --> { Base de dados }.


### 2. Nuget

Em geral a EF é incorporada com a utilização de Nuget que é uma extensão do Visual Studio que facilita a instação e o controle de bibliotecas e ferramentes. Podemos utilizar ele de forma visual ou pelo console. 


A forma visual seria pelo o Visual Studio selecionando:

    Ferramentas > Gerenciador de Pacotes do NuGet > Console do Gerenciador de Pacotes

No caso da API criada nesse repositório um utilizei o seguinte comando da CLI do .NET Core:

```bash
  # comando da CLI do .NET Core
  $ dotnet add package Microsoft.EntityFrameworkCore.SqlServer
```

### 3. Vantagens

Ele da suporte a consultas LINQ, controle de alterações, atualizações e migrações de esquema. Funciona em muitos banco de Dados SQL (local e Azure), o SQLite, o MySQL e o Azure Cosmos DB.

---

## ⚙️ Tecnologias utilizadas

O projeto foi desenvolvido utilizando as seguintes tecnologias:

- [C#](https://docs.microsoft.com/pt-br/dotnet/csharp/)
- [.Net Core](https://github.com/dotnet/aspnetcore)
- [Entity Framework](https://docs.microsoft.com/pt-br/ef/)

---

## ☄️ Como baixar o projeto

No promit command:

```bash

    # Clonar o repositório
    $ git clone https://github.com/fabianysousa/testeef

    # Entrar no diretório
    $ cd testeef
    
    # Baixar a dependencia EF
    $ dotnet add package Microsoft.EntityFrameworkCore.SqlServer 
    
    # Rode o projeto
    $ dotnet run

```
---
## 💡 Insight

Decobri o quanto é vantajoso utilizar o Entity Framework, ele juntamente com o .NET são como companheiros leais. Também não posso deixar de ressaltar a facilidade e inserir esse framework e sua alta abstração o que dá a ele o poder de ter suporte para diversos tipos de banco de dados. Contudo, recomendo a todos o estudo não somente do .NET, mas também do Entity Framework.

---

Desenvolvido ❤️ por Fabiany de Sousa Costa
