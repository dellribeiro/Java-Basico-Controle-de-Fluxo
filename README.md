# Java básico - Controle de Fluxo

Este projeto é um exercício de programação que visa praticar o controle de fluxo utilizando estruturas de repetição. O programa recebe dois números inteiros como parâmetros e realiza a contagem dos números incrementados a partir do primeiro parâmetro até o segundo parâmetro.

## Executando o Programa

**Observação: Certifique-se de ter o Java instalado em seu sistema para executar o programa.**

Para executar o programa, siga as instruções abaixo:

1. Abra o terminal ou prompt de comando.

2. Navegue até o diretório `src` do projeto.

3. Compile os arquivos Java executando o seguinte comando:

   ```shell
   javac ParametrosInvalidosException.java Contador.java
   ```

4. Execute o programa com o seguinte comando:

   ```
   java Contador
   ```

5. O programa é executado via terminal e requer a inserção de dois números inteiros pelo usuário.

6. Digite os valores solicitados e pressione ENTER para avançar para o próximo campo.

7. Após fornecer todas as informações, o programa exibirá uma mensagem mais ou menos assim:

   ```
   Digite o primeiro parâmetro
   > 12
   
   Digite o segundo parâmetro
   > 30
   
   imprimindo o numero 1
   imprimindo o numero 2
   imprimindo o numero 3
   imprimindo o numero 4
   imprimindo o numero 5
   imprimindo o numero 6
   imprimindo o numero 7
   imprimindo o numero 8
   imprimindo o numero 9
   imprimindo o numero 10
   imprimindo o numero 11
   imprimindo o numero 12
   imprimindo o numero 13
   imprimindo o numero 14
   imprimindo o numero 15
   imprimindo o numero 16
   imprimindo o numero 17
   imprimindo o numero 18
   ```

Após inserir os parâmetros, o programa realizará as seguintes ações:

- Verificará se o primeiro parâmetro é maior que o segundo parâmetro.

- Caso seja, lançará a exceção `ParametrosInvalidosException` com a mensagem: "O segundo parâmetro deve ser maior que o primeiro" assim:

  ```
  Digite o primeiro parâmetro
  > 30
  Digite o segundo parâmetro
  > 12
  O segundo parâmetro deve ser maior que o primeiro
  ParametrosInvalidosException
          at Contador.contar(Contador.java:24)
          at Contador.main(Contador.java:15)
  ```

- Caso contrário, chamará o método `contar(parametroUm, parametroDois)` para realizar a contagem dos números e exibir no console.

## Exceção Personalizada

No caso de o segundo parâmetro ser menor ou igual ao primeiro parâmetro, o programa lançará a exceção `ParametrosInvalidosException`. Essa exceção foi criada para representar uma situação de erro nos parâmetros do sistema.

A classe `ParametrosInvalidosException` foi implementada dentro do projeto e é utilizada para lançar a exceção personalizada.