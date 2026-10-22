# AWS Bedrock: estudos e workshops

Notebooks de estudo de IA generativa na AWS com o Amazon Bedrock.

| Pasta | Conteúdo |
|---|---|
| `Getting Started with AWS Generative AI for Developers/` | Exercícios com Bedrock: Converse API, Prompt Management, Guardrails, Tool Use, Prompt Routing |
| `Workshop_Agentcore/` | Workshop de agentes com Amazon Bedrock AgentCore (agente, memória, gateway) |

## Configuração

1. Configure suas credenciais AWS (veja `genai-exercise-0-aws-configure.ipynb`).
2. Instale as dependências: `pip install boto3 python-dotenv`
3. Copie `.env.example` para `.env` e preencha o ID da sua conta AWS:

   ```
   AWS_ACCOUNT_ID=123456789012
   ```

Os notebooks que montam ARNs leem `AWS_ACCOUNT_ID` do `.env` com `python-dotenv`. O `load_dotenv()` procura o arquivo subindo a partir da pasta do notebook, então um `.env` na raiz do repositório já basta. O `.env` está no `.gitignore` e não vai para o repositório.
