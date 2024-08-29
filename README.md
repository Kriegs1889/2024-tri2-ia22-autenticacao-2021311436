# 2024-tri2-ia22-autenticacao-2021311436

# Autenticação de Usuários (single server)

...

## Autenticação VS Autorização
- O que é autenticação?
  È um processo para indentificar a identidade de um usuário ou sistema, respondento a pergunta "que é quem diz ser?", isso é um passo crucial para que apenas usuários legítimos possam acessar um sistema.

- Uma autenticação pode incluir:
- Nome de usuário e senha:
  Essa é a forma mais tradicional de indentificação, o usuário fornece um identificador único(nome de usuário), e um segredo(senha), para obter o acesso.

  - Autenticação multifator:
    Adiciona uma camada a mais de segurança, exigindo dois ou mais fatores de verificação, como uma senha e um código enviado para um dispositivo móvel.

  - Autenticação biométrica:
    Usa traços biológicos do usuário, como as digitais, reconhecimento facial e reconhecimento de íris.


    - O que é autorização?
      vem após a autenticação do usuário, e dita o que um usuário autenticado pode ou não fazer, A autorização tembém permite que só os usuários possas acessar recursos e realizar as devidas funçoẽs que são permitidas.

    - Alguns métodos de autentificação podem incluir:
    - Controle de acesso baseado em papéis (RBAC):
      Atribui permiçoẽs aos usuários de acordo com os seus papéis dentro de uma organização(como por exemplo, administrador, editor, visualizador).

    - Controle de acesso baseado em atributos (ABAC):
      Concede o acesso ao usuário com base em seus atributos e condiçoẽs ambientais(como por exemplo, hora e localização).

    - Listas de controle de acesso (ACLs):
      Especificam quais usuários ou processos tem permiçoẽs para acessar objetos e quais operaçoẽs são permitidas nesses objetos.
...

## Autenticação com Token (JWT)
JWT, resumidamente, é um string de caracters que, caso o cliente e o server estejam sobre HTTPS, permie que somente o server tenha a senha que permita autenticar o usuário. o token não é criptografado, ele é "assinado", de forma que só com a senha a assinatura possa ser comprovada, o que impede que token sejam criados por conta própria.
Em prática, quando o usuário se autentica no sistema ou web API(com usuário e senha), o server gera um token com uma data de expiração para ele. Durante as requisiçoẽs do usuário, o JWT é enviado no cabeçalho da requisição e, caso seja válido, a API dará o acesso aos recurso solicitados, sem a necessidade de se autenticar novamente.


...

## Projeto (Objeto de Estudos)

...
