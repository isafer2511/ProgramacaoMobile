# Relatório – Desenvolvimento do App "Amigo Roubado" (App Inventor)

## Centro Paula Souza
Etec Vasco Antonio Venchiarutti - Jundiaí SP

## Curso
Técnico em Desenvolvimento de Sistemas Integrado ao Ensino Médio

## Turma
2ºC1

## Autores
Henrique Silvestre Martin e Isabella Fernanda da Silva Barbosa

---

# Resumo

Este trabalho apresenta o desenvolvimento do aplicativo móvel do jogo "Amigo Roubado" (também conhecido como Amigo Oculto Ladrão), construído na plataforma App Inventor. O objetivo do projeto é digitalizar a dinâmica tradicional da brincadeira, automatizando o sorteio e as regras de troca de presentes. A metodologia adotada fundamentou-se na programação em blocos e no design centrado no usuário, priorizando uma interface intuitiva e acessível. 
### Palavras-chave: 
App Inventor. Amigo Roubado. Aplicativo Móvel. Programação em Blocos.

---

# Descrição e Funcionamento

Ao ser acessado na tela 1, possui uma tela que apresenta as opções de navegação por meio de botões. Essa tela apresenta as seções do aplicativo, que incluem:

* Iniciar: Abre a tela de configuração do jogo, que defini a turma principal (turma 1) previamente cadastrada e, se desejado pelo usuário, a turma secundária (turma 2), além da quantidade total de alunos. Após a configuração, inicia-se o sorteio dos participantes e situações.
*	Turmas cadastradas: Tela de cadastro das turmas, que permite a criação das turmas com um nome e uma quantidade de alunos, dispondo-as em uma lista as quais podem ser mantidas como opção para o jogo ou excluídas.
*	Tutorial: O passo a passo com imagens para o funcionamento do aplicativo, o qual ao fim direciona o usuário ao início do jogo.
*	Sobre: Informações sobre o trabalho acadêmico e os desenvolvedores.

A tela “Turmas Cadastradas” apresenta uma estrutura composta pelas turmas cadastradas. Ao interagir via clique com uma turma específica, o sistema abre uma caixa que permite o usuário excluir a turma ao confirmar na opção “Sim”. A opção “+ nova turma” redireciona o usuário à tela “Cadastrar Turma”. 

A tela “Cadastrar turma” apresenta as informações necessárias para criação de uma turma — o nome e a quantidade de alunos digitada apenas em números. Após isso, a turma é criada e o usuário redirecionado a tela anterior da disposição das turmas cadastradas. 

A tela “Configuração” é um requisito para o início do sorteio, já que define a quantidade de participantes. O funcionamento lógico desta tela impõe a seleção de uma turma principal que deve ser previamente cadastrada e, por meio de uma caixa de seleção, a escolha de convidar outra turma para participar. Ao fim desse processo, é exibida a quantidade total de participantes — com uma ou duas turmas — e o usuário pode prosseguir para o início do jogo. uma restrição de concorrência: o sistema permite a exibição do resumo de apenas um conflito por vez.

A tela “Sorteio” tem como principal função gerenciar a escolha aleatória dos participantes e determinar a ação/situação que cada um deve executar durante a brincadeira. Ao abrir a tela, o aplicativo permite o sorteio dos participantes, apresentando a turma que o sorteado pertence. Após isso, o usuário pode sortear uma situação: 

1.	Opção 1: "Pode trocar o presente com outro participante!"
2.	Opção 2: "Pode trocar o presente no saco preto!"
3.	Opção 3: "Fique com seu presente!"
4.	Opção 4: "Devolva seu presente no saco preto!"
   
Caso todos os números da lista já tenham sido sorteados, o sistema exibe um alerta informando que não há mais participantes disponíveis e redirecionando o usuário à tela “Fim do Jogo”.

A tela “Tutorial” possui um guia com 6 passos essenciais para o funcionamento do jogo, indicando com uma lista cada item desde o cadastro dos jogos até o encerramento do sorteio com um pequeno texto explicativo e imagens.

A tela “Sobre” apresenta um texto que brevemente explica o trabalho acadêmico, qual a matéria que foi desenvolvida no projeto além da data de finalização e o nome e turma dos participantes.

A tela “Fim do Jogo” possui uma imagem sobre a finalização do sorteio e permite que o usuário inicie um novo jogo.

Vale ressaltar ainda que cada tela possui um botão no canto inferior direito, que permite o usuário voltar à tela anteriormente acessada.

---

# Componentes e Conceitos Aplicados

Para o desenvolvimento do projeto foi fundamento em alguns conceitos apresentados em sala de aula, sendo eles:

*	Eventos (clique de botão, envio de resposta, seleção em lista e disparo de temporizadores),
*	Manipulação de telas (troca entre screens),
*	Design eficiente e agradável (uso de arrangements, além da personalização visual através de cores de fundo, imagens e fontes),
*	Manipulação de estruturas de dados (criação e gerenciamento de listas dinâmicas para controle dos participantes disponíveis),
*	Uso de variáveis globais e locais (armazenamento de dados temporários na memória),
*	Estruturas condicionais (validação de regras do jogo por if e else if),
*	Laços de repetição (preenchimento automático da lista de números de 1 até o número total de alunos por exemplo, com for each),
*	Lógica matemática (operações matemáticas e random integer).

A implementação prática dos componentes utilizados fundamenta-se nos itens a seguir:

*	TextBox: entrada de respostas do usuário;
*	CheckBox: seleção pelo usuário;
*	Button: envio de respostas e navegação;
*	Label: exibição de resultados;
*	Image: imagens do sorteio;
*	Arrangements: incluindo o Scroll Arrangement, permitindo melhor organização dos componentes;
*	Notifier: mensagens importantes no jogo, como a finalização do sorteio;
*	Clock: armazenamento do sorteio de participantes e situações;
*	TinyDB: armazenamento de informações entre as telas do jogo;
*	ListPicker: seleção de itens a partir de uma lista suspensa de turmas cadastradas;
*	Sound / Player: execução de efeitos sonoros durante o giro das roletas e áudios do jogo;
*	Screens: organização do app em múltiplas telas.
  
## Da Lógica de Programação – Funcionamento da Configuração e Sorteio

1.	Carregamento dos Dados
Na inicialização da tela de configuração, o aplicativo busca no banco de dados local (TinyDB) a lista de turmas cadastradas com seus respetivos nomes e quantidades de alunos. Os componentes ListPicker são preenchidos com os nomes das turmas para permitir a seleção pelo usuário. 

2.	Seleção e Cálculo do Total de Participantes
O usuário deve escolher a primeira turma (ListPicker1) e, opcionalmente, marcar uma caixa de seleção (CheckBox1) para incluir uma segunda turma (ListPicker2). O procedimento “calcularTotal” identifica o número de alunos de cada turma selecionada através do seu índice na lista. A quantidade da Turma 1 “qtd1” e a quantidade da Turma 2 “qtd2” são somadas para determinar o “totalAlunos”. 

3.	Armazenamento e Transição 
Ao confirmar no botão de iniciar, o sistema salva no TinyDB o “totalAlunos” e o limite de alunos da primeira turma “qtdTurmaA”, redirecionando o usuário para a tela de Sorteio.

4.	A Tela de Sorteio
Na abertura da tela de Sorteio, o sistema recupera o valor de “totalAlunos” e o valor limite “qtdTurmaA” armazenados no TinyDB, criando uma lista global (numerosDisponiveis) preenchida sequencialmente de 1 até o total geral de alunos (exemplo: de 1 a 50). 
Ao clicar no botão de sortear (Btn_sortearnum), o aplicativo gera um índice aleatório (random integer) baseado na quantidade de itens restantes na lista “numerosDisponiveis”. O número sorteado é selecionado, armazenado em “numSorteado” e removido da lista para que a mesma pessoa seja sorteada duas vezes. Um temporizador (Clock1) faz o efeito visual de giro da roleta exibindo números temporários até a parada final. 
Quando a roleta para, o sistema compara o “numSorteado” com o valor limite “qtdTurmaA”: se o número for menor ou igual a “qtdTurmaA” o sistema identifica que o aluno pertence à primeira turma e exibe diretamente o resultado como Turma 1; se o número for maior que “qtdTurmaA” o sistema realiza uma conversão matemática subtraindo o valor de “qtdTurmaA” do “numSorteado” (exemplo: 35 - 30 = 5), exibindo o resultado como Turma 2.
Em seguida, o botão de sortear situação escolhe aleatoriamente um número de 1 a 4. O temporizador (Clock2) faz a animação da situação e exibe a instrução correspondente ao número sorteado (como "Fique com seu presente!" ou "Pode trocar o presente no saco preto!"), além de alterar a imagem ilustrativa da tela. 
