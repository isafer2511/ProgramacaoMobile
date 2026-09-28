# Relatório – Desenvolvimento do App "Guerras Oriente" (App Inventor)

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

O presente trabalho tem como objetivo apresentar, de forma prática e organizada, o resultado final do projeto realizado, utilizando a ferramenta App Inventor, a respeito dos conflitos na região do Oriente Médio. Por meio de registros em imagens (prints), busca-se demonstrar a funcionalidade prática do aplicativo, evidenciando a aplicação dos conceitos aprendidos, bem como a evolução na construção do aplicativo. Dessa forma, o material reúne a interface final do aplicativo e o código desenvolvido.
### Palavras-chave: 
App Inventor, Oriente Médio, Conflitos, Componentes Avançados.

---

# Introdução

O Oriente Médio historicamente se posiciona como um dos principais epicentros de tensões geopolíticas, sociais e territoriais do cenário global contemporâneo, sendo de extrema importância a divulgação de conhecimento histórico, geográfico e humanitário. Diante disso, este trabalho apresenta o desenvolvimento do aplicativo mobile intitulado "Guerras do Oriente" partindo de uma ferramenta digital e interativa desenvolvida na plataforma App Inventor.
Nesse contexto, o projeto atua como uma plataforma técnico-educativa capaz de instruir o usuário acerca da dinâmica dos conflitos no Oriente Médio através de quatro pilares fundamentais: a conscientização civil humanitária, a cronologia dos fatos, a síntese analítica das principais disputas e a fixação do espaço geográfico.
Dessa maneira, a relevância científica e tecnológica deste projeto reside na utilização de recursos tecnológicos na divulgação de conteúdos educativos considerados essenciais ao conhecimento geral fundamentados em pesquisas e de um jogo interativo para a conscientização geográfica.

---

# Descrição e Funcionamento

O presente aplicativo tem como objetivo informar o usuário sobre os conflitos no Oriente Médio, apresentando conteúdos educativos como uma linha do tempo histórica, explicações dos principais conflitos e um guia de segurança baseado em recomendações da ONU, além de reforçar o aprendizado da geografia dessa região de forma prática por meio de um jogo interativo.
Ao ser acessado na tela 1, possui uma tela que apresenta o aplicativo e as opções de navegação. Essa tela apresenta as seções do aplicativo, que incluem:

*	Guia de Segurança: As medidas básicas de segurança para civis em áreas de guerra recomendadas pela ONU divididas em “O que fazer em uma emergência” e “Protocolos de Abrigo” e um “Checklist de Emergência” com itens recomendados para se manter em um contexto de guerra.
*	Linha do Tempo: Linha visual com os anos que marcaram os principais acontecimentos do Oriente Médio a partir da Segunda Guerra Mundial.
*	Principais Conflitos: Cards que detalham os 6 principais conflitos dessa região.
*	GeoQuiz: Jogo que testa seus conhecimentos ao relacionar áreas no mapa com os países do Oriente Médio.
*	Mais Informações: Botões interativos com informações na web que detalham os principais conflitos relatados na seção anterior, além de um mapa indicando um dos pontos turísticos mais famosos do Oriente Médio.
*	Enviar Email ou Fazer ligação: Botões interativos para enviar um email ou fazer uma ligação ao desenvolvedor do site.

A tela “Guia de Segurança” segmenta as diretrizes oficiais da Organização das Nações Unidas (ONU) voltadas para a preservação da integridade física de populações civis imersas em zonas de guerra. As informações são organizadas didaticamente em duas frentes de ação: "O que fazer em uma emergência" e "Protocolos de Abrigo". Além disso, a tela implementa um Checklist de Emergência funcional. Através do uso de caixas de seleção, o usuário pode registrar os insumos e providências que já possui ou tomou.

A tela “Linha do Tempo” apresenta uma estrutura composta por marcos temporais importantes. Ao interagir via clique com um ano específico, o sistema processa a requisição e exibe o acontecimento geopolítico correspondente àquele período. O engajamento do usuário é estimulado por um algoritmo de validação de progresso: a visualização da linha cronológica completa apenas se consolida após o acionamento individual de todos os doze botões dispostos.

A tela “Principais Conflitos” é estruturada em seis botões principais que representam as maiores disputas do Oriente Médio. O funcionamento lógico desta tela impõe uma restrição de concorrência: o sistema permite a exibição do resumo de apenas um conflito por vez. Ao clicar em um determinado botão, o bloco informativo correlato torna-se visível, enquanto os demais resumos são automaticamente ocultados pelo sistema, garantindo um foco visual direcionado e livre de distrações.

A tela inicial do “GeoQuiz” possui uma prévia do mapa com as identificações dos países por números, uma breve explicação da importância de conhecer a geografia de uma região, a explicação de como o jogo funciona e quais os países presentes no mapa, com ao fim, um botão para iniciar o jogo. O jogo funciona da seguinte maneira: o usuário observa o número exigido na pergunta e identifica o país correspondente àquela posição no mapa digitando-o corretamente no campo de texto. Ao clicar no botão “Enviar”, o aplicativo valida a resposta e só permite prosseguir em caso de acerto, além de exibir uma mensagem caso a resposta esteja incorreta. O botão "Dica", disponível apenas após pelo menos um acerto, fornece as três primeiras letras da resposta correta, reduzindo 3 pontos da pontuação final. Caso o usuário queira encerrar o quiz sem completá-lo, o botão "Desistir" finaliza o jogo e o direciona diretamente para a tela de encerramento do jogo, que exibe suas informações até a desistência. A tela de finalização exibe a mensagem de parabéns pelo reconhecimento geográfico caso o usuário conclua o quiz, além de informações sobre seu desempenho: a duração do quiz, qual o total de tentativas em relação aos acertos e a pontuação final. 

A tela “Mais informações” apresenta uma lista vertical de botões interativos dedicados a cada um dos tópicos fundamentais: "Oriente Médio: resumo", "Guerra Irã-Iraque", "Guerra dos Seis Dias", "Guerra Yom Kippur", "Guerra do Golfo", "Guerra Civil na Síria" e um direcionamento cartográfico em "Mapa". Ao acionar qualquer um desses botões, o aplicativo executa uma chamada de sistema que redireciona o usuário, via navegador web integrado, a artigos e matérias aprofundadas sobre o respectivo conflito ou ao mapa da “Cidade Perdida” ou “Petra” na Jordânia, um importante ponto turístico.

A tela “Enviar Email ou Fazer Ligação” permite o contato imediato com os desenvolvedores do projeto, oferecendo duas opções de ação: o acionamento de um código que abre o cliente de e-mail nativo do dispositivo móvel com o endereço eletrônico do autor, ou a inicialização da interface de discagem telefônica do aparelho para chamadas de suporte.

Vale ressaltar ainda que cada tela possui um menu no canto superior esquerdo, indicando as opções de navegação disponíveis a partir daquela tela – ou seja, a tela do guia de segurança possui em seu menu apenas as opções de início, linha do tempo, principais conflitos, geoquiz, mais informações e enviar email ou fazer ligação.

---

# Componentes e Conceitos Aplicados

Para o desenvolvimento do projeto foi fundamento em alguns conceitos da apostila apresentada em sala de aula, sendo eles:

*	Eventos (clique de botão, envio de resposta),
*	Manipulação de telas (troca entre screens),
*	Design eficiente (uso de arrangements),
*	Design agradável (cores de fundo e do texto para personalização). 

A implementação prática dos componentes utilizados fundamenta-se nos itens a seguir:

*	TextBox: entrada de respostas do usuário;
*	CheckBox: seleção pelo usuário;
*	Button: envio de respostas e navegação;
*	Label: exibição de textos explicativos e resultados;
*	Image: imagens sobre o tema;
*	Spinner: menu com opções de navegação;
*	Arrangements: incluindo o Scroll Arrangement, permitiram melhor organização dos componentes;
*	Notifier: mensagens importantes no jogo, como o erro e a não utilização da dica;
*	Clock: armazenamento do tempo de quiz;
*	TinyDB: armazenamento de informações entre as telas do jogo;
*	Screens: organização do app em múltiplas telas.
*	ActivityStarter: acesso ao navegador do dispositivo;
*	EmailPicker / PhoneCall: intents de envio de e-mail e realização de chamadas telefônicas.

Em relação aos recursos de lógica, vale a pena enfatizar a utilização de variáveis globais, procedimentos, estruturas condicionais (if, else if, else), bem como o sensor de tempo e o componente de armazenamento tinydb.

### Diferenciais

O aplicativo "Guerras do Oriente" apresenta inovações significativas em relação aos modelos de software descritos na apostila, destacam-se:

*	Adição de tempo de duração do quiz com um sensor;
*	Sistema de pontuação e feedback em tempo real conforme o usuário interage com o aplicativo;
*	Botão de encerrar o jogo, alterando o comportamento da tela final;
*	Uso de variáveis para armazenar pontuação, tempo, respostas;
*	Uso de listas para o sistema de perguntas e respostas e a exibição de arrangements conforme a intenção do usuário;
*	Ocultação da visibilidade de componentes para promover maior interação entre usuário e aplicativo

---

# Referências
* CAMPOS, T. Guerra Yom Kippur. Disponível em: <https://www.historiadomundo.com.br/idade-contemporanea/guerra-do-yom-kippur-e-a-crise-do-petroleo.htm>. Acesso em: 12 de abril 2026.
* GUITARRARA, P. Oriente Médio. Disponível em: <https://brasilescola.uol.com.br/geografia/oriente-medio.htm>. Acesso em: 12 de abril 2026.
* IBGE. Oriente Médio. Disponível em: <https://atlasescolar.ibge.gov.br/continentes-e-regioes-do-mundo/2968-oriente-medio.html>. Acesso em: 16 maio 2026.
* NAÇÕES UNIDAS BRASIL. ONU lança guia para proteger escolas e hospitais em zonas de conflito. Disponível em: <https://brasil.un.org/pt-br/66074-onu-lan%C3%A7a-guia-para-proteger-escolas-e-hospitais-em-zonas-de-conflito>. Acesso em: 12 maio 2026.
* NEVES, D. Guerra Civil Síria. Disponível em: <https://brasilescola.uol.com.br/geografia/conflito-na-siria-primavera-que-nao-consegue-se-estabelecer.htm>. Acesso em: 19 de abril 2026.
* OLIVEIRA, R. A Guerra dos Seis Dias: 1967, o início da ocupação. Disponível em: <https://diplomatique.org.br/guerra-dos-seis-dias-1967-inicio-ocupacao/ >. Acesso em: 19 de abril 2026.
* ROUMIEH, E. Saiba o que foi a Guerra do Golfo. Disponível em: <https://www.politize.com.br/autores/erica-yazigi-roumieh/ >. Acesso em: 19 de abril 2026.
* SILVA, D. Guerra Irã-Iraque. Disponível em: <https://brasilescola.uol.com.br/geografia/a-guerra-ira-iraque.htm>. Acesso em: 12 de abril 2026.
