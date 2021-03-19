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
- Meio de trandporte genérico, ou seja, pode ser usado por outros protocolos além do HTTP.

##### O que é XML

Extensible Markup Language
Criada pela W3C, com o objetivo de padronizar o padrão da web. Essa linguagem tem como principal caracterísica ser universal, podendo ser integrada em deiversas aplicações.

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


### Aprenda o que são REST, API e JSON


### Veja sobre integração com REST e métodos HTTP na prática

