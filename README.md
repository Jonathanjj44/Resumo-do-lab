# Resumo-do-lab

# Computação em Nuvem e Microsoft Azure

Este `README.md` aborda conceitos fundamentais de computação em nuvem, com foco especial na Microsoft Azure, incluindo como criar uma conta e as opções de armazenamento disponíveis.

## O que é Computação em Nuvem?

A Computação em Nuvem (Cloud Computing) é um modelo de entrega de recursos de computação (servidores, armazenamento, bancos de dados, redes, software, análises, inteligência artificial) sob demanda pela internet, com pagamento conforme o uso. Em vez de possuir e manter sua própria infraestrutura de TI, você pode acessá-la de um provedor de serviços em nuvem, como a Microsoft Azure.

### Principais Características:

* **Autosserviço sob demanda:** Os usuários podem provisionar recursos de computação sem a necessidade de interação humana com o provedor de serviços.
* **Amplo acesso à rede:** Os recursos estão disponíveis pela rede e podem ser acessados por uma variedade de dispositivos (laptops, celulares, tablets).
* **Agrupamento de recursos:** Os recursos de computação do provedor são agrupados para atender a vários consumidores usando um modelo multi-tenant, com diferentes recursos físicos e virtuais atribuídos e reatribuídos dinamicamente de acordo com a demanda do consumidor.
* **Elasticidade rápida:** Os recursos podem ser provisionados e liberados de forma elástica e rápida para escalar rapidamente conforme a demanda.
* **Serviço medido:** Os sistemas de nuvem controlam e otimizam o uso de recursos, medindo-o em um nível de abstração apropriado ao tipo de serviço (por exemplo, armazenamento, processamento, largura de banda).

### Modelos de Serviço em Nuvem:

* **IaaS (Infrastructure as a Service):** Você aluga a infraestrutura de TI virtualizada, como servidores, redes, sistemas operacionais e armazenamento. Você tem controle sobre o sistema operacional e os aplicativos. Exemplos: Máquinas Virtuais Azure.
* **PaaS (Platform as a Service):** Você tem uma plataforma de desenvolvimento e ambiente de execução completo na nuvem. O provedor gerencia a infraestrutura subjacente. Exemplos: Azure App Service, Azure Functions.
* **SaaS (Software as a Service):** O software é hospedado e gerenciado pelo provedor de serviços em nuvem e disponibilizado aos usuários finais pela internet. Exemplos: Microsoft 365, Outlook.com.

### Modelos de Implantação em Nuvem:

* **Nuvem Pública:** Os recursos são de propriedade e operados por um provedor de serviços em nuvem terceirizado e são compartilhados com outros clientes.
* **Nuvem Privada:** Os recursos de computação são usados exclusivamente por uma única organização. Podem ser gerenciados internamente ou por um terceiro.
* **Nuvem Híbrida:** Combinação de nuvem pública e privada, permitindo que os dados e aplicativos se movam entre elas.

## Criando uma Conta Gratuita no Microsoft Azure

O Microsoft Azure oferece uma conta gratuita que permite explorar muitos de seus serviços por 12 meses, além de um crédito inicial.

Siga os passos abaixo para criar sua conta:

1.  **Acesse o site do Azure:** Navegue até o [site do Microsoft Azure](https://azure.microsoft.com/pt-br/free/).
2.  **Clique em "Iniciar gratuitamente":** Você encontrará um botão proeminente para iniciar sua avaliação gratuita.
3.  **Faça login com sua conta Microsoft:** Se você já tem uma conta Microsoft (Outlook.com, Hotmail, Xbox, etc.), pode usá-la. Caso contrário, será necessário criar uma.
4.  **Preencha seus dados:** Você precisará fornecer informações pessoais, como nome, endereço de e-mail e número de telefone.
5.  **Verificação de identidade por telefone:** O Azure exigirá uma verificação de identidade por meio de um código enviado para o seu telefone.
6.  **Informações do cartão de crédito:** **É obrigatório fornecer um cartão de crédito para verificação de identidade.** No entanto, **você não será cobrado automaticamente após o término do período de avaliação gratuita.** O Azure solicitará sua permissão antes de qualquer cobrança. Eles usam o cartão para garantir que você não é um robô e para evitar abusos do serviço gratuito.
7.  **Concorde com os termos e condições:** Leia e aceite os termos do contrato de serviços Microsoft e a política de privacidade.
8.  **Inicie seu teste gratuito:** Após a verificação e aceitação, sua conta Azure gratuita será ativada e você será redirecionado para o portal do Azure.

## Armazenamento no Azure

O Azure oferece uma ampla gama de serviços de armazenamento para atender a diversas necessidades, desde dados não estruturados até bancos de dados relacionais e não relacionais.

### Principais Tipos de Armazenamento no Azure:

1.  **Armazenamento de Blobs do Azure (Azure Blob Storage):**
    * **O que é:** Um serviço de armazenamento de objetos altamente escalável para dados não estruturados. Isso inclui texto, binários, imagens, vídeos, documentos, arquivos de log, backups de VMs, etc.
    * **Casos de uso:** Servir imagens ou documentos diretamente para um navegador, armazenamento de arquivos para acesso distribuído, streaming de vídeo e áudio, gravação de dados de log, armazenamento de dados para backup e restauração.
    * **Camadas de acesso:**
        * **Hot (Quente):** Para dados acessados com frequência. Custo de armazenamento mais alto, mas custo de acesso mais baixo.
        * **Cool (Frio):** Para dados acessados com pouca frequência, mas que precisam estar disponíveis imediatamente. Custo de armazenamento mais baixo, mas custo de acesso mais alto.
        * **Archive (Arquivo):** Para dados raramente acessados e que podem tolerar latência de acesso de horas. Custo de armazenamento muito baixo, mas custo de acesso muito alto.

2.  **Armazenamento de Arquivos do Azure (Azure Files):**
    * **O que é:** Oferece compartilhamentos de arquivos totalmente gerenciados na nuvem, acessíveis via protocolo SMB (Server Message Block) ou NFS (Network File System).
    * **Casos de uso:** Substituir servidores de arquivos locais, "lift and shift" de aplicativos que esperam um compartilhamento de arquivos, compartilhamento de arquivos entre máquinas virtuais.

3.  **Armazenamento de Tabelas do Azure (Azure Table Storage):**
    * **O que é:** Um armazenamento de chave-valor NoSQL para grandes quantidades de dados estruturados não relacionais.
    * **Casos de uso:** Aplicativos que precisam armazenar grandes quantidades de dados NoSQL de forma econômica e escalável.

4.  **Armazenamento de Filas do Azure (Azure Queue Storage):**
    * **O que é:** Um serviço para armazenar um grande número de mensagens. Usado para comunicação assíncrona entre componentes de aplicativos.
    * **Casos de uso:** Construir cargas de trabalho assíncronas, desacoplar componentes de aplicativos.

5.  **Discos Gerenciados do Azure (Azure Managed Disks):**
    * **O que é:** Volumes de armazenamento em bloco para uso com máquinas virtuais do Azure. Os Managed Disks são gerenciados pelo Azure e garantem alta disponibilidade.
    * **Casos de uso:** Armazenamento principal para sistemas operacionais e dados de máquinas virtuais.

### Como Usar o Armazenamento no Azure (Exemplo: Blob Storage)

Você pode interagir com o armazenamento do Azure de diversas maneiras:

* **Portal do Azure:** Interface gráfica para gerenciar seus recursos.
    1.  No Portal do Azure, pesquise por "Contas de armazenamento".
    2.  Clique em "Criar conta de armazenamento".
    3.  Preencha os detalhes (Grupo de recursos, Nome da conta de armazenamento, Região, Nível de desempenho, Tipo de redundância).
    4.  Após a criação, navegue até a conta de armazenamento e selecione "Contêineres" em "Armazenamento de dados".
    5.  Crie um novo contêiner para organizar seus blobs.
    6.  Dentro do contêiner, você pode carregar blobs (arquivos).

* **Azure CLI (Command Line Interface):** Para automação e scripts.
    ```bash
    # Fazer login no Azure
    az login

    # Criar um grupo de recursos (se ainda não tiver um)
    az group create --name MeuGrupoDeRecursos --location brazilsouth

    # Criar uma conta de armazenamento
    az storage account create \
        --name minhacontazurao \
        --resource-group MeuGrupoDeRecursos \
        --location brazilsouth \
        --sku Standard_LRS \
        --kind StorageV2

    # Criar um contêiner de blobs
    az storage container create \
        --name meucontainer \
        --account-name minhacontazurao \
        --public-access blob

    # Carregar um arquivo para o contêiner
    az storage blob upload \
        --container-name meucontainer \
        --file caminho/para/seu/arquivo.txt \
        --name meu_arquivo_na_nuvem.txt \
        --account-name minhacontazurao
    ```

* **Azure PowerShell:** Outra ferramenta de linha de comando para automação.
    ```powershell
    # Fazer login no Azure
    Connect-AzAccount

    # Criar um grupo de recursos
    New-AzResourceGroup -Name "MeuGrupoDeRecursos" -Location "brazilsouth"

    # Criar uma conta de armazenamento
    New-AzStorageAccount -Resource
    
