# Passo a passo para implantação de um modelo automatizado de Machine Learning

# Passo 1: Preparação dos dados

Para iniciar, é primordial preparar os dados que serão usados para treinar e testar o modelo. Nesse exemplo, usaremos um conjunto de dados de alugueis de bicicletas, disponíveis em: https://aka.ms/ai900-auto-ml

# Passo 2: Configuração do Azure ML

1. Faça login no Portal Azure (https://portal.azure.com) utilizando suas credenciais da Microsoft.
2. Selecione (+Create a new resource), procure por "Machine Learning", e crie um novo recurso Azure Machine Learning com as configurações necessárias. Nesse caso, utilizarei as seguintes configurações:

    - Subscription: Your Azure subscription.
    - Resource group: Create or select a resource group.
    - Name: Enter a unique name for your workspace.
    - Region: Select the closest geographical region.
    - Storage account: Note the default new storage account that will be created for your workspace.
    - Key vault: Note the default new key vault that will be created for your workspace.
    - Application insights: Note the default new application insights resource that will be created for your workspace.
    - Container registry: None (one will be created automatically the first time you deploy a model to a container).
3. Selecione (Review+Create) e depois (+Create) e aguarde a workspace ser criada. Esse processo pode levar alguns minutos.


# Passo 3: Treinamento do modelo

1. Escolha um algoritmo de Machine Learning adequado para o seu problema. Nesse caso, utilizaremos um modelo de Regressão.
2. Crie um novo trabalho utilizando o Automated ML e configure de acordo com suas necessidades.
3. Envie o trabalho de treinamento, ele irá iniciar automaticamente e poderá levar cerca de 15 minutos para ser concluído.

# Passo 4: Revisão do melhor modelo

1. Após a finalização do treinamento do modelo, você poderá revisar o melhor modelo treinado. 

# Passo 5: Implantação e teste do modelo


