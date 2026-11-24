# API de Chamados de Suporte

**Estudante:** Lucas Gabriel Correia Gonçalves

## Objetivo
Criar a estrutura inicial de uma API REST para gerenciamento de chamados de suporte utilizando Python, Flask e `uv` para gerenciamento de ambiente e dependências.

## Instalação das Dependências
Certifique-se de ter o `uv` instalado e execute o comando abaixo na raiz do projeto para recriar o ambiente conforme o `uv.lock`:

```bash
uv sync --locked
```

## Como Executar a Aplicação

**No GitHub Codespaces:**
```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

**Em ambiente local:**
```bash
uv run flask --app app run --port=5000
```

## Acesso à Rota Inicial e Resposta Esperada
Com a aplicação em execução, faça uma requisição `GET` para a rota `/` pelo navegador em `http://localhost:5000/` ou pelo terminal:

```bash
curl -i http://localhost:5000/
```

**Resposta esperada:**
- **Status HTTP:** `200 OK`
- **Cabeçalho:** `Content-Type: application/json`
- **Corpo (JSON):**
```json
{
  "mensagem": "API de chamados em funcionamento"
}
```