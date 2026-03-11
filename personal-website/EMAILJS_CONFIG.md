# Configuração EmailJS - AU-Ê Pet Care

## 🚀 Configuração Rápida (Já está pronta!)

O EmailJS já está configurado no arquivo `index.html`. Veja o código:

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
<script type="text/javascript">
    (function() {
        console.log('🔧 Inicializando EmailJS...');
        emailjs.init("g7uF0Elsr-_HOn0ck"); // Chave pública já configurada
        console.log('✅ EmailJS inicializado com sucesso!');
        console.log('🔑 Chave: g7uF0Elsr-_HOn0ck');
    })();
</script>
```

## 📧 Configurações de Envio

### Service ID e Template ID:
- **Service ID:** `service_1wwk81o`
- **Template ID:** `template_p7wp6qq`
- **Email Destino:** `aue.petcare@gmail.com`

## 📋 Tipos de Emails Enviados

### 1. Cadastro de Pet
**Assunto:** `🐕 NOVO CADASTRO - [Nome do Pet]`

**Campos enviados:**
- `tutor_name` - Nome do tutor
- `tutor_phone` - Telefone
- `tutor_email` - Email
- `tutor_cpf` - CPF
- `pet_name` - Nome do pet
- `pet_age` - Idade
- `pet_breed` - Raça
- `pet_gender` - Sexo (macho/fêmea)
- `pet_neutered` - Castrado (sim/não)
- `pet_temperament` - Temperamento
- `service` - Serviço selecionado
- `registration_date` - Data do cadastro
- `message` - Mensagem automática

### 2. Agendamento de Visita
**Assunto:** `📅 NOVA VISITA AGENDADA - [Nome do Cliente]`

**Campos enviados:**
- `tutor_name` - Nome do cliente
- `tutor_phone` - Telefone
- `tutor_email` - Email
- `service` - "Visita Presencial"
- `registration_date` - Data do agendamento
- `message` - Data, horário e mensagem

### 3. Solicitação de Serviço
**Assunto:** `🐕 NOVA SOLICITAÇÃO - [Tipo de Serviço]`

**Campos enviados:**
- `tutor_name` - Nome do tutor
- `tutor_phone` - Telefone
- `tutor_email` - Email
- `tutor_cpf` - CPF
- `pet_name` - Nome do pet
- `pet_age` - Idade
- `pet_breed` - Raça
- `service` - Tipo de serviço
- `registration_date` - Data da solicitação
- `message` - Detalhes do serviço

## 🎯 Fluxo de Funcionamento

### Para Cadastro de Pet:
1. Cliente preenche formulário completo
2. Clique em "Cadastrar Pet"
3. Email enviado automaticamente
4. Modal WhatsApp aparece
5. Cliente envia documentos via WhatsApp

### Para Agendamento de Visita:
1. Cliente clica em "Agendar Visita"
2. Preenche formulário (nome, telefone, email, data, horário)
3. Clique em enviar
4. Email enviado automaticamente
5. Alerta de confirmação exibido

### Para Solicitação de Serviço:
1. Cliente escolhe serviço (Creche, Hotel, etc.)
2. Preenche formulário no modal
3. Clique em enviar
4. Email enviado automaticamente
5. Modal fecha e alerta exibido

## ✅ Verificação de Funcionamento

Para testar se está tudo funcionando:

1. **Abra o console do navegador** (F12)
2. **Preencha qualquer formulário**
3. **Veja as mensagens no console:**
   - `🔧 Inicializando EmailJS...`
   - `✅ EmailJS inicializado com sucesso!`
   - `📧 Enviando email...`
   - `✅ Email enviado com sucesso!`

## 🔧 Resolução de Problemas

### Se o email não chegar:

1. **Verifique a chave pública:**
   - Acesse: https://dashboard.emailjs.com/admin/account
   - Copie a "Public Key"
   - Substitua no código: `emailjs.init("SUA_CHAVE_AQUI")`

2. **Verifique o Service ID:**
   - Acesse: https://dashboard.emailjs.com/admin/services
   - Confirme se `service_1wwk81o` está ativo

3. **Verifique o Template ID:**
   - Acesse: https://dashboard.emailjs.com/admin/templates
   - Confirme se `template_p7wp6qq` existe

4. **Verifique o email de destino:**
   - O email `aue.petcare@gmail.com` está configurado
   - Verifique a caixa de spam/lixo eletrônico

## 📱 Estrutura dos Dados no Email

Cada email enviado contém:

```
Para: aue.petcare@gmail.com
Assunto: 🐕 NOVO CADASTRO - Rex

Corpo do email:
- Nome do Tutor: João Silva
- Telefone: (11) 99999-9999
- Email: joao@email.com
- Nome do Pet: Rex
- Raça: Golden Retriever
- Idade: 3 anos
- Serviço: Creche
- Data: 10/03/2026 14:30
```

## 🎨 Template do EmailJS

Para criar um template personalizado no EmailJS:

1. Acesse: https://dashboard.emailjs.com/admin/templates
2. Crie novo template
3. Use estas variáveis:

```html
<h2>Novo Cadastro - {{pet_name}}</h2>
<p><strong>Tutor:</strong> {{tutor_name}}</p>
<p><strong>Telefone:</strong> {{tutor_phone}}</p>
<p><strong>Email:</strong> {{tutor_email}}</p>
<p><strong>Pet:</strong> {{pet_name}}</p>
<p><strong>Raça:</strong> {{pet_breed}}</p>
<p><strong>Idade:</strong> {{pet_age}}</p>
<p><strong>Sexo:</strong> {{pet_gender}}</p>
<p><strong>Castrado:</strong> {{pet_neutered}}</p>
<p><strong>Temperamento:</strong> {{pet_temperament}}</p>
<p><strong>Serviço:</strong> {{service}}</p>
<p><strong>Data:</strong> {{registration_date}}</p>
<hr>
<p>{{message}}</p>
```

## 🆘 Suporte

Se precisar de ajuda:
- Email: aue.petcare@gmail.com
- WhatsApp: (11) 99575-5021
- Documentação EmailJS: https://www.emailjs.com/docs/

---
**AU-Ê Pet Care - Sistema 100% funcional! 🐾✨**
