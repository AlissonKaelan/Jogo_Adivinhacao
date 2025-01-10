# Jogo_Adivinhacao
 Este projeto é uma aplicação Java Swing que implementa um jogo de adivinhação. O usuário tenta adivinhar um número aleatório entre 1 e 5. A interface exibe o resultado do palpite, contabilizando os acertos e erros do jogador.

 Funcionalidades
Geração de Número Aleatório:
O jogo gera um número aleatório entre 1 e 5 sempre que o botão "Palpite" é pressionado.

Entrada de Dados pelo Usuário:
O jogador seleciona um número utilizando um componente JSpinner.

Avaliação de Resposta:
O programa compara o número gerado com o número escolhido pelo usuário e exibe:

Mensagem de "Acertou!" se o número estiver correto.
Mensagem de "Errou!" informando o número correto em caso de erro.
Contadores de Acertos e Erros:
Os acertos e erros são registrados e exibidos em tempo real na interface.

Interface Responsiva:
O painel com os contadores de acertos e erros é exibido apenas após o primeiro palpite.

Componentes da Interface Gráfica
JLabel:

jLabel2: Exibe o título "Adivinhe o Número de 0 a 5".
lblFrase: Mostra mensagens de acerto ou erro.
lblA: Exibe o número total de acertos.
lblE: Exibe o número total de erros.
JSpinner:

txtval: Permite ao jogador selecionar um número entre 1 e 5.
JButton:

btnP: Botão para registrar o palpite do jogador.
JPanel:

Panel1: Contém os rótulos e valores dos contadores de acertos e erros.
Lógica do Jogo
Fluxo de Execução:
O botão "Palpite" (btnP) é pressionado.
Um número aleatório é gerado pelo método Math.random().
O valor selecionado pelo jogador é recuperado do JSpinner.
É realizada a comparação entre o número gerado e o selecionado:
Se forem iguais, a mensagem "Acertou!" é exibida, e o contador de acertos é incrementado.
Caso contrário, a mensagem "Errou!" é exibida, junto com o número correto, e o contador de erros é incrementado.
Os valores dos contadores são atualizados nos rótulos lblA e lblE.
O painel com os contadores é exibido após o primeiro palpite.
Estrutura do Código
Variáveis Globais
nA (int): Contador de acertos.
nE (int): Contador de erros.
Métodos Principais
Construtor ViewSwing: Inicializa os componentes e define o painel Panel1 como invisível no início.

btnPActionPerformed: Método chamado ao pressionar o botão "Palpite". Responsável pela lógica do jogo e atualização da interface.

main: Método principal que inicializa e exibe a janela do jogo.
