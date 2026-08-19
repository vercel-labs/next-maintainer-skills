# Next.js Maintainer Skills

Portable agent skills for investigating and fixing issues in
[`vercel/next.js`](https://github.com/vercel/next.js).

## Install

Install all skills:

```bash
npx skills add vercel-labs/next-maintainer-skills --skill '*'
```

Install one skill:

```bash
npx skills add vercel-labs/next-maintainer-skills \
  --skill nextjs-reproduce-issue
```

## Skills

- `nextjs-reproduce-issue` — produce and validate a minimal reproduction.
- `nextjs-verify-canary` — compare the reported version with `next@canary`.
- `nextjs-bisect-regression` — locate an introduction or fix boundary.
- `nextjs-create-regression-test` — add the smallest relevant regression test.
- `nextjs-fix-issue` — implement and validate the smallest correct fix.

These skills are tool-agnostic. They use the shell, browser, GitHub, and other
capabilities available in the agent that installs them.

## Development

When updating a skill, keep its `SKILL.md` instructions and any referenced
scripts or assets in sync.
