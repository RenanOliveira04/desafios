# Sistema Bancário em Python

Este é um projeto de sistema bancário desenvolvido em Python que utiliza conceitos de programação orientada a objetos, como herança, polimorfismo e classes abstratas. 

## Funcionalidades

O sistema possui as seguintes funcionalidades principais:

- Criação de contas bancárias (conta corrente) 
- Realização de transações bancárias, como saques e depósitos 
- Registro de histórico de transações 
- Limite de saques e verificação de saldo 

## Estrutura do Projeto

O projeto é composto pelas seguintes classes principais:

- `Cliente`: Representa um cliente do banco, contendo informações como endereço e lista de contas. 
- `PessoaFisica`: Herda da classe `Cliente` e adiciona atributos específicos para pessoas físicas, como nome, data de nascimento e CPF. 
- `Conta`: Classe base para representar uma conta bancária, contendo atributos como número, agência, cliente e histórico de transações. 
- `ContaCorrente`: Herda da classe `Conta` e adiciona funcionalidades específicas para contas correntes, como limite de saque e limite de saques diários.
- `Historico`: Representa o histórico de transações de uma conta, armazenando informações como tipo de transação, valor e data. 
- `Transacao`: Classe abstrata base para representar uma transação bancária, contendo métodos abstratos para valor e registro da transação. 
- `Saque` e `Deposito`: Classes que herdam de `Transacao` e implementam os métodos abstratos para representar transações de saque e depósito, respectivamente. 

## Utilização do Módulo ABC

O projeto utiliza o módulo `abc` (Abstract Base Classes) do Python para definir classes abstratas e métodos abstratos. 

- A classe `Transacao` é definida como uma classe abstrata base utilizando a metaclasse `ABC`. 
- Os métodos `valor` e `registrar` são decorados com `@abstractmethod` para indicar que são métodos abstratos e devem ser implementados pelas classes derivadas. 

## Como Executar o Projeto

Para executar o projeto, siga os passos abaixo:

1. Certifique-se de ter o Python instalado em sua máquina.
2. Faça o download dos arquivos do projeto ou clone o repositório.
3. Abra um terminal ou prompt de comando e navegue até o diretório do projeto.
4. Execute o arquivo principal do projeto utilizando o comando `python desafio.py`.

## Contribuição

Contribuições para o projeto são bem-vindas. Se você encontrar algum problema, tiver sugestões de melhorias ou quiser adicionar novos recursos, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto está licenciado sob a [MIT]. Consulte o arquivo `LICENSE` para obter mais informações. 
