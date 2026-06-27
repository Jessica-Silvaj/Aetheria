# Start Here

Passo a passo futuro:
1. Verificar no site oficial do PaperMC se Paper 26.2 esta estavel.
2. Se nao estiver, usar Paper 26.1.2.
3. Verificar a versao de Java exigida para Paper 26.x na documentacao oficial do Paper.
4. Baixar o Paper.
5. Salvar como paper.jar em server/runtime/.
6. Executar o servidor uma vez.
7. Aceitar o EULA.
8. Executar novamente.
9. Testar entrada local pelo Minecraft.

## Registro desta execucao
- Data: 2026-06-27.
- Verificacao oficial: Paper 26.2 estava como experimental.
- Versao usada: Paper 26.1.2 build #72 (estavel), salvo como paper.jar.
- Java usado: Java 25 (conforme docs oficiais para 26.1+).
- Resultado: primeiro boot executado, EULA aceito, segundo boot sem erro critico e parada com `stop`.

## Registro do primeiro lote de plugins
- Data: 2026-06-27.
- Plugins baixados e testados no Paper 26.1.2 build #72:
  - LuckPerms 5.5.57
  - Vault 1.7.3-b131
  - PlaceholderAPI 2.12.2
  - ProtocolLib 5.4.0
  - EssentialsX 2.22.0
  - CoreProtect Community Edition 23.2
- Resultado do boot com plugins: servidor iniciou e chegou a `Done` com 6 plugins inicializados.
- Problema encontrado: CoreProtect 23.2 informou `Minecraft 26.1.2 is not supported` e foi desativado pelo proprio plugin.
- Acao tomada: `CoreProtect-CE-23.2.jar` foi removido de `server/runtime/plugins/` para manter apenas plugins compativeis instalados.
- Estado atual instalado: LuckPerms, Vault, PlaceholderAPI, ProtocolLib e EssentialsX.
- Validacao final: boot curto confirmou `Initialized 5 plugins` e `Done` sem erro critico.
- Observacao: ProtocolLib 5.4.0 carregou, mas avisou que Minecraft 26.1.2 ainda nao foi testado.
- Observacao: o comando `stop` foi enviado, mas Paper 26.1.2 retornou uma excecao no comando de console; o processo foi encerrado manualmente apos a validacao.
