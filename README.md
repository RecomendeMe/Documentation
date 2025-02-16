# Documentação 
Documentação Geral do Projeto RecomendeMe 



## Arquitetura atual

O RecomendeMe é uma plataforma web desenvolvida para que usuários possam compartilhar e descobrir recomendações em diferentes comunidades temáticas, como filmes, livros, álbuns e jogos. Cada página da plataforma representa uma comunidade, e dentro delas, os usuários podem submeter recomendações que passam por um processo de validação antes de serem salvas no banco de dados.

O sistema foi construído utilizando uma abordagem clássica de aplicações monolíticas PHP, garantindo simplicidade, eficiência e um desenvolvimento rápido para validação do produto para o público externo e captura dos dados iniciais


## Arquitetura experimental

O desenvolvimento do RecomendeMe seguiu uma abordagem experimental e iterativa, testando diferentes tecnologias e arquiteturas antes de consolidar a versão atualmente em produção. Esse processo foi essencial para validar a viabilidade do projeto, garantindo que a plataforma atendesse às necessidades dos usuários da maneira mais eficiente possível. Por meio de provas de conceito e mvp




# Divisão de Módulos Experimentais

O Sistema do RecomendeMe Experimental está dividido em 5 partes sendo 4 dessas partes conectadas em uma arquitetura modular (Mobile Interface, ACDC, API, Data) e outra independente servindo com um mvp de validação  de tecnologia feito em ruby on rails.

- RecomendeMe Mobile Interface (React Native)
- RecomendeMe ACDC Microservice - (Flask  & MySQL)
- RecomendeMe API(Node.Js & MySql)
- RecomendeMe Data(Mysql, Sqlite)
- RecomendeMe Monolith Backend(Ruby on rails, sqlite3)

A divisão de módulos experimentais permitiu uma validação da viabilidade técnica do produto em termos de escalabilidade e adoção de tecnologia. Foi importante inicialmente, pois por razões de estratégia o RecomendeMe como ideia não poderia depender de um tecnologia ou linguagem em especifico. Da parte do servidor, cada um ficou isolado e testados em grupos especificos de usuários, o módulo de álbum foi o mais testado entre todos esses. Para teste, foi necessário criar um sistema de tunelamento com o Ngrok e disponibilizar o link em grupos especificos. 



Cada módulo experimental possui uma documentação associada para que os desenvolvedores e contribuidores entendam melhor o funcionamento e lógica do sistema como um todo 
