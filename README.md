# agenda-zap-embed-sample
Exemplo de uso de embed da plataforma agenda-zap.com

## Como criar uma conta no Agenda Zap

1. Acesse o site [Agenda Zap](https://agenda-zap.com/).
2. Clique no botão "Criar Conta" no canto superior direito.
3. Preencha o formulário de cadastro com suas informações pessoais.
4. Confirme seu e-mail através do link enviado para sua caixa de entrada.

## Como criar uma organização no Agenda Zap

1. Após fazer login, clique no menu "Organizações" no painel de controle.
2. Clique no botão "Nova Organização".
3. Preencha o formulário com as informações da sua organização.
4. Clique em "Salvar" para criar a organização.

## Como obter o slug da organização

1. No painel de controle, clique na organização que você criou.
2. O slug da organização estará disponível na URL do navegador, após `/organizations/`.

## Como adicionar o botão de agendamento no seu site

Para adicionar o botão de agendamento do Agenda Zap no seu site, siga os passos abaixo:

1. Adicione o seguinte script no `<head>` ou no final do `<body>` do seu site:
   ```html
   <script src="https://agenda-zap.com/embed.js"></script>
   ```

2. Adicione o botão onde desejar, substituindo `<slug-da-organização>` pelo slug da sua organização:
   ```html
   <button data-agenda-zap-slug="<slug-da-organização>">Agendamento</button>
   ```

Exemplo de código completo:
```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Agenda Zap | Exemplo de Embed</title>
    <script src="https://agenda-zap.com/embed.js"></script>
  </head>
  <body>
    <!-- Adicione o botão onde desejar -->
    <button data-agenda-zap-slug="demo">Agendamento</button>
  </body>
</html>
```

Para mais informações, acesse o site do [Agenda Zap](https://agenda-zap.com).
