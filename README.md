# 🤖 Agno AI Agents

> Exploração e implementação de agentes de IA utilizando a biblioteca [Agno](https://github.com/agno-agi/agno).

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)
![Agno](https://img.shields.io/badge/Library-Agno-purple)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)

---

## 📖 Sobre o Projeto

Este repositório tem como objetivo explorar, prototipar e implementar **agentes de inteligência artificial** utilizando a biblioteca **Agno** — um framework moderno e modular para construção de agentes autônomos com suporte a ferramentas, memória, raciocínio e workflows multiagente.

---

## ✨ Funcionalidades Planejadas

- 🧠 Criação de agentes com raciocínio autônomo
- 🛠️ Integração com ferramentas customizadas (tools)
- 🗂️ Gerenciamento de memória e contexto
- 🔄 Workflows com múltiplos agentes colaborando
- 🌐 Integração com APIs externas (ex: Microsoft Graph, OpenAI)
- 📊 Geração de relatórios e automações inteligentes

---

## 📁 Estrutura do Projeto

```
agno-ai-agents/
├── agents/             # Definição e configuração dos agentes
├── tools/              # Ferramentas customizadas para os agentes
├── workflows/          # Fluxos de trabalho multiagente
├── memory/             # Configurações de memória e contexto
├── examples/           # Exemplos práticos de uso
├── tests/              # Testes unitários e de integração
├── requirements.txt    # Dependências do projeto
└── README.md           # Documentação principal
```

---

## 🚀 Começando

### Pré-requisitos

- Python 3.10 ou superior
- pip ou uv (gerenciador de pacotes)

### Instalação

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/Leandro-SM/agno-ai-agents.git
   cd agno-ai-agents
   ```

2. **Crie um ambiente virtual:**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Linux/macOS
   .venv\Scripts\activate     # Windows
   ```

3. **Instale as dependências:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure as variáveis de ambiente:**
   ```bash
   cp .env.example .env
   # Edite o arquivo .env com suas chaves de API
   ```

---

## 💡 Exemplo Rápido

```python
from agno.agent import Agent
from agno.models.openai import OpenAIChat

agent = Agent(
    model=OpenAIChat(id="gpt-4o"),
    description="Você é um assistente inteligente especializado em automações.",
    instructions=["Seja objetivo e claro.", "Use ferramentas quando necessário."],
    markdown=True,
)

agent.print_response("Quais são as melhores práticas para agentes de IA?")
```

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Descrição |
|------------|-----------|
| [Agno](https://github.com/agno-agi/agno) | Framework principal para agentes de IA |
| [OpenAI](https://platform.openai.com/) | Modelos de linguagem (GPT-4o, etc.) |
| [Python](https://www.python.org/) | Linguagem de programação principal |
| [Pydantic](https://docs.pydantic.dev/) | Validação e modelagem de dados |

---

## 📌 Roadmap

- [ ] Configuração inicial do projeto
- [ ] Primeiro agente funcional
- [ ] Integração com ferramentas externas
- [ ] Workflow multiagente
- [ ] Documentação completa dos exemplos
- [ ] Testes automatizados

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma _issue_ ou enviar um _pull request_.

1. Faça um fork do projeto
2. Crie sua branch: `git checkout -b feature/minha-feature`
3. Commit suas alterações: `git commit -m 'feat: adiciona minha feature'`
4. Push para a branch: `git push origin feature/minha-feature`
5. Abra um Pull Request

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👤 Autor

**Leandro Medeiros**
- GitHub: [@Leandro-SM](https://github.com/Leandro-SM)
- Localização: São Paulo, Brasil 🇧🇷
