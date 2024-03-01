# Documentacao-Shelfie
## Contribuidores
- Mayara Spieker Carvalho 
[![Github Badge](https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/mayspiek)](https://github.com/mayspiek) [![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/mayara-spieker/)](https://www.linkedin.com/in/mayara-spieker/) [![](https://img.shields.io/badge/Gmail-red?style=flat-square&logo=gmail&logoColor=white)](mailto:maya.spieker@gmail.com)
- Gabriela Marques dos Santos
[![Github Badge](https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/gabrielamarqs)](https://github.com/gabrielamarqs) [![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/gabriela-marques-dos-santos-899092161/)](https://www.linkedin.com/in/gabriela-marques-dos-santos-899092161/) [![](https://img.shields.io/badge/Gmail-red?style=flat-square&logo=gmail&logoColor=white)](mailto:margabrielaqs@gmail.com)

### Tecnologias
 <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" /> <img height="60em" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" /> <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" />

### Escopo Macro
O Shelfie é um **Sistema** de Gerenciamento de Leituras, e surge da necessidade de proporcionar aos viciados em livros uma ferramenta com a proposta de ser simples e intuitiva para o gerenciamento de suas experiências literárias.

O Shelfie visa não apenas registrar o status da leitura, mas também permitir que os usuários expressem suas opiniões, pensamentos e sentimentos em relação aos livros. Com funcionalidades como a organização do acervo, indicar a progressão da leitura (abandonado, em andamento, favoritos, na lista de leituras), paginômetro que conta a quantidade de páginas lidas, leitura em conjunto para acompanhar em grupo o progresso da leitura.
 
## Requisitos Funcionais
| Código do Requisito | Descrição | Caso de Uso |
| ------ | ------ | ------ |
| RF 01 | O ****Sistema**** deve permitir que os usuários se registrem no mesmo, com os seguintes dados: identificador único, login (e-mail), senha, nome, username e foto. <br> <br> Existem dois tipos de usuário no sistema: **Administrador** e **Leitor**. <br> <br> Deverá existir na base de dados um **Usuário** **Administrador** padrão, que não poderá ser excluído do sistema. <br> <br> Os usuários do tipo **Administrador** poderão cadastrar novos usuários **Administradores**. | UC 01 - Gerenciar **Usuário** |
| RF 02 | O sistema deve permitir que o **Usuário** gerencie seu acesso com os seguintes dados: email (login) e senha. | UC 02 - Gerenciar Acesso | 
| RF 03 | O **Leitor** deve ser capaz de gerenciar a sua leitura de livros, indicando o estado do livro, se ele já foi **lido**, está sendo lido, foi **abandonado**, está na lista de **próximas leituras**. O **Cliente** também deve ser capaz de excluir a associação do livro ao seu perfil. <br> <br> O **Leitor**, quando acessar a página do livro que está lendo, poderá visualizar quem são os outros usuários que estão lendo e que já leram o mesmo livro que ele. <br><br> A partir do gerenciamento de leituras, será montado um ranking de livros mais lidos e mais abandonados, mensalmente e anualmente. | UC 03 - Gerenciar Monitoramento/Acervo de Livros | 
| RF 04 | O **Leitor** deve ser capaz de anotar o progresso da leitura e deixar comentários e reações, indicando a última página lida do livro, mas o estado do livro tem que ser “lendo”. O **Leitor** também deve ser capaz de excluir estes registros. <br> <br> A quantidade de páginas lidas que vão ser adicionadas ao paginômetro, é o número da página colocada no último registro no progresso da leitura feito pelo **Leitor**. <br><br> Quando o **Leitor** adicionar um livro já com o status “lido”, vai ser adicionado somente o progresso final do livro, que seria a página final. | UC 04 - Gerenciar Progresso do Livro |
| RF 05 | O **Leitor** deve ser capaz de postar review e dar nota aos livros já lidos. E ele também deve ser capaz de votar na review de outros **Leitores**. | UC 05 - Gerenciar Review de Livros |
| RF 06 | O **Leitor** deve ser capaz de curtir ou retirar a curtida da review de outros **Leitores**. | UC 06 - Gerenciar Curtidas das Reviews |
| RF 07 | O **Leitor** deve ser capaz de reportar reviews de outros **Leitores** que infringem os Termos de Uso do **Sistema**. <br><br> E o **Administrador** deve ser capaz de analisar os reportes solicitados pelos **Leitor**es e definir se a review viola ou não os Termos de Uso do **Sistema**. | UC 07 - Gerenciar Reporte de Reviews |
| RF 08 | O **Leitor** deve ser capaz de adicionar os livros que estão lendo ou que já foram lidos como favoritos. Caso necessário, ele também poderá retirar o livro dos favoritos. | UC 08 - Gerenciar Livros Favoritos |
| RF 09 | O **Leitor** deve ser capaz de enviar solicitação de amizade para outros usuários, sendo que eles podem aceitar, recusar ou deixar pendente.  | UC 09 - Gerenciar Amigos | 
| RF 10 | O **Usuário** deve ser capaz de pesquisar os Livros por **título, autor e assunto**. Se o livro for encontrado, o sistema deverá fornecer informações detalhadas sobre o mesmo como **resumo, escritor, editora, ano de publicação e ISBN**. | UC 10 - Buscar Dados dos Livros | 
| RF 11 | O **Sistema** deve permitir que **Leitor** receba badges pela quantidade de livros lidos.  | UC 11 - Gerenciar Badges do **Usuário** | 

## Diagrama de Casos de Uso Geral
<img height="600em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/30441ff3-a7ef-4b38-94f4-0e2159dc07a1" />

## Modelo Entidade-Relacionamento
<img height="600em" src="https://github.com/shelfiie/Documentacao-Shelfie/assets/79992764/4dfe45bb-ec7e-4cde-bd50-db5b8c74f095" />
