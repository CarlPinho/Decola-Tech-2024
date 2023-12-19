# Decola-Tech-2024
Repositório para organização de estudos.




# Sintaxe e Tipos de Dados em c#

## O conceito de classe

### O que é uma classe?

Uma classe ela esta relacionada com o conceito de abstração na programação orientada ao objeto

-Uma abstração é um objeto do mundo real e transformá-lo em programação para que você possa trabalhar com ele e implementar suas ações.

#Você só precisa abstrair o que for usar e o que for necessário.


Exemplo:

Classe do tipo pessoa:

          Pessoa                             

   "Atributos"
+ Nome: string
+ Idade: int

   "Métodos"
+ Apresentar() 



### O que é um método?

Um método é uma ação que sua classe irá executar.

Quando você representa uma classe, ela sempre terá seus atributos seguidos de seus métodos.


Exemplo: + Apresentar()

## Objeto Pessoa

String Name = "Bob";



Para que o meu objeto execute uma ação é preciso representar uma AÇÃO na minha classe "Classe Pessoa"


-Então uma classe é como se fosse um molde.


## Exemplos em códigos

### Classe

- using System;

public class Pessoa
{
   
    // Atributos da classe
    public string Nome { get; set; }
    public int Idade { get; set; }

    // Construtor da classe
    public Pessoa(string nome, int idade)
    {
        Nome = nome;
        Idade = idade;
    }

    // Método da classe
    public void Apresentar()
    {
        Console.WriteLine($"Olá, meu nome é {Nome} e tenho {Idade} anos.");
    }
}

class Program
{
    
    static void Main()
    {
        // Exemplo de utilização da classe
        Pessoa pessoa1 = new Pessoa("João", 25);
        pessoa1.Apresentar();

        Pessoa pessoa2 = new Pessoa("Maria", 30);
        pessoa2.Apresentar();
    }
}
