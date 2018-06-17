# trabalhoPOO

## Construtor 
Um construtor é basicamente o responsável por criar objetos de uma classe. Sempre tem o mesmo nome da classe e não tem nenhum tipo de retorno.

Ex:

```java 
public class animal {
  public String raça; 
  public animal (String raça) { 
    this.raça = raça; 
  }

} 
```

## Palavra reservada new

É a palavra chave utilizada para invocar o construtor

Ex:

```java
public class ex {
	
	public static void main (String[] args) {
		animal m = new animal("macaco");
		m.setraça("homo");
		System.out.println(m.getraça());
		
		
	}

}
```

## Palavra reservada instanciof

É a palavra chave utilizada para verifcar se um objeto é uma instancia de uma classe, ou seja se esse objeto foi criado a partit dessa classe

Ex:

```java
public boolean equals(Object object){
		boolean b = false;
		if(object instanceof Ponto){
			Ponto q = (Ponto) object;
			b = x == q.getX() && y == q.getY();
		}
		return b;
	}
```

## Encapsulamento

É um tipo de tecnica que possibilita "esconder" atributos auxiliando dessa forma na proteção dos

Ex: 

``` java 		
m.setraça("homo");
```

## Palavra reservada this

É utilizada para meios de diferenciação entre métodos e nome de parametros

Ex:

```java
public void setraça(String raça) {
		this.raça = raça;
	}
```

## Getters/Setters

O getter é utilizado para buscar alguma informação sem ter que invocar o atributo, normalmente é utilizado junto com o encapsulamento

Ex:

```java
public String getraça() {
		return raça;
		
	}
```

O setter é utilizado para para setar alguma informação ao atributo ou variável em questão

Ex:

```java
public void setraça(String raça) {
		this.raça = raça;
	}
```

## Palavra reservada public/private

A palavra chave public serve para idenbtificar a visibilidade da classe, objeto ou método como publico ou seja que pode ser visualizado e alterada por todos

Ex:

```java
public double peso;
```

A palavra chave private tem como função identificar a visibilidade da classe, objeto ou método como privado, nesse caso sópodem ser visualizados ou aletrados por métodos especificos aplicando assim a técnica de encapsulamento

Ex:

```java
private String raça;
```

## Assinatura de método

Faz parte da assinatura de método a visibilidade do mesmo, nome, argumentos, quantidades de argumentos

Ex:

```java
public void setraça(String raça) {
		this.raça = raça;
	}
```

## Sobrecarga de método
