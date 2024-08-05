# Desafio-Beedoo
Este desafio tem o objetivo de avaliar os conhecimentos e habilidades em teste de software.

```
Situação hipotética: dado que você recebe a especificação do módulo de curso para testar a funcionalidade. Identifique ao menos 3 pontos críticos que exigem esclarecimentos do time responsável antes do início dos testes. Qual seria o próximo passo e como seria realizado para garantir que a funcionalidade seja entregue com qualidade?
1. Quais as funcionalidades do sistema?
2. Qual será o objetivo do usuário ao utilizar tais funcionalidades?
3. Qual será a qualificação do usuário que irá se utilizar do sistema?
4. Que tipo de permissões de usuário são necessárias para cadastrar um curso?
5. Que tipo de permissões de usuário são necessárias para excluir um curso?
```

## Perguntas
1. Quem será permitido cadastrar um curso? Qualquer usuário ou apenas usuários com permissões especiais?
2. A tela de Listar Cursos será a mesma para o aluno/visitante?
  a. Terá opção do usuário aluno visualizar mais informações de um curso?
  b. Terá opção de se inscrever no curso direto através da tela de Listar Cursos?
4. Terá opção de editar um curso criado? Recomendo.
5. Qual o limite máximo e mínimo de caracteres para o campo 'Nome do Curso'?
6. Qual o limite máximo e mínimo de caracteres para o campo 'Descrição do Curso'?
7. Qual o limite máximo e mínimo de caracteres para o campo 'Instrutor'?
8. Qual o limite máximo e mínimo de caracteres para o campo 'Url da imagem de capa'?
9. Qual o limite máximo e mínimo para uma quantidade de vaga para um curso 'Presencial'?
10. Qual o limite máximo e mínimo para uma quantidade de vaga para um curso 'Online'?
11. Qual o limite máximo e mínimo de caracteres para o campo 'Link de Inscrição' quando o curso for 'Online'?
12. Qual o limite máximo e mínimo de caracteres para o campo 'Endereço' quando o curso for 'Presencial'?

## Sugestões
1. Falta filtro para pesquisar um curso, por exemplo: Tecnologia, Economia, Direito, Linguas e etc...
2. Falta barra de pesquisa para pesquisar por um curso diretamente.
3. Falta adicionar categorias de acordo com a área do curso e permitir o usuário professor cadastrar o curso e escolher a área do curso.
4. 

## Erros encontrados até agora:
1. Possível criar curso sem nenhuma informação (precisa tornar os campos obrigatórios)
2. Erro no console ao tentar excluir um curso e recebendo mensagem do sistema de apagado com sucesso
3. o campo de Link de Inscrição precisa de um verificador de link confiável
4. o campo de Url da imagem de Capa precisa de um verificador de link confiável e verificar se é uma imagem ou não
5. o campo de 'Número de Vagas' ta aceitando a letra 'e', -, +, .
6. Erro ao atualizar a página estando na tela de 'Cadastrar Curso'

## Decisões tomadas em relação as Users Story


## Users Story
1. Como um professor / Quero cadastrar um curso no sistema / Para que eu possa passar meus conhecimentos a outras pessoas
2. Como um professor que cadastrou um curso / Quero excluir um curso / Para que eu possa retirar um curso desatualizado do sistema
3. [sugerida] Como um professor que cadastrou um curso / Quero editar um curso cadastrado por mim / Para que eu possar suas informações 
4. Como um usuário ? / Quero utilizar a barra de pesquisa em Listar Cursos / Para que eu possa encontrar um curso específico rapidamente
5. Como um usuário ? / Quero utilizar o filtro de curso 'Tecnologia' em Listar Cursos / Para que eu possa encontrar cursos específicos daquela área
6. Como um usuário ? / Quero visualizar mais informações de um curso / Para que eu possa verificar se aquele curso vai atender as minhas necessidades
7. Como um usuário ? / Quero comprar um curso / Para que eu possa aprender mais sobre o assunto do curso

