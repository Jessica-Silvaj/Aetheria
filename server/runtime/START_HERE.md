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
- Estado funcional confirmado: servidor iniciou e chegou a `Done` com 5 plugins carregados.
- Instalados: LuckPerms, Vault, PlaceholderAPI, ProtocolLib e EssentialsX.
- ProtocolLib 5.4.0 esta instalado, mas carregou com aviso de que Minecraft 26.1.2 ainda nao foi testado.
- CoreProtect 23.2 esta pendente/incompativel temporariamente: informou `Minecraft 26.1.2 is not supported` e foi removido de `server/runtime/plugins/`.
- Nao reinstalar CoreProtect ate existir uma versao compativel com Paper/Minecraft 26.1.2 ou ate a versao do Paper ser reavaliada.
- Observacao: em um teste anterior, o comando `stop` no console do Paper 26.1.2 gerou excecao.

## Registro do segundo lote de plugins
- Data: 2026-06-27.
- Plugins instalados e testados no Paper 26.1.2 build #72:
  - WorldEdit 7.4.3
  - WorldGuard 7.0.16
  - Chunky 1.5.3
  - BlueMap 5.22
- Resultado: servidor iniciou e chegou a `Done` com 9 plugins carregados.
- Parada: comando `stop` executado e servidor salvo/desligado.
- Avisos: ProtocolLib 5.4.0 segue com aviso de versao nao testada; BlueMap precisa aceitar o download de recursos em `plugins/BlueMap/core.conf`; Essentials gerou aviso de tarefa assincrona durante shutdown.
- CoreProtect continua pendente/incompativel e nao deve ser reinstalado agora.
