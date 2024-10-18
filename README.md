# Projeto - Formulário de cadastro completo
 
# 📍 Cadastro de Endereço

Este projeto contém um formulário para cadastro de endereço de usuários, permitindo a coleta de informações essenciais para cadastro e localização.

## Estrutura do Formulário

O formulário inclui os seguintes campos:

- **Nome**: Campo obrigatório para inserir o nome do usuário.
- **Email**: Campo obrigatório para o email do usuário.
- **Senha**: Campo obrigatório para criar uma senha.
- **CPF**: Campo obrigatório para o Cadastro de Pessoa Física.
- **Data de Nascimento**: Campo obrigatório para informar a data de nascimento.
- **CEP**: Campo obrigatório para o Código de Endereçamento Postal.
- **Logradouro**: Campo opcional para a rua.
- **Número**: Campo opcional para o número da residência.
- **Bairro**: Campo opcional para o bairro.
- **Complemento**: Campo opcional para informações adicionais.
- **Cidade**: Campo opcional para a cidade.
- **Estado**: Campo opcional para o estado.

## Tecnologias Utilizadas

- **HTML**: Estrutura básica do formulário.
- **CSS**: Estilização através do arquivo `main.css`.
- **JavaScript**: Lógica de interação no arquivo `main.js`.

## Responsividade

O design do formulário é responsivo, adaptando-se a diferentes tamanhos de tela, graças à configuração do `meta viewport`.

## Como Usar

1. Clone o repositório.
2. Abra o arquivo `index.html` em um navegador.
3. Preencha os campos do formulário e clique em "Enviar".

## Contribuição

Sinta-se à vontade para contribuir com melhorias ou correções. Faça um fork do repositório e envie suas sugestões!

# Explanação do codigo
 
1.  Inicio:
    > - 'use strict'; ativa um modo de programação que evita erros comuns, garantindo que o código seja mais seguro.
 
2. Função limparFormulario:
 
    > Limpa os campos do formulário de endereço ao definir seus valores como vazios, utilizando getElementById.
 
3. Validação do CEP:
 
    > - Função eNumero: Verifica se o valor contém apenas dígitos numéricos usando uma expressão regular.
    >
    > - Função cepValido: Confirma se o CEP possui exatamente 8 dígitos e é numérico.
 
4. Função preencherFormulario:
 
    > Recebe um objeto endereco e preenche os campos do formulário com os dados correspondentes, como logradouro e bairro.
 
5. Função pesquisarCep:
 
    >- Assíncrona: Utiliza async/await para lidar com a API.
    >
    > - Limpa o formulário e monta a URL da requisição.
    >
    > - Verifica se o CEP é válido, faz uma requisição à API viaCep, e trata a resposta convertendo-a para JSON.
    > - Se o CEP não for encontrado, exibe um alerta; caso contrário, preenche o formulário.
 
6. Escutador de Evento:
 
    > - addEventListener é usado para chamar a função pesquisarCep quando o usuário sai do campo CEP (evento focusout: O evento focusout é acionado assim que o elemento perde o foco, no caso quando o usuário sai do campo de texto).
 
7. Validar Cpf
 
    > Valida se o formato digitado no cpf é correto
 
8. Validar Email
 
    >Valida se o formato digitado no Email é correto
 
 # Atributos diferenciais no codigo javaScript
 - 'async function: A async function define uma função assíncrona que produz um objeto do tipo AsyncFunction. Este recurso é empregado em JavaScript para facilitar o gerenciamento de operações assíncronas, permitindo que o código se assemelhe a um fluxo síncrono.

- 'const: A palavra-chave const declara uma variável que não pode ser reatribuída, ou seja, é uma constante. Isso não implica que o valor da variável seja imutável; por exemplo, se o valor for um objeto, suas propriedades podem ser modificadas, mas a referência da variável em si não pode ser alterada.

- 'await: Ao usar await, o JavaScript suspende a execução da função assíncrona até que a Promise correspondente seja resolvida. Se a Promise for concluída com êxito, o valor resultante é retornado.

- 'hasOwnProperty: O método hasOwnProperty() fornece um valor booleano que indica se um objeto contém a propriedade especificada como uma propriedade direta (definida no próprio objeto), em contraste com propriedades que possam ser herdadas de sua cadeia de protótipos.

# ⚙️ Como Usar
 
Digite o CEP no campo correspondente.
O formulário será automaticamente preenchido com as informações do endereço.
 
Caso o CEP não seja encontrado ou seja inválido, uma mensagem de alerta será exibida.
 
# 🧮 Tecnologias Utilizadas
 
- HTML
 
- CSS
 
- JavaScript
 
- API ViaCEP
 
- Com apoio do chat GPT

# 📝 Fontes
 
[ViaCEP](https://viacep.com.br/)
 
>foi usado o formato JSON para o projeto
 
[Mozilla](https://developer.mozilla.org/pt-BR/)
