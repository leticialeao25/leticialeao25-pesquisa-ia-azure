📌 Configuração de Laboratório no Azure

Este repositório contém instruções detalhadas para a criação e configuração de um laboratório no **Microsoft Azure**. O objetivo é criar três recursos essenciais para extrair dados de uma fonte de dados e realizar buscas utilizando **Azure AI Search**.

---

## 📋 Pré-requisitos

Antes de iniciar, certifique-se de ter:

- Uma conta no [Microsoft Azure](https://portal.azure.com/)
- Permissões para criar e gerenciar recursos no Azure
- Conhecimento básico sobre serviços de **IA**, **Armazenamento** e **Pesquisa** no Azure

---

## 🛠 Passo a Passo

### 1️⃣ Criando um Recurso do Azure AI Search

1. Acesse o portal do Azure: [Clique aqui](https://portal.azure.com/#view/Microsoft_Azure_ProjectOxford/CognitiveServicesHub/~/overview)
2. No menu lateral esquerdo, clique em **+ Criar um Recurso** e depois em **Introdução**.
3. Na barra de pesquisa, procure por **AI Search**.
4. Selecione a opção correspondente e clique em **Criar Recurso**.
5. Preencha os campos obrigatórios:
   - Escolha uma assinatura e um grupo de recursos.
   - Configure a localização e o tipo de precificação.
6. Clique em **Criar**.

### 2️⃣ Criando um Recurso do Azure AI Services

1. No menu lateral esquerdo, clique em **+ Criar um Recurso**.
2. Vá para **IA Machine Learning** > **Azure IA Services** > **Criar Recurso**.
3. Configure as informações solicitadas:
   - Escolha uma assinatura e um grupo de recursos.
   - Defina a localização e o tipo de precificação.
4. Finalize clicando em **Criar**.

### 3️⃣ Criando um Recurso do Azure Storage Accounts

1. Acesse **Storage Accounts** na página inicial do Azure.
2. Clique em **Criar**.
3. Preencha os dados necessários:
   - Escolha uma assinatura e um grupo de recursos.
   - Configure a localização e o tipo de precificação.
4. Clique em **Criar**.

📌 **Configuração Adicional:**
- Acesse **Storage Accounts** e vá até **Configuração**.
- Habilite **Allow anonymous access to the Blob**.
- Salve as alterações.

### 📂 Enviando Arquivos para o Storage

1. Acesse **Storage Accounts** > **Armazenamento de Dados**.
2. Selecione **Contêineres** e clique em **+ Contêineres**.
3. Defina um nome e clique em **Criar**.

### 🔎 Indexando Documentos no Azure AI Search

1. Acesse **Azure AI Services** e clique em **AI Search**.
2. Selecione o recurso criado e clique em **Importar Dados**.
3. Escolha **Armazenamento de Blob do Azure** e selecione a conexão criada.
4. Clique em **Criar Indexador** e nomeie como `coffee-indexer`.
5. Defina a execução como **Uma vez** e clique em **Enviar**.
6. Vá até **Search Management > Indexers** e atualize a página até o status ser **Sucesso**.

### ✅ Testando Consultas com o Search Explorer

- Acesse **Search Explorer** no portal do Azure.
- Escreva consultas para validar a indexação.
- Analise os resultados no formato **JSON**.
