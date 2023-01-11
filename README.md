# ProjetoDiagramadbCursos.

O sistema foi Desenvolvido da seguinte forma.

1.EXISTEM MAIS ENTIDADES?
SIM.

Além das entidades(tabela cursos,turmas e alunos)
teve as entidades.
Instrutor :para as turmas.
Endereço: para ter os endereços dos alunos e professores.
Unidade:Para os cursos.
ALUNO_has_Turma: onde temos a matricula do aluno,código(nome) da turma
e o instrutor que terá na turma assim a tabela terá a relação das entidades ALUNO E TURMA 
pois os alunos podem ter várias turmas assim como a turma podem ter vários alunos.

2.PRINCIPAIS CAMPOS E TIPOS?

cada tabela terá vários campos como nome ,chave primária(para identificação para o relacionamento),nome do curso,
código da turma,professor dessa turma,onde os tipos serão VARCHAR(100) com 100 caracteres ,alguns campos como
data de nascimento será do tipo DATE,e alguns campos como o SALA que serão INT ,é o número da sala que a turma ocupa.)

3.COMO SE RELACIONAM?

A Unidade terá vários cursos que possuirá carga horária e preço ,sua unidade será herdada pela Id_unidade o nome da tabela UNIDADES.
Na tabela turmas temos seu código que irá para a Tabela cursos ,a tabela turmas terá seus dias da semana ,número da sua sala e seu turno.
Essa turma terá vários alunos que fará parte de um curso ,assim como o aluno pode ser de várias turmas
criando outra tabela que terá o nome da disciplina e o professor que irá ministrar a turma.
que herdará da tabela instrutor da chave ID_NOME na tabela Instrutor.

As tabelas aluno e professor além de ter vários alunos em uma turma e 1 professor para cada turma ,temos que o aluno possui 1 endereço assim como o instrutor e a unidade.
