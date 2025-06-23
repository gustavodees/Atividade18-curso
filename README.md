# Loop de Entrada com Condição de Parada

Este é um programa Java simples que solicita ao usuário que digite um valor inteiro repetidamente até que o valor 0 seja inserido. Ele utiliza a biblioteca Swing para exibir janelas de diálogo para interação com o usuário.

## Descrição

O programa inicia pedindo ao usuário para digitar um valor inteiro. Em seguida, ele entra em um loop contínuo. Dentro desse loop, o programa solicita novamente ao usuário que digite outro valor inteiro. O loop continua a se repetir até que o usuário digite o número 0. Quando o usuário insere 0, o loop é encerrado e o programa termina sua execução.

## Como Executar

Para executar este código, você precisará ter o Java Development Kit (JDK) instalado em seu sistema. Siga os passos abaixo:

1.  **Salve o código:** Salve o código Java fornecido em um arquivo chamado `Main.java` dentro de uma pasta chamada `principal`. Certifique-se de que a estrutura de pastas seja `principal/Main.java`.
2.  **Compile o código:** Abra um terminal ou prompt de comando, navegue até a pasta onde você salvou o arquivo `principal` e execute o seguinte comando para compilar o código:

    ```bash
    javac principal/Main.java
    ```

    Isso criará um arquivo chamado `Main.class` dentro da pasta `principal`.

3.  **Execute o programa:** No mesmo terminal ou prompt de comando, execute o programa com o seguinte comando:

    ```bash
    java principal.Main
    ```

    Uma janela de diálogo aparecerá solicitando a entrada do primeiro valor.

## Como Usar

1.  Ao executar o programa, uma janela de diálogo será exibida com a mensagem "Digite o primeiro valor:".
2.  Digite um número inteiro qualquer e clique em "OK".
3.  Uma nova janela de diálogo aparecerá com a mesma mensagem. Continue digitando diferentes números inteiros e clicando em "OK".
4.  O programa continuará a exibir a janela de diálogo solicitando um valor até que você digite o número 0 e clique em "OK".
5.  Quando você digitar 0, o loop será encerrado e o programa terminará sua execução.

## Explicação do Código

* `package principal;`: Declara o pacote ao qual a classe `Main` pertence.
* `import javax.swing.*;`: Importa a biblioteca Swing, que fornece classes para criar interfaces gráficas, como janelas de diálogo.
* `public class Main { ... }`: Define a classe principal do programa.
* `public static void main(String[] args) { ... }`: O método principal onde a execução do programa começa.
* `int x = Integer.parseInt(JOptionPane.showInputDialog("Digite o primeiro valor:"));`: Exibe uma janela de diálogo para obter a primeira entrada do usuário e converte a entrada para um número inteiro, armazenando-o na variável `x`.
* `while(x != 0){ ... }`: Inicia um loop `while` que continuará a executar o código dentro de suas chaves enquanto a condição `x != 0` for verdadeira (ou seja, enquanto o valor de `x` for diferente de 0).
* `x = Integer.parseInt(JOptionPane.showInputDialog("Digite o primeiro valor:"));`: Dentro do loop, esta linha exibe novamente a janela de diálogo, permitindo que o usuário digite um novo valor. Esse novo valor sobrescreve o valor anterior da variável `x`. O loop continuará até que o usuário digite 0, fazendo com que a condição `x != 0` se torne falsa e o loop termine.
