# Orinion_Way_AI_ugynoko

Az Orinion Way AI ügynökének projektje (`@orinion-way/ai-ugynok`). [Nx](https://nx.dev)-szel generált TypeScript library ebben a monorepóban; a felépítése a `@plantbase/core` mintáját követi (lásd `docs/konvenciok.md`).

## Parancsok

```bash
pnpm nx build orinion-way-ai-ugynok       # build (tsc → dist/)
pnpm nx test orinion-way-ai-ugynok        # unit tesztek (Vitest)
pnpm nx lint orinion-way-ai-ugynok
pnpm nx typecheck orinion-way-ai-ugynok
```

## Használat a workspace-en belül

```ts
import { orinionWayAiUgynok } from '@orinion-way/ai-ugynok';
```

DEV-ben (`tsx --conditions=@plantbase/source`) a csomag közvetlenül a TypeScript forrásból (`src/index.ts`) oldódik fel, build nélkül — ugyanúgy, mint a `@plantbase/core`.
