
Buscar

Notificações
99+

Carreira
Desafios - Projetos Pessoais
Desafios

Projeto 2: Sistema de banco de dados de doação de sangue
Desenvolver um sistema de gerenciamento de um banco de dados de doação de sangue.
Cadastro de doadores
Validar dados.
No cadastro de endereço integrar API externa para consulta CEP. (PLUS)
Controle de estoque de sangue
Avisar quando o estoque atingir a quantidade mínima definida. (PLUS)
Registro de doações
Atualizar o estoque de sangue sempre que registrar uma doação.
Consulta de doadores
Consultar o histórico de doações de um doador.
Relatórios
Gerar um relatório sobre a quantidade total de sangue por tipo disponível. (PLUS)
Relatório de doações nos últimos 30 dias com informações dos doadores. (PLUS)


Criar Publicação no LinkedIn

Cumprimentar
Comunicar que está iniciando um projeto como parte do Treinamento (me marcando https://www.linkedin.com/in/luisdeol/)
Falar Sobre o Projeto
Concluir falando que vai publicando na rede sobre as evoluções do Projeto


Regras de negócio
Não deixar cadastrar um doador com o mesmo e-mail.
Menor de idade não pode doar, mas pode ter cadastro.
Pesar no mínimo 50KG.
Mulheres só podem doar de 90 em 90 dias.(PLUS)
Homens só podem doar de 60 em 60 dias. (PLUS)
Quantidade de mililitros de sangue doados deve ser entre 420ml e 470ml (PLUS)


Entidades e Dados
Doador
Id (int)
Nome Completo (string)
Email (string)
DataNascimento (datetime)
Genero (string)
Peso (double)
TipoSanguineo (string)
FatorRh (string)
Doacoes (List<Doacoes>)
Endereco (Endereco) (PLUS)


Endereco (PLUS)
Id (int)
Logradouro (string)
Cidade (string)
Estado (string)
CEP (string)
Doador (Doador)


Doacao
Id (int)
DoadorId (int)
DataDoacao (datetime)
QuantidadeML (int)
Doador (Doador)


EstoqueSangue
Id (int)
TipoSanguineo (string)
FatorRh (string)
QuantidadeML (int)



Stack / Padrões
Nível Básico I: Aplicação Console
Nível Básico II
ASP NET Core API
Entity Framework Core
POO
Banco em memória
Nível Intermediário
Fluent Validation
Padrão Repository
Middleware (Lidar com exceções)
InputModel, ViewModel, DTO’s (Modelos de entrada e saída de dados)
IEntityTipeConfiguration (mapear as entidades separadamente)
Sql Server ou SqLite
Nível Avançado
Unit Of Work
HostedService
Domain Event
CQRS
Teste Unitários
Arquitetura Limpa
Como você avalia este conteúdo?





Marcar como concluído
10%
17 Comentários



Mais recentes
Mais antigos
Meus comentários

Vinicius Benicio
6 meses atrás
Olá, aonde encontro conteúdos de Middleware (Lidar com exceções), Domain Event por gentileza
 
[Equipe LuisDev] Francisco Victor
6 meses atrás
Fala, Vinicius! Nas gravações dos encontros você encontra esses conteúdos
Tratamento de exceções: https://metododotnet.luisdev.com.br/185976-formacao-net-start/4309962-14-tratamento-de-excecoes
Eventos de domínio: https://metododotnet.luisdev.com.br/101358-aulas-dotlive/3969755-ef-core-deep-dive
 
Vinicius Benicio
6 meses atrás
Infelizmente não tenho acesso aos encontros, não tem outro conteúdo ou um link de algum artigo na internet, ou uma orientação de como pesquisar?
 
[Equipe LuisDev] Francisco Victor
6 meses atrás
A melhor forma de encontrar é no YouTube, Vinicius! No canal do Luis você já encontra alguns desse conteúdos https://www.youtube.com/@nextwave.education
 
Heros Hlatki Godoy
10 meses atrás
Onde posso encontrar conteúdo de integração de api?
 
[Equipe LuisDev] Francisco Victor
10 meses atrás
Fala, Heros! Aqui mesmo na plataforma, no curso de micro serviços, você encontra conteúdos sobre essa integração!
 
Ronan De Souza Castro
10 meses atrás
onde acho conteúdo de HostedService?
 
[Equipe LuisDev] Francisco Victor
10 meses atrás
Fala, Ronan! Nos módulos de micro serviços você encontrará conteúdos sobre hosted services.
 
Rafael santiago dos santos
cerca de 1 ano atrás
Pelo que entendi a relação das entidades vai ser de: Doador e Endereco 1 - 1 e Doador e Doacao 1 - N, seria isso?
 
[Equipe LuisDev] Francisco Victor
cerca de 1 ano atrás
Isso mesmo, Rafael!
 
Edilson Manjate
12 meses atrás
No segmento da pergunta do Rafael, usar Endereço como value object é recomendado?
 
[Equipe LuisDev] Francisco Victor
11 meses atrás
É uma boa opção sim, Edilson, já que podemos ter vários campos para representar um Endereço, então criando um ValueObject pra ele podemos reutilizar as lógicas da classe em outros trechos.
 
Rafael santiago dos santos
cerca de 1 ano atrás
No cadastro de endereço integrar API externa para consulta CEP. (PLUS), não entendi muito bem como seria essa implementação
 
[Equipe LuisDev] Francisco Victor
cerca de 1 ano atrás
Fala, Rafael! Seria a ideia de chamar alguma API externa para buscar CEPs na sua API. Você pode usar por exemplo a ViaCEP: https://viacep.com.br/

A ideia seria configurar sua API para que ela conseguisse acessar a ViaCEP, daí quando o usuário informasse o CEP, você buscaria as informações do CEP na API ViaCEP.
 
Rafael santiago dos santos
cerca de 1 ano atrás
Obrigado
Ver mais