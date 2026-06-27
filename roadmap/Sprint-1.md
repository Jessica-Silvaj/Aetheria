# Sprint 1

## Objetivo
- Preparar o servidor Paper local basico para o projeto Aetheria Online, sem executar instalacoes nesta etapa de planejamento.

## Tarefas
1. Definir a versao-alvo do Minecraft e a build do Paper para desenvolvimento local.
2. Verificar na documentacao oficial do Paper a versao de Java exigida para Paper 26.x (sem assumir Java 21 automaticamente).
3. Definir estrutura da pasta de runtime do servidor (ex.: server/runtime/).
4. Planejar o download futuro do Paper (origem oficial e arquivo esperado).
5. Planejar o primeiro start do servidor para gerar arquivos base.
6. Planejar o aceite do EULA (arquivo eula.txt, alteracao para true).
7. Planejar configuracao inicial de server.properties para ambiente local.
8. Planejar criacao de scripts de inicializacao (PowerShell e Bash) para start local.
9. Definir lista de plugins essenciais para instalacao futura (sem baixar agora):
	- LuckPerms
	- Vault
	- PlaceholderAPI
	- ProtocolLib
	- EssentialsX
	- CoreProtect
	- WorldEdit
	- WorldGuard
	- Chunky
	- BlueMap
10. Definir checklist de teste local apos setup inicial (startup, logs, plugins e comandos basicos).
11. Planejar commit final da Sprint 1 com mensagem padronizada.

## Status da Etapa Atual
- Concluido nesta etapa: escolha de build estavel (fallback Paper 26.1.2), download do paper.jar, primeiro boot, aceite do EULA e segundo boot sem erro critico.
- Primeiro lote de plugins base testado em 2026-06-27.
- Servidor base funcional com 5 plugins carregados: LuckPerms 5.5.57, Vault 1.7.3-b131, PlaceholderAPI 2.12.2, ProtocolLib 5.4.0 e EssentialsX 2.22.0.
- ProtocolLib 5.4.0 instalado com aviso: Minecraft 26.1.2 ainda nao foi testado pelo plugin.
- CoreProtect 23.2 esta pendente/incompativel temporariamente: foi testado, informou `Minecraft 26.1.2 is not supported` e foi removido.
- Nao reinstalar CoreProtect ate existir versao compativel com Paper/Minecraft 26.1.2 ou ate a versao do Paper ser reavaliada.
- Observacao: em um teste anterior, o comando `stop` no console do Paper 26.1.2 gerou excecao.
- Segundo lote de plugins base testado em 2026-06-27.
- Servidor iniciou com 9 plugins carregados: LuckPerms, Vault, PlaceholderAPI, ProtocolLib, EssentialsX, WorldEdit, WorldGuard, Chunky e BlueMap.
- Segundo lote instalado: WorldEdit 7.4.3, WorldGuard 7.0.16, Chunky 1.5.3 e BlueMap 5.22.
- Aviso do segundo lote: BlueMap carregou, mas precisa aceitar o download de recursos em `plugins/BlueMap/core.conf` antes de funcionar plenamente.
- ProtocolLib esta funcional, mas segue com aviso de versao nao testada em Minecraft 26.1.2.
- Aviso de shutdown: EssentialsX 2.22.0 gerou aviso de tarefa assincrona durante parada com `stop`, sem bloquear o servidor.
- `server.properties` ajustado para Alpha Local: `online-mode=false`, `white-list=false`, servidor leve para ate 10 jogadores, survival normal e PvP desativado.
- Aviso de seguranca: antes de abrir ao publico, sera obrigatorio instalar/configurar autenticacao/login e proteger nicks administrativos.
- AuthMeReloaded 6.0.0 Paper instalado em 2026-06-27 para proteger nicks no modo offline/cracked aberto.
- Servidor iniciou com 10 plugins carregados; AuthMe habilitou SQLite e hooks em LuckPerms/Essentials.
- Jogadores precisam usar `/register senha senha` no primeiro acesso e `/login senha` nos proximos acessos; administradores devem registrar seus nicks antes de liberar para amigos.
- Pendencia: validar o fluxo `/register` e `/login` em jogo com cliente Minecraft local.
- Guia `docs/Admin-Seguranca.md` criado com checklist de registro do dono/admin e permissoes iniciais via LuckPerms.
- Antes de chamar amigos: dono deve registrar o nick no AuthMe, aplicar permissoes pelo console e registrar todos os comandos executados.
- Mantido fora de escopo nesta etapa: plugins de RPG e configuracoes de RPG.
- Situacao: servidor base funcional com 10 plugins; CoreProtect permanece pendente.
- Proxima etapa recomendada: configurar `server.properties`, `bukkit.yml`, `spigot.yml` e configuracoes Paper com foco em servidor local leve.

## Resultado Esperado
- Plano de execucao da Sprint 1 aprovado e pronto para implementacao passo a passo.
- Versao do Minecraft/Paper e Java 21 definidos para ambiente local.
- Estrutura de runtime, scripts e checklist documentados antes da fase de execucao.
- Lista de plugins essenciais validada para instalacao futura.

## Critérios de Conclusão
- Versao do Minecraft/Paper escolhida e registrada.
- Java 21 definido como requisito obrigatorio da sprint.
- Estrutura de runtime do servidor definida.
- Procedimento de download do Paper planejado (sem executar).
- Procedimento de primeiro start e aceite de EULA planejados (sem executar).
- Parametros iniciais de server.properties listados para ajuste futuro.
- Estrategia de scripts de start definida para Windows e Linux.
- Lista de plugins essenciais fechada exatamente com 10 itens.
- Checklist de teste local pronto para validacao futura.
- Plano de commit final documentado.

## Atenção ao limite de tokens
- Executar cada tarefa futura em prompts separados, uma por vez.
- Em cada prompt, focar apenas no escopo da tarefa atual para evitar respostas longas e truncadas.
- Antes de iniciar a proxima tarefa, confirmar rapidamente o que foi concluido na tarefa anterior.
