# Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure

Este resumo descreve os passos necessários para configurar recursos de computação e rede, além de adicionar a extensão HPE Security em uma máquina virtual na Azure.

## Pré-requisitos

- Conta ativa no Microsoft Azure.
- Acesso ao Azure Portal ou à CLI do Azure.
- Permissões adequadas para criar máquinas virtuais e configurar redes virtuais.
- Conhecimento básico de rede e computação em nuvem.

## Passo 1: Criar uma Rede Virtual

1. Acesse o [Azure Portal](https://portal.azure.com).
2. No menu lateral, clique em **Rede Virtual** e selecione **Criar**.
3. Defina o nome da rede virtual, o intervalo de endereços (ex: `10.0.0.0/16`) e a região onde ela será criada.
4. Configure sub-redes conforme necessário (ex: `10.0.1.0/24` para a sub-rede principal).
5. Clique em **Revisar e Criar** para provisionar a rede virtual.

## Passo 2: Criar uma Máquina Virtual

1. No Azure Portal, vá para **Máquinas Virtuais** e selecione **Criar**.
2. Selecione o **Sistema Operacional** e a **Região** onde a VM será criada.
3. Defina o **Tipo de Instância** de acordo com o dimensionamento necessário (por exemplo, `Standard_B2ms`).
4. Conecte a VM à rede virtual criada no Passo 1, escolhendo a sub-rede adequada.
5. Escolha o método de autenticação (chave SSH ou senha).

## Passo 3: Dimensionamento da Máquina Virtual

1. No painel de configuração da máquina virtual, configure o **Tamanho da Instância** com base nas necessidades de processamento e memória.
2. O Azure permite alterar o tipo de instância posteriormente para acomodar o aumento de tráfego ou processamento. Isso pode ser feito em **Configurações > Dimensionamento** da VM.

## Passo 4: Adicionar a Extensão HPE Security

1. Após configurar a máquina virtual, vá para **Extensões + Aplicativos** no painel da VM.
2. Clique em **Adicionar** e pesquise por **HPE Security**.
3. Selecione a extensão HPE Security e configure os parâmetros necessários, como as credenciais e as políticas de segurança.
4. Clique em **OK** para instalar a extensão.

## Passo 5: Verificar e Monitorar a Máquina Virtual

1. Após a criação da máquina virtual, verifique se está acessível usando SSH (para Linux) ou RDP (para Windows).
2. No **Painel de Monitoramento**, configure alertas e métricas de desempenho para acompanhar o uso de CPU, memória e tráfego de rede.
3. Configure backups regulares e políticas de segurança adicionais para proteger a VM contra vulnerabilidades.

## Conclusão

Seguindo esses passos, é possível configurar uma máquina virtual no Azure, conectada à rede virtual, com dimensionamento configurado para suportar diferentes níveis de tráfego e com a extensão HPE Security ativada para maior segurança. É importante ajustar o tamanho da instância e as políticas de segurança conforme as necessidades mudarem ao longo do tempo.
