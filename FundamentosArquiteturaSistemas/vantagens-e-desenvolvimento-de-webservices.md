# Vantagens e desenvolvimento de Web Services

### O que são Web Services

##### WebServices
São soluções que permitem aplicações se comunicarem independentemente da linguagem, software ou hardware utilizados. A comunicação é feita através da web por meio de protocolos HTTP. (Todo WebService é uma API mas nem toda API é um WebService, porque uma API pode ter outros protocolos).

##### Vantagens
- Linguagem única comum às aplicaões
- Integração
- Reutilização de implemetação
- Segurança
- Menor custo (Manutenção e Desenvolvimento)

##### Tecnologias mais utilizadas
.
| Tecnologia | Característica |
| ------ | ------ |
| SOAP | Protocolo para troca de informações baseado em XML |
| REST | Princípios de arquitetura pelos quais os dados podem ser transmitidos |
| XML | Linguagem de marcação |
| JSON | Notação utilizada para estruturar dados baseada em JavaScript  |
```sh
# XML exemplo
    <endereco>
        <cep>9999-999</cep>
        <bairro>Jd. Boa Vista</bairro>
        <logradouro>Av. Paulista</logradouro>
        <cidade>São Paulo</cidade>
        <numero>99</numero>
    </endereco>
    
# JSON exemplo
{    
    "endereco": {
        "cep": "9999-999",
        "bairro": "Jd. Boa Vista",
        "logradouro": "Av. Paulista",
        "cidade": "São Paulo",
        "numero": 99
    }
}
```

### Estrutura SOAP

##### O que é SOAP

Simple Object Access Protocol
É um protocolo, baseado em XML, que visa facilitar as integrações entre aplicações.
Pode-se dizer que SOAP é uma definição de como serviços web se comunicam.

##### As vantagens de se utilizar SOAP

- Utiliza uma linguegem comum, XML, permitindo integração entre aplicações em diferentes linguagens. 
- É independente de plataforma e software.
- Meio de transporte genérico, ou seja, pode ser usado por outros protocolos além do HTTP.

##### O que é XML

Extensible Markup Language
Criada pela W3C, com o objetivo de padronizar a web. Essa linguagem tem como principal caracterísica ser universal, podendo ser integrada em diversas aplicações.

##### Entendendo a estrutura de uma mensagem SOAP 

SOAP Envelope: Encapsula toda a mensagem SOAP. 
SOAP Header: Gerencia os atributos e metadados da requisição.
SOAP Body: Contém a mensagem em si.
```sh
# SOAP exemplo
<soap:Envelope xmlns:soap="url">
    <soap:Header>
    </soap:Header>
    <soap:Body>
        <m:endereco>
            <m:cep>9999-999</m:cep>
            <m:bairro>Jd. Boa Vista</m:bairro>
            <m:logradouro>Av. Paulista</m:logradouro>
            <m:cidade>São Paulo</m:cidade>
            <m:numero>99</m:numero>
        </m:endereco>
     </soap:Body>
</soap:Envelope>
```

### Entendendo o que é WSDL e XSD

##### O que é um WSDL

Web Services Descripion Language (WSDL)
Usado para descrever WebServices, funciona como um contrato do serviço.
A descrição pe feito em um documento XML, onde é descrito o serviço, especificações de acesso, operações e métodos.

##### O que é um XSD

XML Schema Deinition (XML)
É um schema no formato XML usado para difinir a estrutura de dados que será validada no XML
O XSD funciona como uma documentação de como deve ser montado o SOAP Message (XML), que será enviado atrvés de WebService.

### Aprenda o que são REST, API e JSON

##### REST

###### O que é?
Representational State Transfer.
Representa o estado do objeto no momento da transferência.
Diferente do SOAP que é um protocolo o REST é um estilo de arquitetura para implementação de serviços web.

###### Vantagens
1. Permite a integração entre sistemas e entre clientes e servidor.
2. Utiliza os métodos HTTP.
3. Arquitetura simples.

###### Estrutura do REST
Cliente manda uma requisição HTTP
Servidor retorna um código de operação e uma mensagem.

##### API
Application Programming Interface.
São um conjunto de métodos disponibilizados por uma aplicação para que outra possa usufruir de suas funcionalidades.

###### Principais métodos HTTP
- GET: Solicita a representação de um recurso.
- POST: Solicita a criação de um recurso.
- DELETE: Solicita a exclusão de um recurso.
- PUT: Solicita a atualização de um recurso.

##### JSON
JavaScript Object Notation
Notação para estruturar dados na troca de mensagens entre sistemas.
Tem uma estrutura chave-valor.

### Veja sobre integração com REST e métodos HTTP na prática

##### Códigos de Estado/Status
Usado para informar o cliente sobre a reposta do servidor.
- 1XX - INFORMATIVO
- 2XX - SUCESSO
- 3XX - REDIRECIONAMENTO
- 4XX - ERRO NO CLIENTE
- 5XX - ERRO NO SERVIDOR

