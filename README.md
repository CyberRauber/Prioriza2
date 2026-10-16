# Prioriza

**Prioriza** é um MVP desenvolvido para o 2º Hackathon IFC Concórdia 2026 pela equipe Felipe, Weslley, Enzo P. e Isabel.

Esta versão de desenvolvimento fica no repositório [CyberRauber/Prioriza2](https://github.com/CyberRauber/Prioriza2). O projeto original [prioriza-mvp](https://github.com/CyberRauber/prioriza-mvp) continua separado e não foi alterado.

## Experiência
- Landing page editorial com apresentação da proposta e visão conceitual da Matriz de Eisenhower.
- Portal do cliente para abertura e consulta de solicitações por código.
- Gestão interna com triagem por oito critérios, ranking, atualização de status e histórico de decisões.
- Matriz de Eisenhower complementar.

## Executar localmente
Requer Node.js e npm.

```bash
npm install
npm run dev
```

Validar a compilação com `npm run build`. A landing fica na raiz e o aplicativo em `/app/`.

## Arquitetura e limites atuais
Interface React + Vite. O motor de priorização fica em `src/core/priorizacao.js`. No estado atual, as demandas são persistidas apenas no `localStorage` do navegador; não há autenticação real nem banco de dados compartilhado. A integração opcional de sugestão de IA é um recurso de demonstração executado no cliente e não deve expor chaves secretas em produção.

O portal externo não apresenta pontuação, posição no ranking ou critérios internos.

## Equipe
Felipe, Weslley, Enzo P. e Isabel.
