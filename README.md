# Event Registration Service

Este repositório contém um microserviço dedicado ao cadastro de eventos. Ele se integra perfeitamente com o [Email Service Desafio Uber](https://github.com/WesleyS08/Email-Service-Desafio_Uber), permitindo o envio automático de e-mails para os participantes registrados.

## Principais Recursos

- **Cadastro de Eventos:** Fornece uma API para cadastrar novos eventos, incluindo detalhes como título, data e descrição.

- **Integração com E-mail:** Comunica-se com o serviço de e-mail (por exemplo, Amazon SES) para enviar e-mails de confirmação e lembretes aos participantes registrados.

- **Configuração Flexível:** Personalize as configurações do serviço, incluindo a mensagem de confirmação e lembrete, através do arquivo de configuração.

## Como Usar

1. **Configuração:**
   - Clone este repositório.
   - Execute `npm install` para instalar as dependências.
   - Configure as credenciais e as configurações de e-mail no arquivo `config.json`.

2. **Execução:**
   - Inicie o serviço com `npm start`.
   - Acesse a API para cadastrar novos eventos.

3. **Cadastro de Eventos:**
   - Utilize a API do serviço para cadastrar novos eventos, fornecendo informações como título, data, localização e descrição.

## Configuração do Arquivo `config.json`
```json
{
  "emailService": {
    "apiEndpoint": "http://endereco-api-email-service"
  },
  "eventConfirmationMessage": "Obrigado por se cadastrar em nosso evento!",
  "eventReminderMessage": "Lembrete: Nosso evento está chegando! Não esqueça de participar!"
}
