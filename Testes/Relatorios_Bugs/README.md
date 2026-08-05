# 🐛 Gestão e Relatórios de Bugs (Bug Reports)

Esta seção centraliza o registro, o acompanhamento e o histórico de resolução de **falhas, erros e comportamentos inesperados** identificados durante os testes da **Biblioteca Virtual TG Americana**.

---

## 📌 O que é um Relatório de Bug?

Um **Relatório de Bug (Bug Report)** é o documento formal que descreve detalhadamente uma falha encontrada no sistema. Seu objetivo é fornecer aos desenvolvedores todas as informações necessárias para **reproduzir, isolar e corrigir** o problema com rapidez e precisão.

Um bom relatório de erro reduz o tempo de depuração e evita ambiguidades entre as equipes de testes (QA) e desenvolvimento.

---

## 🚦 Classificação de Severidade

Os bugs identificados devem ser categorizados conforme o impacto no sistema:

- 🔴 **Bloqueante (Critical/Blocker)**: O sistema trava, ocorre crash irrecuperável ou uma funcionalidade chave fica inacessível sem contorno.
- 🟠 **Alta (High)**: Falha grave em regra de negócio (ex: cálculo incorreto de devolução ou erro ao salvar dados no banco).
- 🟡 **Média (Medium)**: Comportamento incorreto em fluxo secundário, mas que possui alternativa de contorno.
- 🟢 **Baixa (Low)**: Erro estético, desalinhamento de interface (IHC), pequenos erros ortográficos ou mensagens pouco claras.

---

## 📋 Estrutura Padronizada de um Bug Report

Todos os relatórios desta pasta devem ser registrados utilizando a estrutura abaixo:

| Campo | Descrição / Exemplo |
| :--- | :--- |
| **ID do Bug** | `BUG-001` |
| **Título** | Erro de exceção não tratada ao salvar livro sem campo "Autor" |
| **Severidade** | 🔴 Bloqueante |
| **Ambiente** | Windows 11 / .NET Framework 4.8 (Offline) |
| **Passos para Reproduzir** | 1. Acessar a tela *Cadastro de Livros*.<br>2. Preencher o título e a categoria.<br>3. Deixar o campo "Autor" em branco.<br>4. Clicar no botão *Salvar*. |
| **Comportamento Esperado** | Exibir mensagem de validação: *"O campo Autor é obrigatório"*. |
| **Comportamento Observado** | O sistema encerra inesperadamente com erro `NullReferenceException`. |
| **Evidência** | Screenshot da tela do erro (`bug001_crash.png`) ou arquivo de log. |
| **Status** | `Aberto` / `Em Análise` / `Corrigido` / `Fechado` |
