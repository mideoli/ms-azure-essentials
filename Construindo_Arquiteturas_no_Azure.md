# Criando uma Arquitetura no Azure

Este resumo descreve os passos básicos para criar uma arquitetura no Microsoft Azure. A arquitetura inclui a criação de uma rede virtual, um grupo de recursos e a configuração de uma máquina virtual para rodar um ambiente simples.

## Pré-requisitos

- Uma conta ativa no [Azure](https://azure.microsoft.com/).
- Conhecimentos básicos de redes e máquinas virtuais.

## Passo 1: Criar um Grupo de Recursos

O **Grupo de Recursos** é uma estrutura que facilita a organização de todos os recursos necessários para a sua arquitetura.

1. Acesse o portal do Azure.
2. No menu, selecione **Grupos de Recursos**.
3. Clique em **Adicionar**.
4. Preencha os campos:
   - **Nome do Grupo de Recursos**: Nome único para organizar seus recursos.
   - **Região**: Escolha a região mais próxima.
5. Clique em **Revisar e Criar** e depois **Criar**.

## Passo 2: Criar uma Rede Virtual (VNet)

Uma **Rede Virtual (VNet)** permite que os recursos na arquitetura comuniquem-se de forma segura.

1. No menu, selecione **Rede Virtual**.
2. Clique em **Criar**.
3. Escolha o **Grupo de Recursos** criado anteriormente.
4. Defina:
   - **Nome da Rede**: Nome único para sua VNet.
   - **Endereço IP**: Defina o intervalo de endereços IP para a rede.
   - **Sub-redes**: Configure uma ou mais sub-redes.
5. Clique em **Revisar e Criar** e depois **Criar**.

## Passo 3: Criar uma Máquina Virtual (VM)

Uma **Máquina Virtual** será utilizada para rodar seus aplicativos ou serviços.

1. No menu, selecione **Máquinas Virtuais**.
2. Clique em **Criar**.
3. Preencha os detalhes:
   - **Nome da Máquina Virtual**.
   - **Região** (deve ser a mesma do grupo de recursos).
   - **Imagem**: Escolha o sistema operacional (como Ubuntu ou Windows).
   - **Tamanho**: Selecione o tamanho da VM baseado nos recursos necessários (CPU, RAM).
4. Configure as **Configurações de Rede**:
   - Escolha a **Rede Virtual** e **Sub-rede** criadas anteriormente.
   - Selecione ou crie um novo **Endereço IP Público**.
5. Clique em **Revisar e Criar** e depois **Criar**.

## Passo 4: Configurar Segurança

1. Acesse as **Configurações de Rede** da VM.
2. Configure as regras de segurança:
   - **Portas de entrada**: Defina as portas para permitir acesso, como SSH (porta 22) para Linux ou RDP (porta 3389) para Windows.
3. Habilite **Firewalls** e configure **Grupos de Segurança de Rede** (NSG) para proteger seus recursos.

## Passo 5: Conectar-se à Máquina Virtual

Depois que a VM estiver em execução, você pode se conectar a ela:

