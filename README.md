<h1 align="center">Sistema Resilia</h1>

## Descrição do Projeto
<p align="justify">Neste projeto, foi desenvolvida uma modelagem de banco de dados para o lançamento de um novo sistema de acompanhamento para armazenar cursos, turmas e alunos da Resilia.</p>

## Modelo Relacional
![Diagrama](https://github.com/MarianaFigueiredoI/projeto-individual-m4/blob/main/modelo_relacional.png)

## Perguntas realizadas:

### Existem outras entidades além de curso, turma e aluno?
Além das entidades solicitadas, existem mais três: 
* Instituicao_de_ensino;
* Docente;
* Disciplina.


### Quais são os principais campos e tipos?
<p align="justify">Os principais campos são: ins_cnpj (VARCHAR), cur_id (INT), tur_id (INT), alu_matricula (INT), doc_cpf (VARCHAR), e dic_id (INT), que são as chaves primárias de cada entidade.</p>

### Como essas entidades estão relacionadas?
<p align="justify">As entidades se relacionam mediante ao uso de chaves estrangeiras que fazem referência à chave primária de outras entidades. Por exemplo, a chave primária da entidade ‘turma’ é utilizada como chave estrangeira nas entidades ‘aluno’ e ‘docente’.<br>
Existem três principais tipos de relacionamentos: um para um, um para muitos e muitos para muitos. No diagrama desenvolvido, pode-se observar que o tipo de relacionamento de ‘instituicao_de_ensino’ e ‘curso’ é de um para muitos, pois uma instituição contém um ou mais cursos, porém um curso pertence a somente uma instituição; ‘curso’ e ‘turma’ é de um para muitos, pois um curso possui uma ou mais turmas, porém uma turma possui apenas um curso; ‘curso’ e ‘disciplina’ é de um para muitos, pois um curso pode conter uma ou mais disciplinas, porém uma disciplina pertence a somente um curso; ‘curso’ e ‘turma’ é de um para muitos, pois um curso possui uma ou mais turmas, porém uma turma pertence a somente um curso; ‘turma’ e ‘aluno’ é de um para muitos, pois os alunos possuem uma turma; ‘docente’ e ‘disciplina’ é de um para muitos, pois um docente leciona uma ou mais disciplinas, porém uma disciplina é lecionada por apenas um docente.</p>
