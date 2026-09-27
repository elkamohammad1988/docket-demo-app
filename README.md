# docket-demo-app

A tiny TypeScript pagination helper.

```ts
import { paginate } from "./src/paginate.ts";

paginate(["a", "b", "c", "d", "e"], 2, 2);
// { items: ["c", "d"], page: 2, pageSize: 2, totalItems: 5, totalPages: 3, hasNextPage: true }
```

Pages are 1-indexed. A page past the end returns an empty `items` array.

## Development

Requires Node 22.18 or later (the tests run TypeScript directly, with no build step).

```bash
npm install
npm test         # node:test
npm run typecheck
```
