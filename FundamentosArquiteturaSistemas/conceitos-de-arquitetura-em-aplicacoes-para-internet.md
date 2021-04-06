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


### Gerenciamento de erros e volume de acesso

É mais complexo em processos assíncronos e em pipelines.

No primeiro, pois não há rollback e o erro acaba ficando isolado.
No segundo, pois além de fazer o rollback do próprio passo deve-se fazer o rollback dos passos anteriores.

Solução: Dead letter queue ou Filas de re-tentativas (O que deu erro é enviado de volta para a fila para ser reprocessado).