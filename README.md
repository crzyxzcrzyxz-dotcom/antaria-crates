# Antaria Crates

Analisem a pasta do plugin que estou a enviar e recriem este plugin do zero em Java (para Spigot/Paper/Folia 1.20+ que funcione na 1.21.11 tambem ja que estamos em 2026) com o nome "AntariaCrates", corrigindo e adicionando exatamente o seguinte:

1. Hologramas Per-Player (Individuais por Jogador):

   - Corrijam o bug visual onde a contagem de chaves (%crate_keys_...%) no holograma altera para todos quando alguém usa a caixa. O holograma no topo do bloco deve ser renderizado individualmente para cada jogador (per-player holograms) usando Display Entities nativas do Minecraft ou suporte a FancyHolograms/DecentHolograms.

2. Comando de Chaves Individuais:

   - Adicionem um comando para dar chaves a um jogador específico em vez de existir apenas o keyall:

     /antariacrates give <jogador> <caixa> <quantidade>

   - Mantenham os comandos normais de giveall, take, set e balance de chaves.

Mantenham exatamente o mesmo formato de ficheiros YAML, lógica das caixas (GUI, CHOOSE mode, rewards, trims, custom-model-data) e suporte ao Folia que a pasta atual já possui, alterando apenas os comandos e a lógica do holograma para ser per-player.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/06aaf200-3c5c-404b-bb5a-d71a4ec77a36).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
