# TECHNICAL DESIGN DOCUMENT - TDD

## Seção 1 - Técnica de Elicitação de Requisitos

### Personas
"Uma persona é um personagem fictício, arquétipo hipotético de um grupo de usuários reais, criada para descrever um usuário típico" - BARBOSA, 2010.

Para cada papel de usuário deve ser criado ao menos uma persona formando um elenco de personas para o projeto que consiste entre 3 a 12 personas distintas. Cada elenco de personas possui ao menos uma persona primária, porém a recomendação que haja pelo menos 3 personas primárias no elenco de personas.

O elenco de personas pode ser complemntado por personas secundárias, que são demais stackholders envolvidos, mas que não é o público alvo da interface e anti-personas, que são aqueles para quem a interface não é projetada.

#### PERSONA 1: Primária

<img src="./img/personas/foto1.jpg" width="auto" height="200" alt="Persona 1 - Nicolly Souza">

Nicolly Souza, aluna do curso de Engenharia de Software, 20 anos. Ele está cursando a disciplina de IHC. Durante o ensino médio ela fez um curso de design gráfico, o qual lhe deu uma boa percepção para elaborar interfaces.

Ela costuma separar longos períodos de estudo, onde, ao som de um bom Jazz instrumental, se dedica e foca até conseguir ter a percepção que está dominando bem a matéria, no caso até o ponto que foi ministrado em sala de aula pelo professor. Nicolly tem o hábito de estudar bem a teoria, seguindo os livros base que os professores sugerem, e depois fazer exercícios para fixar.

Nesse semestre atípico da faculdade ela se preocupa com seu desempenho nas disciplinas, pois as estão acontecendo diversas reuniões de trabalho em grupo durante a semana que acabam quebrando seu ritmo de estudo. Agora seu objetivo é se adaptar a essa nova realidade. 

#### PERSONA 2: Primária

<img src="./img/personas/foto2.jpg" width="auto" height="200" alt="Persona 2 - Carlos André Feitosa da Silva">

Carlos André Feitosa da Silva, aluno do curso de Engenharia de Software, tem 21 anos. Ele está cursando a disciplina de IHC. Gosta bastante jogos eletrônicos e toca violão.

Carlos ainda tem uma boa rotina de estudos, ele costuma prestar bem a atenção nas aulas, anotar e sanar dúvida ali, pois em casa ela acaba estudando apenas quando se sente disposto ou quando realmente existe a necessidade de uma prova ou entrega de lista de exercícios que precisam ser entregues muito em breve. Ele prefere ir direto para a prática a partir do conhecimento prévio visto em sala de aula e a medida que vai tendo dúvidas na resolução de exercícios ele vai consultando os livros ou suas anotações.

Seu desejo é fazer o mínimo possível de esforço fora da sala de aula para entender a matéria, pois em casa quer passar o tempo descansando, tocando violão ou jogando vídeo game.

#### PERSONA 3: Primária

<img src="./img/personas/foto4.jpg" width="auto" height="200" alt="Persona 3 - Felipe Pereira">

Felipe Pereira dos Santos, aluno do curso de Engenharia de Software, tem 22 anos. Ele está cursando a disciplina de IHC.

Felipe gosta de balancear o estudo de forma que é estudado bem sobre um assunto pequeno e praticá-lo até sentir que está bem naquele tópico, assim Felipe acaba estudando em vários momentos diferentes do dia, pois não gosta de ficar estudando por um período muito longo sobre um assunto, o que se encaixou muito bem com as aulas remotas, onde ele pode ter períodos de descanso durante suas atividades, assim conseguindo atingir o seu objetivo, que é estudar de forma leve, sem ficar exausto por estar a muito tempo estudando. 

#### PERSONA 4: Anti-persona

<img src="./img/personas/foto3.jpg" width="auto" height="200" alt="Persona 4 - Renato Queiroz">

Renato Queiroz, aluno do curso de Engenharia de Software, tem 23 anos. Ele está cursando a disciplina de IHC.

Renato é um aluno que tem orgulho de dizer que estuda na UnB, porém não se esforça em suas atividades. Sua escolha de curso foi baseada no salário e status da profissão, mesmo ele percebendo que não gosta do seu curso, ele continua o curso com o objetivo de ficar rico após se formar. Seu objetivo é se formar e passar em qualquer concurso que pague bem, sem se importar quais funções serão exercidas por ele.

## Seção 2 - Elicitação dos Requisitos

### Requisitos Funcionais
- RF01: CRUD do Jogador [Brainstorming]
- RF02: O Jogador deve ser capaz de iniciar, progredir e finalizar as fases [Brainstorming]
- RF03: O Jogador deve ser capaz de responder cada questão [Brainstorming]
- RF04: O Jogo deve contabilizar a porcentagem de progresso da fase jogada [Brainstorming]
- RF05: O Jogador deve ser capaz de entrar e sair do jogo [Brainstorming]
- RF06: O Jogo deve salvar o progresso do jogador a cada confirmação de resposta [Brainstorming]
- RF07: O Jogo deve aceitar e verificar a resposta selecionada pelo jogador em cada questão[Brainstorming]
- RF08: As questões de cada fase devem disponibilizar o corpo textual da pergunta ou afirmativa [Brainstorming]
- RF10: O jogador deve poder confirmar sua resposta antes dela ser aceita [Personas]
- RF11: O jogo deve armazenar e apresentar conteúdo textual das regras, história, conteúdo disciplinar acesso às regras do jogo [Protótipo] [Brainstorming]
- RF12: O jogo deve armazenar recompensas conquistadas [Protótipo] [Personas]
- RF13: O jogo deve possibilitar o ajuste de algumas configurações [Protótipo] [Brainstorming]


### Requisitos Não-Funcionais
- RNF01: O jogador deve ser capaz de visualizar seu progresso das fases [Brainstorming]
- RNF02: O jogador deve ser capaz de visualizar seu progresso nas questões [Brainstorming]
- RNF03: O jogador deve receber feedback ao final de cada fase, se conseguiu ou não passar para a próxima fase [Artigo CBIE] [Personas]
- RNF04: O Jogo deve apresentar dicas durante a execução das tarefas das fases [Artigo CBIE] [Personas]
- RNF05: O Jogo deve apresentar a história do jogo [Artigo CBIE]
- RNF06: O Jogo deve aprensentar o conteúdo da disciplina [Artigo CBIE] [Personas]
- RNF07: Opções selecionadas devem ser destacadas visualmente [Artigo CBIE]
- RNF08: O jogo deve apresentar uma breve explicação a cada tarefa caso o jogador erre a questão[Artigo CBIE] [Personas]
- RNF09: As tarefas de inspeção de interface devem apresentar um lista de componentes da interface e lista de opções de violação como resposta [Brainstorming]
- RNF10: O jogo deve apresentar a mecânica do jogo e suas regras [Artigo CBIE]
- RNF11: O jogo deve disponibilizar uma seção onde o aluno pode exercitar sobre qualquer conteúdo [Personas]
- RNF12: Ao clicar na fase desejada a opção de iniciar fica habilitada ao clique [Personas]
- RNF13: O jogo deve apresentar uma mensagem de congratulação em algumas tarefas caso o jogador acerte [Artigo CBIE] [Persona]
- RNF14: O jogo deve dar um feedback de conclusão da fase e direcionar para a próxima [Personas] [Artigo CBIE]
- RNF15:  O jogo deve dar feedbacks ao longo da fase para manter o engajamento do jogador [Quick and Dirty] [Artigo CBIE]
- RNF16: O jogo deve recompensar o jogador com emblemas e conquistas [Quick and Dirty] [Artigo CBIE]
- RNF17: O jogo deve apresentar um menu accessível [Protótipo] [Brainstorming]
- RNF18: O jogo deve disponibilizar no menu, o acesso às configurações, regras, história, conteúdo, recompensas, perfil do jogador, página principal e sair do jogo  [Protótipo] [Brainstorming]

## Seção 3 - Metas de Usabilidade e Experiência do Jogador

O modelo MEEGA + visa avaliar a qualidade dos jogos educacionais em termos de usabilidade e experiência do jogador da perspectiva dos alunos [Petri et al., 2018]. Neste projeto adotamos alguns desses critérios de qualidade, exceto os fatores de experiência do jogador relacionados a interação social.

| Fator de Qualidade     | Dimensão               | ID   | Descrição                                                                                                |   
|------------------------|------------------------|------|----------------------------------------------------------------------------------------------------------|
|      Usabilidade       | Estética               | 1    | O design do jogo é atraente (interface, gráficos, cartões, placas, etc.).                                |   
|                        |                        | 2    | A fonte e as cores do texto são bem combinadas e consistentes.                                           |   
|                        | Aprendizagem           | 3    | Eu precisava aprender algumas coisas antes de poder jogar.                                               |   
|                        |                        | 4    | Aprender a jogar esse jogo foi fácil para mim.                                                           |   
|                        |                        | 5    | Acho que a maioria das pessoas aprenderia a jogar esse jogo muito rapidamente.                           |   
|                        | Operabilidade          | 6    | Acho que o jogo é fácil de jogar.                                                                        |   
|                        |                        | 7    | As regras do jogo são claras e fáceis de entender.                                                       |   
|                        | Acessibilidade         | 8    | As fontes (tamanho e estilo) usadas no jogo são fáceis de ler.                                           |   
|                        |                        | 9    | As cores usadas no jogo são significativas.                                                              |   
|------------------------|------------------------|------|----------------------------------------------------------------------------------------------------------|  
| Experiência do Jogador | Confiança              | 10   | O conteúdo e a estrutura me ajudaram a ter certeza de que aprenderia com este jogo.                      |   
|                        | Desafio                | 11   | Este jogo é apropriadamente desafiador para mim.                                                         |   
|                        |                        | 12   | O jogo oferece novos desafios (oferece novos obstáculos, situações ou variações) em um ritmo apropriado. |   
|                        |                        | 13   | O jogo não se torna monótono à medida que avança (tarefas repetitivas ou enfadonhas).                    |   
|                        | Satisfação             | 14   | Concluir as tarefas do jogo me deu uma sensação satisfatória de realização.                              |   
|                        |                        | 15   | É pelo meu esforço pessoal que consegui avançar no jogo.                                                 |   
|                        |                        | 16   | Estou satisfeito com as coisas que aprendi com o jogo.                                                   |   
|                        |                        | 17   | Eu recomendaria este jogo aos meus colegas.                                                              | 
|                        | Diversão               | 18   | Eu me diverti com o jogo.                                                                                |   
|                        |                        | 19   | Algo aconteceu durante o jogo (elementos do jogo, competição, etc.) que me fez sorrir.                   |   
|                        | Atenção Focada         | 20   | Havia algo interessante no início do jogo que chamou minha atenção.                                      |   
|                        |                        | 21   | Eu estava tão envolvido em minhas tarefas de jogo que perdi a noção do tempo.                            |   
|                        |                        | 22   | Esqueci meu ambiente imediato enquanto jogava.                                                           |   
|                        | Relevância             | 23   | O conteúdo do jogo é relevante para os meus interesses.                                                  |   
|                        |                        | 24   | É claro para mim como o conteúdo do jogo se relaciona com o curso.                                       |   
|                        |                        | 25   | Este jogo é um método de ensino adequado para este curso.                                                |   
|                        |                        | 26   | Prefiro aprender com este jogo a aprender de outras maneiras (por exemplo, outros métodos de ensino).    |   
|                        | Aprendizagem Percebida | 27   | O jogo contribuiu para o meu aprendizado neste curso.                                                    |   
|                        |                        | 28   | O jogo permitiu um aprendizado eficiente em comparação com outras atividades do curso.    

               |   

## Histórico de Revisão

| Data | Versão| Descrição | Fase | Autor |
|----|----|----|----|----|
| 21/09/2020 | 1 | Criado o Documento TDD e adicionando Personas, requisitos fincionais e não funcionais, e as metas de usabilidade e de experiência do jogador | Análise de Requisitos | Mateus Sousa e Rossiscler|
| 05/10/2020 | 1.1 | Atualizando Requisitos e Rastreando suas origens | Análise de Requisitos | Mateus Sousa |
| 05/10/2020 | 1.1.2 | Adicionando fotos para as personas | Análise de Requisitos | Rossicler |
| 09/11/2020 | 1.2 | Atualizando tabela de metas de experiência do jogador e adicionando novos requisitos | Design, Desenvolvimento e Avaliação | Mateus Sousa |
| 23/11/2020 | 1.3 | Atualizando Requisitos | Design, Desenvolvimento e Avaliação | Mateus Sousa |



## Referências

- BARBOSA, S. D. J.; SILVA, B. S. DA. Interação Humano-Computador, 2010.
- COOPER, A. et al. About face 3: the essentials of interaction design. [3rd ed.], Completely rev. & updated ed. Indianapolis, IN: Wiley Pub, 2007. 
- PETRI, G.; WANGENHEIM, C. G. VON. A Method for the Evaluation of the Quality of Games for Computing Education. Anais dos Workshops do VIII Congresso Brasileiro de Informática na Educação (CBIE 2019). Anais... In: VIII CONGRESSO BRASILEIRO DE INFORMÁTICA NA EDUCAÇÃO. Brasília, Distrito Federal, Brasil: Brazilian Computer Society (Sociedade Brasileira de Computação - SBC), 21 nov. 2019 Disponível em: <https://br-ie.org/pub/index.php/wcbie/article/view/9045>. Acesso em: 15 ago. 2020
- DE SALES, A. B.; SOUSA E SILVA, M. A. Jogos Sérios no Processo de Ensino e Aprendizagem de Interação Humano-Computador. p. 10, 2020. 
- Fotos das personas. Disponível em: <https://br.depositphotos.com/stock-phtos/>. Acesso em 04 out. 2020
