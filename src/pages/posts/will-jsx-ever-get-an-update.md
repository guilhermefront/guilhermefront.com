---
setup: |
  import Layout from '../../layouts/BlogPost.astro'
title: Will JSX ever get an update?
publishDate: 17 Jun 2022
name: Guilherme Samuel
value: 128
description: A quick look into why JSX hasn't been improved in the last few years.
---

Over the years several improvements to JSX have been discussed through the react community. The most popular of them is a shorthand to pass props that have the same name as the variable.

<br />

So instead of writing:

```jsx
const a = 10;
<Example a={a}>
```

You would just do:

```jsx
const a = 10;
<Example {a}>
```  

Looks great, don't it? But it's been [7 years since it was proposed](https://github.com/facebook/jsx/issues/23) and there's no progress on it, why?

## The reason

These improvements doesn't go forward because of mostly three points:
<div class="mb-2" />
1. They still have a bunch of [unanswered questions](https://github.com/facebook/jsx/issues/119#issuecomment-501935701).

2. "One of the biggest strengths of JSX is it's stability, as it's used through several projects." - [Sebastian Marbkage](https://github.com/facebook/jsx/issues/119#issuecomment-501888248)


3. "Any changes to JSX are a lot of work for everyone involved to push through because they need to be coordinated with many partner projects, including Babel, ESLint, Prettier, TypeScript, Flow, IDEs and syntax highlighters, and so on. This doesn’t mean it’s insurmountable, but just that the bar for adding something to the JSX grammar is very high." - [Dan Abramov](https://github.com/reactjs/rfcs/issues/155#issuecomment-620303147)


## Conclusion
With all of this said by important core react team members, the question "will JSX ever get an update" is clearly answered... **Probably not**, unless a working group with members of all these projects come together to vastly discuss and start pushing these improvements, which is something difficult to do when this isn't a priority for them.
