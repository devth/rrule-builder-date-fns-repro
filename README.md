This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Repo type error

```bash
npm run tsc
```

### Result

```
> rrule-builder-date-fns-repro@0.1.0 tsc
> tsc

node_modules/react-rrule-builder-ts/src/components/RRuleBuilder/RRuleBuilder.tsx(20,58): error TS2344: Type 'TDate' does not satisfy the constraint 'Date'.
node_modules/react-rrule-builder-ts/src/components/RRuleBuilder/RRuleBuilder.tsx(135,29): error TS2322: Type 'new (...args: any[]) => MuiPickersAdapter<TDate, any>' is not assignable to type 'new (...args: any) => MuiPickersAdapter<Date, any>'.
  Type 'MuiPickersAdapter<TDate, any>' is not assignable to type 'MuiPickersAdapter<Date, any>'.
    Type 'TDate' is not assignable to type 'Date'.
node_modules/react-rrule-builder-ts/src/store/builderStore.tsx(5,19): error TS7016: Could not find a declaration file for module 'lodash/isNil'. '/Users/devth/oss/rrule-builder-date-fns-repro/node_modules/lodash/isNil.js' implicitly has an 'any' type.
  Try `npm i --save-dev @types/lodash` if it exists or add a new declaration (.d.ts) file containing `declare module 'lodash/isNil';`
node_modules/react-rrule-builder-ts/src/store/builderStore.tsx(19,35): error TS2344: Type 'TDate' does not satisfy the constraint 'Date'.
node_modules/react-rrule-builder-ts/src/store/builderStore.tsx(29,47): error TS2344: Type 'TDate' does not satisfy the constraint 'Date'.
node_modules/react-rrule-builder-ts/src/store/builderStore.tsx(168,20): error TS2345: Argument of type 'Frequency | undefined' is not assignable to parameter of type 'Frequency'.
  Type 'undefined' is not assignable to type 'Frequency'.
node_modules/react-rrule-builder-ts/src/utils/buildRRuleString.ts(11,34): error TS2344: Type 'TDate' does not satisfy the constraint 'Date'.
```

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
