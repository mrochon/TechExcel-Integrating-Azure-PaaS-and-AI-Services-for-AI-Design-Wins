[Lab instructions](https://microsoft.github.io/TechExcel-Integrating-Azure-PaaS-and-AI-Services-for-AI-Design-Wins/)

### Starting python

```
source aiwins/bin/activate
python -m streamlit run Index.py
```

### Creating secrets for web api:

```
dotnet user-secrets set "CosmosDB:AccountEndpoint" "https://cosmos-gcrhokmpwzvag.documents.azure.com:443/"
dotnet user-secrets set "AZURE_CLIENT_ID" "..."
dotnet user-secrets set "CosmosDB:DatabaseName" "ContosoSuites"
dotnet user-secrets set "CosmosDB:MaintenanceRequestsContainerName" "MaintenanceRequests"
dotnet user-secrets set "AzureOpenAI:EmbeddingDeploymentName" "text-embedding-ada-002"
dotnet user-secrets set "AzureOpenAI:Endpoint" "https://openai-gcrhokmpwzvag.openai.azure.com/"
dotnet user-secrets set "AzureOpenAI:ApiKey" "..."
dotnet user-secrets set "AzureOpenAI:DeploymentName" "gpt-4o"
dotnet user-secrets set "ApiManagement:Endpoint" "https://apim-gcrhokmpwzvag.azure-api.net/azure-openai-api/"
dotnet user-secrets set "ApiManagement:ApiKey" "..."
```

### Setup

In terminal:
```
python -m venv aiwins
cd src/ContosoSuitesDashboard
pip install -r requirements.txt
# Repeat on every terminal to activate
source aiwins/bin/activate
```
