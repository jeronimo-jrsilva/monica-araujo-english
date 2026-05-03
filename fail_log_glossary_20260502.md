---
tipo: diario
subtipo: falha_processamento
titulo: "Relato de Falha: Invocação Indevida de Script de Glossário"
data: 2026-05-02
agente: "Gemini CLI"
---

# ⚠️ Relato de Falha: Invocação Indevida (Track 016)

Durante o processamento da trilha de faculdade (Track 002), o agente invocou indevidamente o script `90_Sistema/98_Recursos/03_Scripts/sort_monica_glossary.py`.

## 🔍 Detalhes da Falha
- **Impacto:** O arquivo `temp_skill_work/monica_portal/data.json` foi reordenado sem necessidade imediata, podendo causar conflitos com deploys pendentes.
- **Ação Corretiva:** Foi executado um `git checkout data.json` no repositório `monica-araujo-english` para reverter as alterações.
- **Status:** Rollback executado. Monitorar próxima aula da Mônica para garantir que nenhuma definição órfã foi criada.
