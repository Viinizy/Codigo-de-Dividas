# Controle de Dívidas em Java

Este projeto é um exemplo simples em Java criado para fins de aprendizado.
Ele simula o controle de uma dívida, permitindo adicionar valores e realizar pagamentos.

Site:[ https://github.com/Viinizy/Site-de-Contre-de-Dividas.git](https://viinizy.github.io/Codigo-de-Dividas/)

## 📌 Funcionalidades
- Criar uma dívida com valor inicial
- Adicionar valores à dívida
- Realizar pagamentos
- Consultar o total da dívida

## 💻 Código de exemplo

```java

class divida {
    private double total;
    divida (double valorinicial) {
        this.total = valorinicial;
    }
    void pagar(double valor) {
        total -= valor;
    }  void adicionar(double valor) {
        total += valor;
    }  double getTotal() {
        return total;
    }
} class Main
{ static void main(String[]args){
    divida a = new divida(5000);
System.out.println("divida inicial: " + a.getTotal());
a.pagar(500);
    System.out.println("pago: " + 500);
a.pagar(500);
    System.out.println("pago: " + 500);
    a.adicionar(300);
    System.out.println("aumento: " + 300);
    a.pagar(500);
    System.out.println("pago: " + 500);
    a.adicionar(100);
    System.out.println("aumento: " + 100);
    System.out.println("divida final: " + a.getTotal());
}
}



