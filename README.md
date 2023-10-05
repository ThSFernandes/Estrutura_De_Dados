<h1 align="center"> Estudo Estrutura de Dados<h1>

#### Estudos Referente ao dia 
05/10/2023

  
### Visibilidade de Métodos e Modificadores de Classes:
No mundo da programação Java, a visibilidade dos métodos e as classes podem ser compreendidas através de modificadores. Os modificadores de classes são palavras reservadas opcionais que antecedem o modificador "public". Vamos destacar alguns deles:

- Abstract: Esse modificador indica que a classe é uma classe abstrata, que não pode ser instanciada diretamente e geralmente contém métodos abstratos, cujas implementações são fornecidas por subclasses.

- Final: Uma classe marcada como final não pode ser estendida, ou seja, não pode ter subclasses.

- Public: Indica que a classe é visível e acessível a qualquer coisa definida no mesmo pacote ou a qualquer coisa que importe essa classe.

### Objetos e Criação de Instâncias:

Para criar um objeto em Java, usamos o operador "new". Ele aloca dinamicamente memória para o novo objeto e inicializa todas as variáveis de instância com seus valores padrão. O operador "new" também chama um construtor específico, se houver, para inicializar o objeto.

É importante destacar que em Java, o valor padrão para variáveis de objeto é null para objetos, 0 para tipos numéricos e false por padrão para tipos booleanos.

### Variáveis de Referência:

Uma variável de referência é usada para acessar os membros de uma classe à qual pertence um objeto, a instância da classe. Isso permite acessar os métodos e variáveis de instância da classe usando o operador "." (ponto).

### Assinatura de Método:

A assinatura de um método é composta pelo nome do método combinado com a quantidade e tipos de seus parâmetros. Por exemplo:

```
oven.cookDinner();
oven.cookDinner(food);
oven.cookDinner(food, seasoning);
```
### Modificadores de Variáveis:

Em Java, variáveis podem ter modificadores que afetam sua visibilidade. Alguns deles incluem:

- Public: Qualquer um pode acessar variáveis de instância públicas.

- Protected: Apenas métodos do mesmo pacote ou subclasses podem acessar variáveis de instância protegidas.

- Private: Apenas métodos da mesma classe (excluindo métodos de subclasses) podem acessar variáveis de instância privadas.

### Métodos e Tipos de Retorno:

Um método permite que o programador envie uma mensagem para um objeto. Os tipos de retorno podem ser "void" se o método não retornar nenhum valor (chamado de procedimento), ou um tipo específico se o método retornar um valor (chamado de função).

Para retornar um valor em Java, usamos a palavra-chave "return". Funções em Java podem retornar apenas um valor, mas para retornar vários valores, podemos combiná-los em um objeto composto cujas variáveis de instância incluam todos os valores desejados e retornar uma referência para esse objeto composto.

- Exemplo abaixo do que já foi visto acima 
```
public class Gnome {
    //variáveis de instância
    public String name;
    public int age;
    public Gnome gnomeBuddy;
    private boolean magical = false;
    protected double height = 2.6;
    public static final int MAX_HEIGHT = 3;
}
Gnome(String nm, int age, Gnome bud, double hgt){// Parâmetros
    name =nm;
    age = ag;
    gnomeBuddy =bud;
    height = ght;
}
Gnome(){
    name = "Otávio";
    age = 23;
    gnomeBuddy = null;
    height = 2.1;
}
public static void makeKing(Gnome h){
    h.name = "King " + h.getRealName();
    h.magical = true //Apenas a classe Gnome pode referenciar este campo; 
}
public void makeMeKing(){
    name = "King " + getRealName();
     magical.true;
}
public boolean isMagical(){
    return magical;
}
public void setHeight(int newHeight){
    height = newHeight;
}
public String getName(){
    return "I wotn't tell";
}
public String getRealName(){
    return name;
}
public void renameGnome(String s ){
    name = s ;
}
```

### Literais e Tipos de Dados:

Em Java, literais são valores constantes que podem ser usados em atribuições ou outras expressões. Alguns tipos de literais incluem:

- Referência para objeto null.

- Booleanos: true ou false.

- Inteiros: Podem ser especificados com sufixos L ou l para indicar longos (64 bits).

- Literais de ponto flutuante: Podem terminar em "F" ou "f" para indicar floats, e notação científica pode ser usada, por exemplo, 3.14E2.

### Operadores e Incremento:

Java possui vários operadores, incluindo operadores de incremento (++, --) que podem ser usados tanto antes quanto depois de uma variável para incrementar ou decrementar seu valor.

### Operadores Lógicos:
Operadores lógicos incluem a negação (!), "e" condicional (&&) e "ou" condicional (||) para avaliar expressões lógicas.
Conversões de Tipo:
Podemos converter um tipo em outro usando castings. 
Por exemplo, (double) 43 converte o valor inteiro 43 em um valor double.

### Comando Switch:

O comando switch é usado para controle de fluxo multivalorado, permitindo que você execute diferentes blocos de código com base em um valor específico, como um número de telefone.

```
public class Switch {
   
    public static void main(String[] args) {
        String d = "e"; // Defina a variável d antes de usá-la
        String mon = "d"; // Atribua o valor "d" a mon
        String tue = "b";
        String wed = "c";
        String thu = "d";
        String frd = "e";
        
        switch (d) {
            case "mon": // Use as strings entre aspas
                System.out.println("Hoje é segunda-feira !");
                break;
            case "tue":
                System.out.println("Hoje é terça-feira !");
                break;
            case "wed":
                System.out.println("Hoje é quarta-feira !");
                break;
            case "thu":
                System.out.println("Hoje é quinta-feira !");
                break;
            case "frd":
                System.out.println("Hoje é sexta-feira !");
                break;
            default:
                System.out.println("Hoje é final de semana !");
        }
    }
}
```
### Referências:
[1] "Estrutura de Dados & Algoritmos em Java."  
Disponível em: https://www.amazon.com.br/Estruturas-Dados-Algoritmos-em-Java/dp/8582600186.
