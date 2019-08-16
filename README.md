# mps_LaboratorioExcecoes
Laboratório para a cadeira de métodos de projetos de software.

Laboratório de Exceções   1 - Crie um projeto de um programa em Java e divida-o em três pacotes: 
    a) camada que lida com a interface com o usuário (view);
    b) camada de negócio (business) com dois pacotes;
        b.1) subcamada que possui regras (gerente de usuário) de negócio (control)
        b.2) subcamada que possui entidades do negócio (model)
    c) camada que lida com a persistência/comunicação externa/etc (infra).
        
2 - Implemente a ADIÇÃO DE USUÁRIOS no sistema e, na camada " business.control", algoritmos para validar os cadastros de usuários. Crie e utilize exceções próprias para representar os erros abaixo:   

Login:     
    máximo 12 caracteres
        não pode ser vazio
        não pode ter números //  strWithNumber.matches(?.*\\d.*?)

Senha:         
    máximo 16 caracteres
    mínimo de 8 caracteres
    deve possuir letras e números e ao menos 2 números.

Dica: Pesquise o método matches da classe String ou os métodos da classe Character

3 - Armazene os usuários numa coleção (deve ser atributo da classe que gerencia os usuários na camada "control") e implemente a persistencia da lista utilizando arquivos binários na camada "infra") 

4 - Implemente a EXCLUSÃO DE UM USUÁRIO dado seu login.

5- Realize o tratamento de exceções em dois níveis: Capture as exceções java.io.IOExpcetion na camada "infra", relance-as (usando as exceções criadas na questão 2) para as camadas acima de modo que apresente uma mensagem para o usuário final amigável.
