# Gestão de Políticas de Acesso no Azure

A gestão de políticas de acesso no Azure envolve o controle e a definição de quem pode acessar e manipular recursos dentro de um ambiente Azure. O Azure fornece mecanismos de controle detalhado por meio do **Entra ID** e das **políticas de controle de acesso baseado em funções (RBAC)**.

## Etapas para Criar Políticas de Acesso no Azure

1. **Definir o Escopo**: Selecione o escopo da política, que pode ser atribuído ao nível de assinatura, grupo de recursos ou recursos individuais.
   
2. **Criar uma Nova Função ou Usar Funções Padrão**: Use uma função predefinida, como Administrador ou Leitor, ou crie uma função personalizada com permissões específicas.

3. **Atribuir Funções aos Usuários ou Grupos**: Atribua a função apropriada a usuários, grupos ou identidades de serviço, especificando o nível de acesso necessário.

4. **Aplicar Restrições com Políticas de Acesso**: Use as **Azure Policies** para impor requisitos como o uso de recursos específicos (ex. tipos de VMs) e garantir a conformidade com políticas de segurança.

5. **Monitorar e Auditar Acessos**: Utilize o Azure Monitor e o Azure Security Center para acompanhar logs de atividade e eventos relacionados ao gerenciamento de políticas de acesso.

## Contas no Microsoft Purview

O **Microsoft Purview** é uma solução de governança de dados que ajuda as empresas a gerenciar, proteger e auditar seus dados em vários ambientes, incluindo o Azure. Para criar contas no Microsoft Purview:

1. **Acessar o Portal do Azure**: Navegue até o portal do Azure e vá até o Microsoft Purview.
   
2. **Criar uma Conta de Governança de Dados**: Selecione **Criar novo recurso**, escolha **Microsoft Purview Account** e forneça as informações necessárias, como nome da conta, região e grupo de recursos.

3. **Configurar Escaneamento e Rótulos**: Configure políticas de escaneamento de dados para detectar e rotular dados sensíveis, como PII ou dados regulatórios.

4. **Gerenciamento de Acessos**: Atribua permissões específicas para usuários gerenciarem o catálogo de dados ou analisarem a conformidade.

## Bloqueio de Recursos no Azure

Para evitar alterações acidentais ou exclusões de recursos no Azure, o Azure permite bloquear recursos com os modos de bloqueio **Read-Only** e **Delete**.

### Etapas para Bloquear Recursos

1. **Selecionar o Recurso ou Grupo de Recursos**: No portal do Azure, navegue até o recurso ou grupo de recursos que deseja bloquear.
   
2. **Configurar o Bloqueio**: Na seção de configurações, selecione **Locks** e adicione um novo bloqueio.
   
   - **Read-Only**: Restringe todas as ações exceto leitura.
   - **Delete**: Impede que o recurso seja excluído, mas ainda permite modificações.

3. **Aplicar o Bloqueio**: Defina um nome para o bloqueio e selecione o tipo de bloqueio desejado.

4. **Gerenciar e Monitorar**: Use o portal do Azure para monitorar os bloqueios e certificar-se de que as políticas estão sendo seguidas corretamente.

Com essas etapas, as organizações podem garantir maior segurança e controle sobre os seus recursos e dados no Azure.
