# Reporte de BUGS

## DEF-001 - Sistema permite o cadastro de Curso sem nada no formulário preenchido.

Descrição: O sistema está permitindo o cadastro de Curso sem nenhum campo do formulário da tela de 'Cadastrar Curso' estar preenchido.

Objeto de Teste: Formulário de Cadastro de Curso.

Ambiente de Teste: Produção.

Caso de teste: CT-002 - Cadastrar um Curso sem nada preenchido

Passo a passo:
1. Logar no sistema
2. Clicar em 'Cadastrar Curso'
3. Clicar no botão 'Cadastrar Curso' do formulário

Evidências:

https://github.com/user-attachments/assets/59139bc7-0446-4a8b-97e5-c891140e899b

Resultado esperado: Não deveria permitir a criação do Curso sem nenhum campo estar preenchido, destacando em vermelho os campos não preenchidos e informando que eles são obrigatórios.

Resultado obtido: O sistema permitiu a criação do Curso sem dados com sucesso.

Severidade do defeito: Média.

## DEF-002 - Cadastrar um Curso com a Data de Fim anterior a Data de Início

Descrição: O sistema está permitindo o cadastro de Curso utilizando uma Data de Fim anterior a Data de Início.

Objeto de Teste: Formulário de Cadastro de Curso.

Ambiente de Teste: Produção.

Caso de teste: CT-035 - Cadastrar um Curso com a Data de Fim anterior a Data de Início.

Passo a passo:
1. Logar no sistema
2. clicar em 'Cadastrar Curso'
3. Clicar no botão 'Cadastrar Curso' do formulário
4. Digitar no campo 'Nome do Curso' 'Curso Teste'
5. Digitar no campo 'Descrição do Curso' 'Curso teste'
6. Digitar no campo  'Instrutor' 'Curso da silva'
7. Digitar no campo 'URL da imagem de capa' 'cursoteste.png'
8. Selecionar a Data de Início 12/08/2024
9. Selecionar a Data de Fim 05/08/2024
10. Digitar no campo 'Número de Vagas' '5'
11. Selecionar o Tipo de Curso Online
12. Digitar no campo 'Link de Inscrição' 'cursoteste.com'

Evidências:

https://github.com/user-attachments/assets/e1dead55-87f0-4054-8123-3e4d423e4d7f

Resultado esperado: Que o sistema não permitisse criar um Curso com a Data de Início sendo maior do que a Data de Fim, destacando ambos os campos e informando que a Data de Início não pode ser maior do que a Data de Fim.

Severidade do defeito: Média.

## DEF-003 - Atualizar a página estando na tela de Cadastro de Curso

Descrição: O sistema apresenta erro ao atualizar a página estando na tela de Cadastro de Curso, mostrando 'Page Not Found'

Objeto de Teste: Formulário de Cadastro de Curso.

Ambiente de Teste: Produção.

Caso de Teste: CT-040	- Atualizar a página estando na tela de Cadastro de Curso

Passo a passo:
1. Logar no sistema.
2. Clicar em 'Cadastrar Curso'
3. Clicar em atualizar página

Evidências:

https://github.com/user-attachments/assets/a572b894-4839-4afb-aa8c-26482ae4db01

Resultado esperado: Que o sistema recarregasse os elementos da página após atualiza-la

Resultado obtido: o sistema apresenta erro (Page Not Found)

Severidade do defeito: Média.

## DEF-004 - Impossibilidade de excluir um curso criado

Descrição: O sistema apresenta erro no console ao tentar excluir um Curso, apresentando erro 405 (Method not allowed), e na interface de usuário apresentando 'Curso excluído com sucesso!' não realizando a exclusão do curso.

Objeto de Teste: Formulário de Cadastro de Curso.

Ambiente de Teste: Produção.

Caso de Teste: CT-041	- Excluir um curso criado

Passo a passo:
1. Logar no sistema.
2. Tendo um curso criado, clicar no botão 'Excluir' do curso.

Evidências:

https://github.com/user-attachments/assets/9ddbe0ec-5003-4ecd-84bf-3eb4214af536

Resultado esperado: Que o sistema permitisse excluir um curso com sucesso.

Resultado obtido: Ao clicar no botão, apresenta erro 405 no console e na interface do usuário 'Curso excluído com sucesso!' não realizando a exclusão.

Severidade do defeito: Alta.
