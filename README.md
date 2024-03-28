# Conta bancária Python
Neste desafio foi criado um programa em Python que simula um sistema básico de caixa eletrônico que emite extratos, realiza saque e depósitos e emite comprovante dos saques e dos depósitos realizados. Os saques são condicionados as regras de negócio. Os extratos trazem as informações das operações realizadas e o saldo disponível para o cliente.

## Descrição de funcionalidade
1. O código define uma variável chamada **menu**, que é uma string multilinha e que apresenta as opções disponíveis para o usuário, incluindo depósito, saque, consulta de extrato e sair do sistema.
2. Em seguida, são definidas algumas variáveis importantes:
   - **Saldo**: Inicia com o valor 0;
   - **Limite**: Definido com o valor 1000;
   - **Extrato**: String iniciada sem valor e utilizada para armazenar as transações do usuário a medida que são executadas;
   - **Numero_saques**: Inicializado como valor 0;
   - **Limite_saques**: Valor constante definido como 3.
3. O programa entra em um loop **while true** que continuará em execução idenfinidamente até que o usuário decida sair do sistema.
4. Dentro do loop, o programa solicita ao usuário que selecione uma das opções do menu e aguarda a entrada do usuário. Para a opção deposito é utilizada a opção **d**, para a opção saque deve selecionar **s**, já para emitir um extrato deve-se selecionar a opção **e** e para finaizar o programa e sair do loop, deve-se selecionar a opçãpo **q**. Após a seleção de uma 
 opção o programa irá executar o bloco de código associado.
5. Para a opção depósito (**d**), o programa solicita ao usuário que insira o valor a ser depósitado. Se o valor for válido (maior que zero), ele é adicionado ao saldo e uma mensagem de comprovante de depósito é exibida.
6. Para a opção de saque(**s**), o programa verifica se o valor do saque excede o saldo disponível, o limite de saque diário ou o limite total de saques. Se não houver divergência em relação a regra de negócio, o valor é subtraído do saldo e uma mensagem de comprovante de saque é exibida.
7. Para a opção de extrato (**e**), o programa exibe todas as transações realizadas pelo usuário e o saldo atual.
8. Se o usuário selecionar a opção (**q**), o programa sai do loop **while** e termina a execução.
9. Se o usuário inserir uma opção inválida, o programa exibe uma mensagem de erro e solicita que o usuário selecione novamente.
