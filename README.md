Implementar o jogo chamado "foda-se" ou "fodinha" em uma rede em anel com 4 máquinas:
- Criar uma rede em anel com 4 máquinas usando Socket DGRAM
- O controle de acesso a rede deve ser feito por passagem de bastão
- Todas as mensagens devem dar a volta toda pelo anel
- O bastão não é temporizado
- As mensagens não são temporizadas
- Não é necessário timeout
- Deve ser feito em Python

Em cada mão do jogo:
- Carteador deve sortear as cartas e enviar para cada jogador as suas cartas
- As cartas podem ser enviadas todas em uma mesma mensagem ou uma mensagem para cada jogador
- Depois das cartas, cada jogador deve fazer as suas apostas (uma mensagem da a volta pelo anel completando as apostas)
- Nova mensagem da a volta pelo anel informando e atualizando as apostas de cada jogador na tela
- Depois das apostas, começa-se o jogo. 
- Mensagem da volta pelo anel, cada jogador que recebe a mensagem deve mostrar as cartas já jogadas, decidir qual carta jogar, adicionar carta na mensagem e reenviar a mensagem
- Depois da mensagem dar a volta no anel, o carteador deve computar o resultado da rodada, e enviar o resultado para todos os jogadores
- Depois deve começar a próxima rodada
- Ao terminar as cartas de cada mão. O carteador deve computar o resultado geral e a pontuação de cada jogador. 
- Informar os jogadores sobre a nova pontuação
- Passar o bastão para a frente, para que o próximo jogador seja o carteador
