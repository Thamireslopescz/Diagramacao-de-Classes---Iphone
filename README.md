Projeto iPhone Multiuso
Este projeto consiste em um exemplo simples de modelagem de classes e interfaces em Java para representar as funcionalidades de um iPhone em diferentes contextos: Reprodutor Musical, Aparelho Telefônico e Navegador na Internet. Cada funcionalidade é representada por uma interface específica, e a classe IPhone implementa todas essas interfaces para demonstrar a versatilidade do dispositivo.

Funcionalidades
Reprodutor Musical
A funcionalidade de Reprodutor Musical é implementada pela interface ReprodutorMusical, que define métodos para reproduzir, pausar, avançar e retroceder músicas.

Aparelho Telefônico
A funcionalidade de Aparelho Telefônico é representada pela interface AparelhoTelefonico, que define métodos para fazer chamadas, receber chamadas e encerrar chamadas.

Navegador na Internet
A funcionalidade de Navegador na Internet é definida pela interface NavegadorInternet, que define métodos para abrir URLs, fechar URLs e realizar buscas na internet.

Diagrama de Classes
A seguir está o diagrama de classes que representa a estrutura das interfaces e da classe IPhone:

Diagrama de Classes

O diagrama de classes acima ilustra as relações entre as interfaces e a classe IPhone. Cada interface representa uma funcionalidade específica do iPhone, e a classe IPhone implementa todas essas interfaces para criar um dispositivo multifuncional.

Implementações em Java
Abaixo estão as implementações das interfaces e da classe IPhone em arquivos .java:

ReprodutorMusical.java

java
Copy code
interface ReprodutorMusical {
    void reproduzirMusica();
    void pausarMusica();
    void avancarMusica();
    void retrocederMusica();
}
AparelhoTelefonico.java

java
Copy code
interface AparelhoTelefonico {
    void fazerChamada(String numero);
    void receberChamada(String numero);
    void encerrarChamada();
}
NavegadorInternet.java

java
Copy code
interface NavegadorInternet {
    void abrirURL(String url);
    void fecharURL();
    void realizarBusca(String termo);
}
IPhone.java

java
Copy code
class IPhone implements ReprodutorMusical, AparelhoTelefonico, NavegadorInternet {
    // Implementações dos métodos das interfaces...

    // ...
}
Uso
O exemplo de uso do iPhone pode ser encontrado no método main da classe Main:

Main.java

java
Copy code
public class Main {
    public static void main(String[] args) {
        IPhone iphone = new IPhone();
        iphone.reproduzirMusica();
        iphone.fazerChamada("123456789");
        iphone.abrirURL("https://www.example.com");
    }
}
