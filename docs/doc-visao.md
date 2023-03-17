# Documento de Visão

Documento construído a partido do **Modelo BSI - Doc 001 - Documento de Visão** que pode ser encontrado no
link: https://docs.google.com/document/d/1DPBcyGHgflmz5RDsZQ2X8KVBPoEF5PdAz9BBNFyLa6A/edit?usp=sharing

## Equipe e Definição de Papéis

Membro     |     Papel   |   E-mail   |    Github   |
---------  | ----------- | ---------- |  ---------- |
David      | Gerente, Analista | davidccb@live.com | daviddevolin |
Manoel     | Analista | manoel.anizio456@gmail.com | manizio |
Lucas     | Analista | lucascantodev@gmail.com | lucascantodev |
Isadora   | Analista | isadorashs1@gmail.com | isadorazs |
Ítalo   | Analista | italog09@gmail.com | italoguil |


### Matriz de Competências

Membro     |     Competências   |
---------  | ----------- |
David      | Full-Stack Developer - Python, C, Java, JavaScript, HTML, CSS, React.js, MySQL, Django |
Manoel | Desenvolvedor Python, Java, C/C++, JavaScript, HTML, CSS, React.js, MySQL, Django |
Lucas | Desenvolvedor JavaScript, HTML, CSS, React.js, NextJS, Node, MySQL |
Isadora | Desenvolvedora Python, Java, C/C++, JavaScript, HTML, CSS, React.js, MySQL, Django |


## Perfis dos Usuários

O sistema poderá ser utilizado por diversos usuários. Temos os seguintes perfis/atores:

Perfil                                 | Descrição   |
---------                              | ----------- |
Administrador | Este usuário realiza os cadastros de despensas e pode realizar qualquer função.
Cliente | Este usuário pode visualizar, adicionar, remover e editar itens da despensa

## Lista de Requisitos Funcionais

Requisito                                 | Descrição   | Ator |
---------                                 | ----------- | ---------- |
RF001 - Manter um cadastro de Centros     | Um centro representa uma unidade administrativa da Universidade. Um centro tem código, nome, sigla, endereço e site. | Administrador |
RF002 - Manter um cadastro de Departamentos | Um departamento tem código, nome, sigla, endereço e o centro a qual pertence. | Administrador |
RF003 - Manter o cadastro de Salas | Uma sala tem um número, um nome, capacidade, tamanho, bloco e o centro a qual pertence. | Administrador |
RF004 - Manter cadastro de Componentes Curriculares | Um componente curricular é de um tipo de componente. Um componente curricular tem: código, nome, ementa, departamento, carga horária e modalidade, equivalências e requisitos com outros componentes, data de criação. | Administrador |
RF005 - Manter o cadastro de Horários de Aula | Um horário tem: um dia de semana, um turno, uma ordem (ordenação/identificador), uma hora de início, uma hora de final | Administrador |
RF006 - Manter o cadastro de professores | um professor tem: matrícula, nome, e-mail, telefone e o departamento | Administrador |
RF007 - Manter cadastro de Turmas | Uma turma tem: código, professor, sala e horários (horário da turma). Uma turma é de um componente curricular. Uma turma tem um ou mais professores. Uma turma tem uma ou mais salas. Uma turma tem vários horários de aulas. | Chefes e Coordenadores |

### Modelo Conceitual

Abaixo apresentamos o modelo conceitual usando o **YUML**.

 ![Modelo UML](yuml/monitoria-modelo.png)

O código que gera o diagrama está [Aqui!](yuml/monitoria-yuml.md). O detalhamento dos modelos conceitual e de dados do projeto estão no [Documento de Modelos](doc-modelos.md).

#### Descrição das Entidades

## Lista de Requisitos Não-Funcionais

Requisito                                 | Descrição   |
---------                                 | ----------- |
RNF001 - Deve ser acessível via navegador | Deve abrir perfeitamento no Firefox e no Chrome. |
RNF002 - Consultas deve ser eficiente | O sistema deve executar as consultas em milessegundos |
RNF003 - Log e histórico de acesso e funções | Deve manter um log de todos os acessos e das funções executadas pelo usuário |

## Riscos

Tabela com o mapeamento dos riscos do projeto, as possíveis soluções e os responsáveis.

Data | Risco | Prioridade | Responsável | Status | Providência/Solução |
------ | ------ | ------ | ------ | ------ | ------ |
16/03/2023 | Implementação de protótipo com as tecnologias | Alto | Todos | Vigente | Procurar por materiais de ensino abrangentes sobre a tecnologia em questão e realizar um caso simples de implementação como exercício inicial |
16/03/2023 | Falta de conhecimento das tecnologias | Alto | Todos | Vigente |Pesquisar tutoriais, assistir aulas sobre o assunto |
16/03/2023 | Distribuição inadequada de responsabilidades | Médio | Gerente | Vigente | Compreender precisamente as demandas do cliente em cada interação e ser pragmático ao estabelecer o que produzir diante do tempo disponível dos colaboradores da equipe |
16/03/2023 | Atrasos na entrega de tarefas | Alta | Todos | Vigente |  planejar e executar as atividades com antecedência, sem deixar de dedicar um pouco do tempo de cada dia ao projeto |

### Referências