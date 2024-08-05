# Desafio-Beedoo
Este desafio tem o objetivo de avaliar os conhecimentos e habilidades em teste de software.


Link do Drive contendo evidências das execuções dos Casos de Testes:

https://drive.google.com/drive/folders/1ZCkJ-ogy2hOtH2dSR5c2sAtATyG7WbAI?usp=sharing

Link da planilha com Casos de Testes:

https://docs.google.com/spreadsheets/d/1B-f0FaRjwqSeRmyy8u4IWRopBIpR5njEg_PF9lizwos/edit?usp=sharing

## Sugestões
1. Falta filtro para pesquisar um curso, por exemplo: Tecnologia, Economia, Direito, Linguas e etc...
2. Falta barra de pesquisa para pesquisar por um curso diretamente.
3. Falta adicionar categorias de acordo com a área do curso e permitir o usuário professor cadastrar o curso e escolher a área do curso.
4. Falta adicionar mensagens nos campos para informar que o campo é obrigatório ser preenchido ao Cadastrar um Curso.
5. Adicionar botão para editar um curso.

## Perguntas:
### *Durante os testes do módulo de curso do Beedoo Chalenge, você pode descobrir um erro (exemplo 404) em algum fluxo. Descreva o bug identificado, incluindo passos para reproduzi-lo, gravidade do problema e o que pode ocasionar esse tipo de erro.*

Foi encontrado o erro 404 ao atualizar a página estando na tela de 'Cadastrar Curso'.

Passo a passo: 
1. Logar no sistema.
2. Clicar em 'Cadastrar Curso'
3. Clicar em atualizar a página.

A gravidade do erro é alta, esse tipo de erro não deveria ocorrer ao recarregar a página, caso o usuário precise atualiza-la ou após ele ficar um certo tempo sem acessar a página aberta no computador.

Ao tentar atualizar a página pode ser que o sistema não esteja reconhecendo que o comando é pra recarregar, resultando assim em um erro 404.


### *Na criação do curso existem vulnerabilidades. Liste quais vulnerabilidades foram identificadas em seus testes e quais técnicas utilizaria para identificar outras potenciais vulnerabilidades.*
1. o campo de Link de Inscrição precisa de um verificador de link confiável para não permitir que seja utilizado com más intenções colocando links contendo vírus.
2. o campo de Url da imagem de Capa precisa de um verificador de link confiável e verificar se é uma imagem ou não.
3. o campo de Url está permitindo o envio de qualquer tipo de arquivo, podendo ser alvo de usuários com más intenções
4. ter limite de tamanho para imagem enviada em Url da imagem de Capa

Pode ser utilizado outras técnicas para identifcar possíveis vulnerabilidades como:
1. tentativa de realizar SQL Injection.
2. verificação de XSS.

### *Situação hipotética: dado que você recebe a especificação do módulo de curso para testar a funcionalidade. Identifique ao menos 3 pontos críticos que exigem esclarecimentos do time responsável antes do início dos testes. Qual seria o próximo passo e como seria realizado para garantir que a funcionalidade seja entregue com qualidade?*
Perguntas:
1. Quem será permitido cadastrar um curso? Qualquer usuário ou apenas usuários com permissões especiais?
2. Quem poderá se cadastrar no curso? Qualquer usuário? ou apenas usuário que possuem alguma qualificação no sistema como por exemplo uma assinatura?
3. Quais as principais funcionalidades do sistema?
3. Os cursos serão pagos?
4. Será necessário testes automatizados?

Passos para gaarantir que a funcionalidade seja entregue com qualidade:
1. O próximo passo seria a elaboração de um Plano de Testes, contendo todas as informações necessárias em relação aos testes.
2. Depois seria feito alguns Testes exploratórios para conhecer o sistema apresentado.
3. Depois seria criado uma documentação com Casos de Uso, para melhor análise dos fluxos.
4. Depois seria criado uma documentação de Tabela de Decisão, para melhor análise das decisões do sistema e das regras de negócios.
5. Depois teria a Criação dos Casos de Testes, cobrindo as funcionalidades e casos de usos que serão feitos pelos usuários.
6. Depois teria a Execução dos testes, e durante a execução, a comunicação com a equipe de desenvolvimento e PO será crucial para informar sobre erros, bugs, tirar dúvidas e/ou dar sugestões de melhorias para o sistema.
7. Depois teria o Teste de Aceite de Usuário, onde o usuário iria utilizar o sistema e avaliar se atende as necessidades de negócio dele.

### *Você recebe essa feature para testar e nos seus testes você identifica alguns erros. Como você avalia e define se o erro foi causado por essa feature? Caso não seja causado por ela, o que faria?*
Primeiro eu verifico o que causou ela, tento reproduzir o erro e faço uma análise em qual será o provável defeito dentro da implementação do sistema. Se o erro não for causado por ela, eu comunicaria os desenvolvedores para avaliar melhor a situação e eu conseguir reportar o erro com maior clareza.

## Decisões tomadas em relação as Users Story
1. Quais as funcionalidades do sistema?
2. Qual será o objetivo do usuário ao utilizar tais funcionalidades?
3. Qual será a qualificação do usuário que irá se utilizar do sistema?
4. Que tipo de permissões de usuário são necessárias para cadastrar um curso?
5. Que tipo de permissões de usuário são necessárias para excluir um curso?

## Users Story
1. Como um professor / Quero cadastrar um curso no sistema / Para que eu possa passar meus conhecimentos a outras pessoas.
2. Como um professor que cadastrou um curso / Quero excluir um curso / Para que eu possa retirar um curso desatualizado do sistema.
3. Como um professor que cadastrou um curso / Quero editar um curso cadastrado por mim / Para que eu possar suas informações.

