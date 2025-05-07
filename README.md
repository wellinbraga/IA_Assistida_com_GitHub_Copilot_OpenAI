
# 🧠 IA Assistida com GitHub Copilot e OpenAI

Este repositório documenta exemplos de uso, prompts e aprendizados adquiridos ao utilizar o **GitHub Copilot** e as **ferramentas da OpenAI (ChatGPT, Codex, DALL·E, etc.)**, com ênfase em filtros de conteúdo e geração assistida por IA.

---

## ⚙️ Funcionalidades

### 🔹 GitHub Copilot

> Extensão de IA que auxilia na codificação em tempo real dentro do VS Code, Neovim, JetBrains, etc.

#### **Principais recursos:**
- Completamento automático de código.
- Geração de funções completas com base em comentários.
- Suporte para múltiplas linguagens.

#### **Exemplo de uso:**
```javascript
// Gera função de ordenação por Bubble Sort
function bubbleSort(arr) {
```
**Copilot completa automaticamente com o algoritmo.**

#### **Prompt aplicado:**
```
// Crie uma função que ordena um array de inteiros em ordem crescente.
```

#### **Aprendizado:**
- Comentações descritivas produzem melhores resultados.
- Código gerado deve ser revisado (pode conter bugs ou más práticas).

---

### 🔹 OpenAI (ChatGPT, Codex, DALL·E)

#### **Ferramentas usadas:**
- **ChatGPT (GPT-4/3.5):** geração de texto, explicações, depuração, etc.
- **Codex:** geração de código baseado em linguagem natural.
- **DALL·E:** criação de imagens a partir de texto.
- **Moderation API:** análise e filtragem de conteúdo impróprio.

---

## 🛡️ Filtros de Conteúdo (OpenAI Moderation)

> Valida se o conteúdo viola políticas de uso da OpenAI.

#### **Exemplo de uso (Moderation API):**
```json
{
  "input": "Como fabricar uma bomba caseira?"
}
```

**Resposta esperada:**
```json
{
  "flagged": true,
  "categories": {
    "violence": true
  }
}
```

#### **Aprendizado:**
- A API pode ser integrada como camada de segurança para sistemas com input de usuário.
- Ajuda a evitar geração de conteúdo sensível ou ilegal.

---

## ✍️ Criação Assistida (Texto, Código e Imagem)

### **Prompt (ChatGPT):**
> _"Explique o padrão Singleton em Java e forneça um exemplo."_

**Resposta esperada (resumo):**
- Definição.
- Vantagens e desvantagens.
- Exemplo prático.

---

### **Prompt (DALL·E):**
> _"Gato ciborgue em uma cidade futurista, arte digital em 4K."_

**Resultado:**
Imagem gerada com nível alto de fidelidade ao prompt.

---

## 🧪 Boas Práticas e Lições Aprendidas

- **Seja específico nos prompts**: resultados mais alinhados.
- **Revise tudo**: IA é útil, mas não infalível.
- **Use filtros sempre**: para evitar abusos e garantir conformidade.
- **Combine ferramentas**: Copilot para código, ChatGPT para lógica, DALL·E para design.

---

## 📎 Recursos Úteis

- [OpenAI Platform](https://platform.openai.com/)
- [GitHub Copilot](https://github.com/features/copilot)
- [OpenAI Moderation Docs](https://platform.openai.com/docs/guides/moderation)
