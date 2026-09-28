# Relatório – Desenvolvimento de Aplicativos (App Inventor)

## Centro Paula Souza
Etec Vasco Antonio Venchiarutti - Jundiaí SP

## Curso
Técnico em Desenvolvimento de Sistemas Integrado ao Ensino Médio

## Turma
2ºC1

## Autores
Henrique Silvestre Martin e Isabella Fernanda da Silva Barbosa

---

# Projeto 1 – ACELERÔMETRO

## Funcionamento
O aplicativo funciona como um leitor sensorial focado em capturar os movimentos físicos do dispositivo através de seus eixos tridimensionais. Assim que o aplicativo é iniciado, ele ativa o sensor de acelerômetro integrado para monitorar constantemente as forças exercidas sobre o aparelho. Ao interagir com o sistema, o usuário inclina ou chacoalha o aparelho para modificar os dados capturados, atualizando dessa maneira os rótulos de texto na tela que indicam os valores dos eixos X, Y e Z em tempo real, alterando também a posição de uma imagem gráfica com base na inclinação. Nesse momento, o aplicativo compara o comportamento do sensor e, caso detecte um movimento de agitação, ele altera aleatoriamente a cor de fundo do aplicativo. 

### Componentes utilizados
A implementação prática dos componentes utilizados fundamenta-se nos itens a seguir:

*	AccelerometerSensor: capturar a aceleração e movimento do celular nos eixos X, Y e Z;
*	Canvas: espaço gráfico para projetar e limitar a área de movimentação dos elementos;
*	ImageSprite: componente gráfico cujas coordenadas são alteradas conforme a inclinação do dispositivo; 
*	Label: exibição em forma de texto dos valores numéricos das coordenadas;
*	Screen: componente principal configurado para alterar aleatoriamente sua cor de fundo ao detectar o gesto de chacoalhar.

---

# Projeto 2 – MAGIC BALL COM ACELERÔMETRO

## Descrição
O aplicativo funciona como um jogo de equilíbrio focado em conduzir uma bolinha para um buraco. Assim que o aplicativo é iniciado, ele posiciona uma bolinha preta e um buraco, definindo o tempo (60 segundos) e a quantidade de bolas restantes na partida (20). Ao interagir com o sistema, o usuário deve inclinar fisicamente o aparelho para os lados para direcionar a trajetória da bolinha, a deslocando. Nesse momento, o aplicativo monitora as coordenadas e, caso a bolinha colida com a área demarcada do buraco, identifica que a jogada foi bem-sucedida, reproduzindo automaticamente um efeito sonoro de pontuação, além de reduzir a quantidade de bolas restantes e reinicia a posição do objeto no cenário para dar continuidade ao jogo. Caso o tempo se esgote, o jogo reinicia para que o usuário tente acertar as 20 tentativas.

### Componentes utilizados
A implementação prática dos componentes utilizados fundamenta-se nos itens a seguir:

*	AccelerometerSensor: leitura da inclinação do aparelho;
*	Canvas: área de interações com uma imagem de fundo de mesa de madeira;
*	ImageSprite: representação da bolinha preta principal;
*	Ball: componente esférico que simula um buraco;
*	Label: exibição do tempo de jogo decorrido e da quantidade de bolinhas restantes;
*	Arrangements: organização dos textos;
*	Sound: reprodução do efeito sonoro da colisão da bolinha com o buraco.

---

# Projeto 3 – ADIVINHA NÚMERO

## Descrição
O aplicativo funciona como um teste de perguntas e respostas focado em operações aritméticas. Assim que o aplicativo é iniciado, ele executa um procedimento automático que sorteia dois valores numéricos inteiros aleatórios (variando de 1 a 999) e escolhe uma operação matemática entre adição, subtração ou multiplicação. Caso a operação escolhida seja a subtração, o sistema faz uma verificação inteligente para identificar qual dos dois números é o maior, garantindo que o cálculo seja estruturado de forma a não gerar um resultado negativo. Com a conta definida, o aplicativo exibe os números e o sinal correspondente na tela para o usuário, que deve digitar a resposta do cálculo do campo de texto e verificar o resultado. Nesse momento, o aplicativo compara o valor digitado pelo usuário com o resultado real da conta armazenado internamente e adiciona aos acertos caso esteja correto ou aos erros caso esteja incorreto. Além disso, automaticamente reinicia o sorteio de uma conta matemática. 

### Componentes utilizados
A implementação prática dos componentes utilizados fundamenta-se nos itens a seguir:

*	TextBox: entrada de dados para que o usuário digite as respostas dos cálculos;
*	Button: acionamento do comando para verificar o resultado digitado;
*	Label: exibição dos números sorteados, dos operadores matemáticos e do placar de acertos e erros;
*	Arrangements: estruturação visual dos campos de texto e dos botões.

---

# Projeto 4 – DADO MÁGICO

## Descrição
O aplicativo funciona como um simulador digital de sorteio de um dado. Ao clicar no botão de “sortear”, o sistema gera um número aleatório entre 1 a 6 para definir a face do dado, que será exibida tanto em forma de texto quanto de forma visual na imagem – o sistema relaciona o número aleatório escolhido com sua imagem correspondente –, além de executar uma vibração de 100 milissegundos. Vale ressaltar que foram utilizadas imagens autorais, já que o tutorial não forneceu os recursos visuais.

### Componentes visuais
A implementação prática dos componentes utilizados fundamenta-se nos itens a seguir:

*	Button: comando com cantos arredondados para disparar o sorteio;
*	Label: exibição textual do número sorteado e do título do aplicativo;
*	Image: renderização das faces do dado correspondentes ao número gerado;
*	AccelerometerSensor / Sound: ativação da vibração do dispositivo.

---

# Projeto 5 – BILHAR

## Descrição
O aplicativo funciona como um simulador eletrônico de jogo de bilhar, focado em movimentar e encaçapar uma bolinha em uma mesa virtual. Assim que o aplicativo é iniciado, ele executa um procedimento automático de inicialização que posiciona os elementos na tela e ao interagir com a tela, o sistema monitora o comportamento da bolinha principal e aplica um efeito dinâmico de gravidade virtual, garantindo que o movimento perca um pouco de velocidade. O sistema faz uma verificação da colisão tanto nas bordas quanto nas caçapas mapeadas: caso a bolinha atinja as tabelas laterais, ela rebate e continua em jogo; porém, caso ocorra uma colisão direta com uma das seis caçapas pretas posicionadas nos cantos, o jogo identifica que a jogada foi bem-sucedida, reproduz instantaneamente um efeito sonoro e reposiciona a bolinha de volta ao centro da mesa. 

### Componentes utilizados
A implementação prática dos componentes utilizados fundamenta-se nos itens a seguir:

*	Canvas: representação digital da mesa de bilhar e gerenciamento do espaço;
*	Ball: simulação tanto da bolinha principal quanto das seis caçapas posicionadas nos cantos;
*	Label: exibição de orientações textuais ou dados sobre o estado do jogo;
*	Arrangements: alinhamento centralizado dos componentes visuais na tela;
*	Sound: execução do efeito sonoro;
*	Clock: controle do efeito de gravidade e desaceleração da bola.

---

# Projeto 6 – JOGO DA CHUVA

## Descrição
O aplicativo funciona como um jogo interativo de esquiva e coleta de elementos digitais. Assim que o aplicativo é iniciado, ele executa um procedimento automático de inicialização que renderiza um cenário com fundo de céu e posiciona um personagem controlável na parte inferior da tela. Ao interagir com o sistema, o usuário arrasta o dedo horizontalmente para movimentar o personagem de um lado para o outro, sendo que o sistema faz uma verificação para fazer com que gotas de chuva caiam continuamente do topo em posições aleatórias. Nesse momento, o aplicativo monitora constantemente as coordenadas na tela e, caso a gota colida com o personagem, adiciona pontos ao placar do usuário e reposiciona o elemento no topo para reiniciar a queda. Além disso, se o sistema identificar que a gota atingiu o limite do chão sem ser coletada, ela é automaticamente reiniciada no topo da tela sem penalidades visíveis, mantendo o fluxo dinâmico e contínuo. 

### Componentes utilizados
A implementação prática dos componentes utilizados fundamenta-se nos itens a seguir:

*	Canvas: cenário gráfico com o espaço do jogo;
*	ImageSprite: representação visual tanto do personagem quanto das gotas de chuva;
*	Label: exibição do placar com a pontuação atual do jogador;
*	Clock: controle de tempo responsável por gerenciar a velocidade da queda das gotas e a frequência com que novos elementos surgem. 
