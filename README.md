# 💳 Simulador de Compras com Cartão de Crédito

> Um programa de console em Java que simula o lançamento de compras em um cartão de crédito com limite pré-definido, exibindo um extrato ordenado no final.

---

## 📚 Sobre o Projeto

Este projeto é uma aplicação de console simples, desenvolvida em Java, para exercitar conceitos de Programação Orientada a Objetos (POO). A aplicação permite ao usuário definir um limite para um cartão de crédito e, em seguida, registrar diversas compras. O sistema valida cada compra contra o saldo disponível e, ao final da operação, exibe um extrato detalhado com todas as compras realizadas, ordenadas por valor, e o saldo remanescente.

---

## ✨ Funcionalidades Principais

* **Definição de Limite:** O usuário informa o limite inicial do cartão de crédito.
* **Registro de Compras:** Permite adicionar múltiplas compras, informando a descrição e o valor de cada uma.
* **Validação de Saldo:** O sistema verifica se o saldo do cartão é suficiente antes de aprovar uma nova compra.
* **Extrato Final:** Ao encerrar, o programa exibe uma lista de todas as compras aprovadas.
* **Ordenação de Compras:** As compras no extrato final são exibidas em ordem crescente de valor.
* **Consulta de Saldo:** Apresenta o saldo final do cartão após todas as operações.

---

## 🛠️ Tecnologias Utilizadas

* [**Java**](https://www.java.com/) (JDK 17 ou superior recomendado)

---

## 🚀 Como Executar o Projeto

Para compilar e executar este projeto localmente, você precisará ter o Java Development Kit (JDK) instalado em sua máquina.

### Pré-requisitos

* [JDK (Java Development Kit)](https://www.oracle.com/java/technologies/downloads/) - Versão 17 ou superior.

### Passos para Execução

1.  Clone o repositório (ou baixe os arquivos para uma pasta):
    ```bash
    git clone [https://github.com/DomCarlosAdriano/Compras.git](https://github.com/DomCarlosAdriano/Compras.git)
    ```

2.  Navegue até a pasta `src` do projeto pelo seu terminal:
    ```bash
    cd Compras/src
    ```

3.  Compile os arquivos `.java`:
    ```bash
    javac Principal.java CartaoDeCredito.java Compra.java
    ```

4.  Execute a classe principal:
    ```bash
    java Principal
    ```

5.  Siga as instruções que aparecerão no terminal para interagir com o programa.

---

## 🏛️ Estrutura do Código

O projeto é organizado em três classes principais, seguindo os princípios da POO:

* `Principal.java`: Contém o método `main`. É a classe responsável por toda a interação com o usuário (entrada de dados) e por orquestrar o fluxo da aplicação.
* `CartaoDeCredito.java`: Modela o cartão de crédito. Gerencia os atributos de limite e saldo, e armazena uma lista de objetos `Compra`.
* `Compra.java`: Modela uma compra individual. Possui atributos como descrição e valor, e implementa a interface `Comparable` para permitir a ordenação da lista de compras.
