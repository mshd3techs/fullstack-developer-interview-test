# Fullstack Developer Tnterview Test ( C#/Node and Angular 9)
Ao conhecer uma pessoa que está aplicando para a Férias & Co gostamos de ter uma conversa sobre código. Afinal, escrever, ler e discutir sobre código faz parte da nossa rotina diária de trabalho.

## O QUE VAMOS AVALIAR
Queremos avaliar sua capacidade de fornecer um produto simples com documentação suficiente para outros desenvolvedores contribuírem ativamente para o projeto posteriormente. Na entrevista vamos prestar atenção nos seguintes itens:

- Comunicação na revisão do código presencial;
- Argumentos sobre desafios enfrentados e escolhas realizadas na implementação;

Ao revisar seu código vamos prestar atenção nos seguintes itens:

- Organização do código;
- Código bem escrito, limpo e coeso;
- Arquitetura e princípios de desenvolvimento;
- Uso adequado de versionamento do código em git;
- Uso de testes automatizados;
- Deploy da aplicação: criação de arquivo docker;
- O design da API RESTful é implementado, usando corretamente os verbos HTTP e o código de status apropriado;
- Uso adequado de HTML5, CSS3 e JavaScript em um front-end minimamente estruturado.
- Caso você não se sinta confortável com algum desses itens, tudo bem, apenas nos fale sobre isso, ok? O objetivo aqui não é você programar de graça para nós, nem te fazer perder tempo com algo irrelevante. Nosso objetivo aqui é ter um código sobre o qual podemos conversar. Como você deve ter notado, a gente preza muito por colaboração, trabalho em time e comunicação. O objetivo aqui é ter, minimamente, essa experiência com você.

Respeite o seu nível de conhecimento e experiência, o importante é você saber dizer o motivo das suas escolhas. Se você tiver qualquer dúvida, por favor, entre em contato com a gente. Se quiser uma revisão no seu código em um Pull Request no Github, pode nos chamar. Estamos disponíveis para te ajudar a finalizar esse processo. Ah, por último. Você acha que consegue nos responder em quanto tempo? Duas semanas é ok para você?

## IDEIAS DE PROJETOS
A seguir seguem uma história do usuário e os seus cenários para o desenvolvimento. Você terá que implementar um serviço REST com a funcionalidade solicitada e uma aplicação Angular 9 que consuma o mesmo serviço.

Ambos devem ter o seu proprio Dockerfile e um arquivo Docker-Compose para subir a stack do serviço e a sua interface. 

```feature
Funcionalidade: Gestão de reservas de quartos.

  "Eu, como o um dos responsáveis pela gestão de reservas do hotel Férias & Co, 
  quero registrar uma nova reserva de quartos,
  para realizar um melhor controle sobre os quartos reservados"

  Cenário: Reserva de quarto.
    Dado uma nova reserva de quarto
    E fornecido os nomes completos de cada hospede 
    E as suas datas de nascimento
    E os seus CPFs
    E indicado qual deles é o pagante
    E o ids dos quartos reservados
    E indicado quais hospedes ficaram em cada quarto
    E informado a data de entrada(Check-in)
    E a data de saída(Check-out),
    Quando solicitado a reserva
    Então garanta que os dados sejam armazenados
    E gere um indentificador único para essa transação.

  Cenário: Quarto já reservado.
    Dado uma nova reserva de quarto
    E fornecido id de um quarto ja esteja reservado 
    Quando solicitado a reserva
    Então garanta que os dados não sejam armazenados
    E informe que o quarto está reservado.

  Cenário: Quarto inexistente.
    Dado uma nova reserva de quarto
    E fornecido id de um quarto que seja inexistente 
    Quando solicitado a reserva
    Então garanta que os dados não sejam armazenados.
    E informe que o quarto não existe.
    
```
Tem alguma outra ideia? Tem algum projeto que já está pronto e gostaria de apresentar? Fale com a gente :)

## COMO COMPARTILHAR O PROJETO CONOSCO
Apague este README.md e adicione informações que achar relevante como configurar o projeto, contendo os comandos que devem ser executados para executar ele e os testes;
Abra um PR apontando para a branch master deste repositório;
Escreva qualquer consideração na descrição do PR e faça qualquer comentário que achar pertinente no código.
