# Admin Seguranca

## Alpha Local offline
- O servidor esta em `online-mode=false` e `white-list=false`.
- Qualquer pessoa com acesso ao IP pode tentar entrar.
- AuthMeReloaded protege por senha, mas o nick de admin precisa ser registrado primeiro.
- O dono deve registrar o proprio nick antes de divulgar o IP.
- Use senha forte e nao compartilhe senha.
- Evite nicks simples como `admin`, `dono`, `owner` ou `server`.
- Mantenha OP desativado sempre que possivel.
- Prefira LuckPerms para permissoes.
- Registre todos os comandos executados no console.

## Primeiro acesso do dono
Dentro do Minecraft, usando o nick real do dono:

```text
/register SENHA_FORTE SENHA_FORTE
/login SENHA_FORTE
```

## Permissoes iniciais
Execute no console do servidor, substituindo `SEU_NICK` pelo nick usado dentro do Minecraft:

```text
lp user SEU_NICK permission set luckperms.* true
lp user SEU_NICK permission set essentials.* true
lp user SEU_NICK permission set worldedit.* true
lp user SEU_NICK permission set worldguard.* true
lp user SEU_NICK permission set bluemap.* true
lp user SEU_NICK permission set chunky.* true
```
