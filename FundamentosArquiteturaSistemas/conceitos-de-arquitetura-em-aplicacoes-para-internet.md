# Conceitos de Arquitetura em Aplicações para Internet

### Introdução à Arquitetura de Sistemas

##### Tipos de Arquitetura

- Monolito: Aplicações únicas (Proxy se conecta às instâncias da aplicação e às instâncias se conectam ao banco de dados)
- Microserviços: A aplicação é separada em pequenos serviços. (Há 3 tipos de microserviços)


### Comparando os modelos Monolito e Microsserviços

##### Monolito
Pros
- Baixa complexidade
- Monitoramento simplificado

Contras 
- Stack única 
- Compartilhamento de recursos
- Acoplamento
- Mais complexo a escalabilidade

##### Microserviços #1
Pros
- Stack dinâmica
- Simples escalabilidade

Contras
- Acoplamento
- Monitoramento mais complexo
- Provisionamento mais complexo

##### Microserviços #2
Pros
- Stack dinâmica
- Simples escalabilidade
- Desacoplamento

Contras
- Monitoramento mais complexo
- Provisionamento mais complexo

##### Microserviços #3
Pros
- Stack dinâmica
- Simples escalabilidade
- Desacoplamento
- Menor complexidade

Contras
- Provisionamento mais complexo
- Plataforma inteira depende do gerenciador de pipeline.


### Gerenciamento d erros e volume de acesso
