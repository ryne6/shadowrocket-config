# Shadowrocket Config

Shared Shadowrocket rules for macOS and iPhone.

## Files

- `lazy.conf`: primary configuration.
- `modules/claude-us.sgmodule`: optional Claude/Anthropic module.

## Remote URLs

Primary configuration:

```text
https://raw.githubusercontent.com/ryne6/shadowrocket-config/main/lazy.conf
```

Optional Claude module:

```text
https://raw.githubusercontent.com/ryne6/shadowrocket-config/main/modules/claude-us.sgmodule
```

## Design

- Node subscriptions stay inside Shadowrocket and are never committed.
- `US-Auto` dynamically matches node names containing `🇺🇸` or `美国`.
- `TW-Auto` dynamically matches node names containing `🇹🇼`, `台湾`, or `台灣`.
- Claude and Anthropic rules use `US-Auto`.
- Other international rules continue to use the currently selected `PROXY`.

## Safety

Do not commit subscription URLs, node credentials, private keys, certificates, or access tokens.

## Attribution

`lazy.conf` is derived from
[Johnshall/Shadowrocket-ADBlock-Rules-Forever](https://github.com/Johnshall/Shadowrocket-ADBlock-Rules-Forever)
and is shared under CC BY-SA 4.0.
