# Resumo sobre Contas de Armazenamento no Azure

As contas de armazenamento no Azure oferecem uma maneira de armazenar dados acessíveis e escaláveis na nuvem. Elas suportam diferentes tipos de armazenamento, como blobs, tabelas, filas e arquivos. Dependendo das necessidades, é possível escolher entre diferentes níveis de desempenho, redundância e opções de proteção de dados.

### Tipos de Armazenamento
- **Blobs**: Ideal para armazenar grandes quantidades de dados não estruturados.
- **Tabelas**: Oferecem uma maneira de armazenar dados estruturados como um banco de dados NoSQL.
- **Filas**: Permitem comunicação assíncrona entre diferentes componentes de uma aplicação.
- **Arquivos**: Oferecem um compartilhamento de arquivos totalmente gerenciado na nuvem, acessível por protocolos SMB.

---

## Passos para Criar uma Conta de Armazenamento no Azure

1. **Acesse o Portal do Azure**: Navegue até [https://portal.azure.com](https://portal.azure.com) e faça login.
   
2. **Criar um Grupo de Recursos**:
   - No menu à esquerda, selecione **Grupos de Recursos** e clique em **Criar**.
   - Nomeie o grupo de recursos como `AZ-900-LAB_Armazenamento` e escolha uma região adequada.
   - Clique em **Revisar + Criar** e depois em **Criar**.

3. **Criar uma Conta de Armazenamento**:
   - No portal, clique em **Criar um recurso** e procure por **Conta de Armazenamento**.
   - Selecione **Conta de armazenamento (geral)** e clique em **Criar**.
   - Escolha o grupo de recursos **AZ-900-LAB_Armazenamento**.
   - Nomeie a conta como `sto-dio-armazenamento-azure-lab`.
   - **Desempenho**: Selecione `Standard`.
   - **Redundância**: Escolha `Locally-redundant storage (LRS)`.
   - Para a seção de **Proteção de Dados**, desabilite as opções de **Recuperação de Soft Delete** e outras opções de recuperação.
   - Mantenha as outras configurações como padrão e clique em **Revisar + Criar**.
   - Após a validação, clique em **Criar**.

---

## Criando Compartilhamento de Arquivos

1. No menu da conta de armazenamento, selecione **File shares**.
2. Clique em **+ File share**.
3. Nomeie o compartilhamento de arquivos e defina a cota de armazenamento, se necessário.
4. Clique em **Criar**.

---

## Criando Filas

1. No menu da conta de armazenamento, selecione **Queues**.
2. Clique em **+ Queue**.
3. Nomeie a fila (por exemplo, `queue-lab`).
4. Clique em **OK**.

---

## Criando Tabelas

1. No menu da conta de armazenamento, selecione **Tables**.
2. Clique em **+ Table**.
3. Nomeie a tabela (por exemplo, `table-lab`).
4. Clique em **OK**.

---

# Resumo sobre Projeto de Migração no Azure

Um projeto de migração no Azure envolve mover recursos e dados de um ambiente existente para o Azure, utilizando as ferramentas e serviços oferecidos pela plataforma para garantir que a migração seja eficiente e sem interrupções.

## Etapas de Criação de um Projeto de Migração

1. **Planejamento da Migração**:
   - Defina o escopo do projeto, incluindo quais cargas de trabalho serão migradas.
   - Avalie o ambiente atual e identifique os recursos que precisam ser migrados.
   - Escolha as ferramentas de migração adequadas (Azure Migrate, Database Migration Service, etc.).

2. **Configurar o Azure Migrate**:
   - No portal do Azure, vá para **Azure Migrate**.
   - Crie um novo **Projeto de Migração** e escolha a assinatura e o grupo de recursos.
   - Defina o nome do projeto e escolha a região onde será configurado.

3. **Descoberta e Avaliação**:
   - Baixe e instale os appliances de descoberta no ambiente local (se necessário).
   - Execute a **descoberta** do ambiente atual para obter informações sobre o estado dos recursos.
   - Avalie os dados para entender os requisitos de migração e dimensionamento de recursos no Azure.

4. **Preparação para a Migração**:
   - Após a avaliação, prepare o ambiente Azure (criação de redes, configuração de recursos, etc.).
   - Use as ferramentas de replicação de dados para mover os dados e recursos para o Azure.

5. **Executar a Migração**:
   - Inicie a migração utilizando as ferramentas escolhidas (VM, banco de dados, aplicativos, etc.).
   - Acompanhe o progresso da migração no painel do **Azure Migrate**.

6. **Validação Pós-Migração**:
   - Teste os recursos migrados para garantir que tudo esteja funcionando corretamente.
   - Monitore o desempenho e ajuste a escala dos recursos conforme necessário.
   - Desative os recursos no ambiente de origem, caso não sejam mais necessários.
