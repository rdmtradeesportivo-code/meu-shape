# Meu Shape 2.0 — Plano de homologação

## Regras de publicação
- Desenvolver somente nesta branch. Não publicar em main antes de validação.
- Preservar a chave localStorage `meushape-v1` e migrar dados sem apagá-los.
- Fazer backup manual antes de testes com dados reais.
- Não colocar registros de saúde, imagens ou backups no repositório público.
- Usar dados sintéticos para testes e conferir funcionamento offline.

## Escopo
1. Treino: seleção livre por grupo muscular, exercícios por grupo, histórico, recuperação de 48h por grupo, aviso e desbloqueio manual; distinguir sessão concluída de exercício isolado.
2. Alimentação: refeições numeradas 1 a 5 e adicionais, múltiplos alimentos por refeição, totais por dia e período.
3. Evolução: peso, cintura, abdômen, peito, braços, quadril, coxas, panturrilhas; fotos armazenadas localmente; comparação semanal/quinzenal/mensal.
4. Dashboard: período selecionável, peso/medidas, treinos, refeições, cargas, resumo de aplicações e exames, sem dados fictícios.
5. Exercícios: biblioteca com instruções e imagens com licença adequada, disponível offline.
6. Aplicações: catálogo pesquisável, concentração e unidade explícitas, histórico, gráfico residual apenas como estimativa de modelo, sem conversão implícita de unidades de seringa para mg nem recomendação de dose.
7. Exames: histórico e comparativos por marcador.
8. Backup: exportar/importar todos os tipos de registros e imagens, com validação de integridade e confirmação antes de substituir.

## Critérios mínimos para publicar
- Aplicativo abre sem erros em celular e computador.
- Todos os registros podem ser criados, exibidos e excluídos.
- Recuperação de 48h usa data/hora da sessão e grupo muscular corretamente.
- Os dados existentes permanecem acessíveis após atualização.
- Dashboard reflete os registros, filtros e períodos corretamente.
- Exportação/restauração testadas com dados sintéticos, inclusive imagens.
- Offline e atualização do service worker testados.
- Somente após aprovação, mesclar a branch em main.
