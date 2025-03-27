# Projeto_ControleDOCS

# 📲 App de Gestão de Documentos Internos – AppSheet

Este é um aplicativo desenvolvido na plataforma **AppSheet**, com integração ao **Google Sheets**, para controle de **documentos recebidos, entregues e rastreados por setores** dentro de uma organização.

---

## 🎯 Objetivo

O sistema foi criado para otimizar o **controle de entrega de documentos físicos e digitais** entre áreas internas, registrando todas as etapas com segurança, rastreabilidade e assinaturas digitais.

---

## ⚙️ Funcionalidades

- ✅ Registro de recebimento e entrega de documentos
- 🧾 Cadastro de destinatário, setor e código de rastreio
- 🗂️ Classificação por tipo de documento (contrato, boleto, nota fiscal, etc.)
- 🖋️ Assinatura digital no momento da retirada
- 📸 Captura de imagem do documento como comprovante
- 🧑‍💻 Registro automático do colaborador responsável (via login)
- 📅 Registro automático de data e hora da entrega (`NOW()`)
- 🔍 Filtros por status: “Em Aberto” e “Entregues”
- 📬 Gatilho de e-mail automático com comprovante para quem retirou
- 📱 Interface mobile e web responsiva

---

## 🧱 Estrutura da Planilha (Google Sheets)

| Coluna                   | Tipo         | Descrição                                |
|--------------------------|--------------|-------------------------------------------|
| ID                       | Texto        | Código identificador do documento         |
| Destinatário             | Texto        | Pessoa ou setor que receberá o documento  |
| Setor / Área             | Enum         | Área responsável (Financeiro, RH, etc.)   |
| Cod Rastreio             | Texto        | Código de rastreamento (Correios etc.)    |
| Data Recebimento         | Data         | Quando o documento foi recebido           |
| Remetente                | Texto        | Quem enviou o documento                   |
| Tipo DOC                 | Enum         | Tipo do documento                         |
| Data Entrega             | DateTime     | Data e hora da entrega ao responsável     |
| Colaborador Responsável  | Texto        | Quem fez a entrega (via USEREMAIL)        |
| Assinatura de Retirada   | Signature    | Assinatura digital de quem retirou        |
| Foto DOC                 | Imagem       | Foto do documento entregue                |
| Observações              | LongText     | Anotações gerais                          |

---

## 🧠 Tecnologias Utilizadas

- [AppSheet](https://www.appsheet.com/)
- [Google Sheets](https://sheets.google.com)
- Workflow e Automations (AppSheet Bots)
- Expressões: `NOW()`, `USEREMAIL()`, `ISBLANK()`, `ISNOTBLANK()`

---

## 🚀 Como testar

> O app está disponível para demonstração.  
> ⚠️ Versão com dados fictícios e restrição de edição.

🔗 [Clique aqui para acessar o app (modo visualização)](https://www.appsheet.com/start/4df444b9-300c-40b5-acb4-d09118031a03) (Versão Navegador)

🔗 [Clique aqui para acessar o app (modo visualização)](https://www.appsheet.com/newshortcut/4df444b9-300c-40b5-acb4-d09118031a03) (Versão Mobile)

---

## 📦 Arquivo Base

- [📄 Planilha Google Sheets - Estrutura de dados](https://docs.google.com/spreadsheets/d/1Or8_8FbNJc4YxfVkBQVNGU650SRVYsovCpq90rtubrw/edit?usp=sharing)

---

## ✍️ Autor

**João Marcos Guilherme**  
📍 São Paulo - SP  
📧 joaomguilherme@icloud.com  
🔗 [LinkedIn](https://www.linkedin.com/in/jmguilherme/)
