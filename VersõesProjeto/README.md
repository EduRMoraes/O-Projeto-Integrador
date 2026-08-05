---

## 📁 Estrutura de Versionamento (`Versoes/`)

A pasta `Versoes/` é destinada ao armazenamento do histórico de lançamentos (*releases*), notas de versão (*change logs*) e compilações executáveis da **Biblioteca Virtual TG Americana**.

Seu principal objetivo é garantir o rastreamento evolutivo do sistema, documentando o progresso das funcionalidades, correções e melhorias ao longo das Sprints do Projeto Integrador.

### 🏷️ Padrão de Nomenclatura (Semantic Versioning)
O projeto segue o padrão `MAJOR.MINOR.PATCH` (`vX.Y.Z`):
- **MAJOR (`v1.0.0`)**: Alterações grandes, marcos principais do projeto ou entregas finais de semestre.
- **MINOR (`v1.1.0`)**: Adição de novas funcionalidades (ex: novos filtros de pesquisa, módulos de relatórios).
- **PATCH (`v1.0.1`)**: Correção de bugs, pequenos ajustes visuais em Windows Forms ou melhorias pontuais de desempenho.

### 📂 Organização da Pasta
```text
📁 Versoes/
│
├── 📁 v0.1.0-alpha/         # Protótipo inicial e validação da interface
│   ├── 📄 CHANGELOG.md       # Detalhamento de alterações da versão
│   └── 📄 Release_Notes.md   # Notas de entrega da versão
│
├── 📁 v1.0.0-beta/          # Versão pré-estável para testes locais offline
└── 📄 VERSOES.md             # Tabela com o histórico geral de lançamentos
