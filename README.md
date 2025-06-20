## Steps for Reproduction

1. Change account ID in `wrangler.jsonc`

2. Create KV namespace and populate it

   ```bash
   # add to wrangler.jsonc after creation
   pnpm wrangler kv namespace create KV

   # add keys
   pnpm wrangler kv key --binding KV put hello 'world'

   # get key
   pnpm wrangler kv key --binding KV get hello
   ```

3. Run `pnpm run dev` and navigate to the home page.
