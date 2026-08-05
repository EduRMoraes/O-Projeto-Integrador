# 🧪 Planos e Casos de Teste — Garantia de Qualidade (QA)

Esta seção reúne a documentação de garantia de qualidade da **Biblioteca Virtual TG Americana**, responsável por validar a estabilidade, segurança e usabilidade do sistema desktop offline antes de sua implantação.

---

## 📌 Conceitos Fundamentais

### 📋 O que é um Plano de Testes?
O **Plano de Testes** é o documento estratégico que define o escopo, os objetivos, os recursos, o cronograma e a abordagem de testes da aplicação. Ele funciona como o guia geral de garantia de qualidade, determinando:
- **O que será testado**: Funcionalidades críticas (ex: cadastro de livros, empréstimos, busca offline).
- **O que NÃO será testado**: Escopos fora da versão atual (ex: integração com nuvem).
- **Critérios de Aceitação e Rejeição**: Parâmetros para considerar o software apto para entrega.
- **Ambiente de Teste**: Configurações de hardware/SO (Windows Forms offline).

### 🔍 O que é um Caso de Teste?
Um **Caso de Teste** é a menor unidade de validação prática do sistema. É um conjunto detalhado de condições, passos e dados de entrada com os quais um testador verifica se uma funcionalidade específica comporta-se como esperado. 

Cada Caso de Teste contém obrigatoriamente:
- **ID do Teste**: Identificador único (ex: `CT-001`).
- **Pré-condições**: O que precisa estar configurado antes de executar (ex: *Usuário logado como administrador*).
- **Passos para Execução**: Ações sequenciais que o testador deve realizar.
- **Resultado Esperado**: O comportamento exato exigido do sistema.
- **Resultado Obtido**: O comportamento real observado (Passou / Falhou).

---

## 🛠️ Estrutura de um Caso de Teste Padronizado

Todos os casos de teste deste repositório devem seguir o modelo abaixo:

| Campo | Descrição / Exemplo |
| :--- | :--- |
| **ID** | `CT-002` |
| **Funcionalidade** | Validação de Devoluição Atrasada |
| **Objetivo** | Garantir que o sistema notifique o operador sobre empréstimos vencidos. |
| **Pré-condições** | Existir um empréstimo cadastrado com data de devolução anterior à data atual. |
| **Passos** | 1. Abrir tela de Devoluções.<br>2. Digitar o código do livro.<br>3. Clicar em "Confirmar Devolução". |
| **Resultado Esperado** | Exibir alerta em vermelho indicando pendência e atualizar o status do exemplar para "Disponível". |
| **Status** | `Aprovado` / `Reprovado` |
