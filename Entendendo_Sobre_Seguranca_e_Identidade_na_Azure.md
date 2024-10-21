# Identidade no Azure: Microsoft Entra ID e RBAC

## Microsoft Entra ID (anteriormente Azure AD)
O Microsoft Entra ID, anteriormente conhecido como Azure Active Directory, é o serviço de gerenciamento de identidade e acesso da Microsoft para recursos na nuvem. Ele oferece uma maneira centralizada e segura de autenticar e autorizar usuários, aplicativos e dispositivos.

### Passos para Configurar com RBAC (Controle de Acesso Baseado em Função)
1. **Crie um grupo no Microsoft Entra ID**: 
   - Navegue até o portal do Azure.
   - Acesse **Azure Active Directory** > **Grupos** > **Novo Grupo**.
   - Defina as permissões de acesso do grupo.
   
2. **Atribua Funções no RBAC**:
   - No portal do Azure, vá até o recurso ao qual deseja conceder acesso.
   - Selecione **Controle de Acesso (IAM)**.
   - Escolha **Atribuir função** e selecione a função apropriada, como Leitor, Colaborador ou Proprietário.
   - Atribua essa função ao grupo ou usuário específico.

3. **Verifique as permissões**: Após atribuir a função, verifique se os usuários têm as permissões corretas acessando o recurso com as novas credenciais.

# Segurança no Azure: Microsoft Defender for Cloud

## Microsoft Defender for Cloud
O Microsoft Defender for Cloud é uma solução integrada de gerenciamento de postura de segurança e proteção contra ameaças para workloads no Azure, AWS, e Google Cloud. Ele monitora constantemente os recursos da nuvem e oferece recomendações para fortalecer a segurança.

### Passos para Configurar o Microsoft Defender for Cloud
1. **Habilite o Defender for Cloud**:
   - Acesse o portal do Azure.
   - Navegue até **Microsoft Defender for Cloud**.
   - Selecione **Começar** e habilite a proteção para suas assinaturas.

2. **Configurar Políticas de Segurança**:
   - No portal do Microsoft Defender for Cloud, vá até **Gerenciamento de Políticas**.
   - Selecione a assinatura ou o escopo em que deseja aplicar a política de segurança.
   - Escolha as recomendações de segurança que deseja seguir, como proteção contra vulnerabilidades e criptografia.

3. **Monitoramento de Segurança**:
   - Use os painéis de segurança do Defender for Cloud para visualizar alertas, ameaças e recomendações.
   - Integre com o **Azure Sentinel** para uma visão mais ampla e respostas automatizadas às ameaças.

4. **Ações de Correção**:
   - Siga as recomendações fornecidas pelo Defender for Cloud para mitigar riscos, como corrigir vulnerabilidades, restringir portas de rede abertas e implementar criptografia.
