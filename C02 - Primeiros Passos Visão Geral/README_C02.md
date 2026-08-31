# Curso de Python — Visão Geral, Instalação e DSA | AI Coder

## Sobre o curso

Este repositório reúne anotações, códigos, exercícios e materiais desenvolvidos durante o módulo **Primeiros Passos com a Linguagem Python**, do curso **DSA AI Coder**.

O módulo apresenta os fundamentos necessários para iniciar projetos em Python, preparar o ambiente de desenvolvimento e construir uma aplicação utilizando recursos de Inteligência Artificial.

## Objetivos

- Conhecer a proposta do curso e a metodologia de estudo.
- Entender o conceito de *Vibe Coding* e programação assistida por IA.
- Instalar e validar o ambiente Anaconda em diferentes sistemas operacionais.
- Utilizar o Google Colab como alternativa para executar códigos Python.
- Aprender os fundamentos iniciais da linguagem Python.
- Conhecer pacotes, dependências e ambientes virtuais.
- Criar uma aplicação com Streamlit.
- Consumir uma API de modelo de linguagem.
- Utilizar a plataforma Groq para acesso a modelos de IA.
- Configurar prompts personalizados para LLMs.

## Conteúdo do módulo

### 1. Primeiros passos

- Introdução ao curso.
- Como estudar programação em Python na era da IA.
- Conceito de *Vibe Coding* com ChatGPT.
- Programação assistida por IA.
- Expectativas de aprendizagem no curso.
- Ferramentas utilizadas.

### 2. Preparação do ambiente

- Download e instalação do Anaconda Python.
- Instalação no macOS.
- Instalação no Linux.
- Instalação no Windows.
- Testes da instalação em macOS/Linux e Windows.
- Google Colab como alternativa para programação em Python.

### 3. Estudo de caso: assistente de IA

O estudo de caso consiste na criação de um assistente de IA para programação Python, utilizando uma aplicação web desenvolvida com Streamlit e integrada a um modelo de linguagem.

Tópicos abordados:

- Funcionamento do estudo de caso.
- Criação de uma conta e utilização da plataforma Groq.
- Criação e utilização de uma API.
- PyPI e instalação de pacotes Python.
- Pacotes e gerenciamento de dependências.
- Definição de prompts personalizados para LLMs.
- Construção da interface da aplicação com Streamlit.
- Criação de uma chave Groq para acesso ao LLM.
- Seleção de modelos de linguagem disponíveis.

## Tecnologias e ferramentas

- [Python](https://www.python.org/)
- [Anaconda](https://www.anaconda.com/)
- [Google Colab](https://colab.research.google.com/)
- [Streamlit](https://streamlit.io/)
- [Groq](https://groq.com/)
- [PyPI](https://pypi.org/)
- Modelos de linguagem — LLMs
- ChatGPT como ferramenta de apoio ao desenvolvimento

## Pré-requisitos

- Conhecimentos básicos de informática.
- Conta Google para utilizar o Google Colab, caso necessário.
- Conta na plataforma Groq para gerar uma chave de API.
- Python e Anaconda instalados localmente, ou acesso ao Google Colab.
- Editor de código, como Visual Studio Code, opcionalmente.

## Instalação do ambiente

### Opção 1: Anaconda

1. Acesse o site oficial do [Anaconda](https://www.anaconda.com/download).
2. Baixe o instalador correspondente ao seu sistema operacional.
3. Execute o instalador e siga as instruções exibidas.
4. Abra o Anaconda Prompt, Terminal ou uma ferramenta equivalente.
5. Verifique a instalação:

```bash
python --version
conda --version
```

### Opção 2: Google Colab

1. Acesse o [Google Colab](https://colab.research.google.com/).
2. Crie um novo notebook.
3. Execute uma célula simples para validar o Python:

```python
print("Ambiente Python funcionando!")
```

## Estrutura sugerida do projeto

```text
.
├── README.md
├── requirements.txt
├── app.py
├── .env.example
├── notebooks/
│   └── estudos_python.ipynb
├── src/
│   └── prompts.py
└── docs/
    └── anotações.md
```

A estrutura pode ser adaptada conforme a evolução do estudo de caso.

## Ambiente virtual

A criação de um ambiente virtual ajuda a isolar as dependências do projeto:

```bash
conda create -n dsa-python python=3.11
conda activate dsa-python
```

Caso seja utilizado `venv`:

```bash
python -m venv .venv
```

No Windows:

```bash
.venv\Scripts\activate
```

No macOS/Linux:

```bash
source .venv/bin/activate
```

## Dependências

Depois de ativar o ambiente, instale os pacotes necessários:

```bash
pip install streamlit groq python-dotenv
```

Para registrar as dependências instaladas:

```bash
pip freeze > requirements.txt
```

## Configuração da API

Crie uma chave de API na plataforma Groq e armazene-a em uma variável de ambiente. Nunca publique chaves reais no repositório.

Crie um arquivo `.env` com o seguinte formato:

```env
GROQ_API_KEY=sua_chave_aqui
```

Também é recomendável adicionar `.env` ao arquivo `.gitignore`:

```gitignore
.env
.venv/
__pycache__/
```

## Execução da aplicação

Com o ambiente virtual ativado e as dependências instaladas, execute:

```bash
streamlit run app.py
```

O Streamlit exibirá um endereço local para abrir a aplicação no navegador.

## Boas práticas

- Não compartilhe chaves de API ou outros segredos.
- Utilize ambientes virtuais para cada projeto.
- Registre as dependências em `requirements.txt`.
- Faça commits pequenos e descritivos.
- Valide as respostas geradas pela IA antes de utilizá-las em produção.
- Use a IA como apoio ao aprendizado, mantendo entendimento sobre o código produzido.
- Documente decisões, limitações e problemas encontrados durante o desenvolvimento.

## Status

Em desenvolvimento, acompanhando a evolução das aulas e do estudo de caso do curso DSA AI Coder.

## Autor

Luís Filipe

Estudante de Análise e Engenharia de Dados.
