## This Repo explores the issues with using `tsx watch` with Epic Stack/Remix in a Windows environment

* Reference: https://github.com/remix-run/remix/pull/6538

The main branch is a vanilla Epic Stack installed with:

 `npx create-remix@latest --typescript --install --template epicweb-dev/epic-stack`

 Run `npm run dev` to get the app started.


The following branches demonstrate the issues:

* `tsx watch` without editing stdio: https://github.com/xHomu/epic-stack-tsx-watch-bug/tree/tsx-watch-no-child-process
* `ts-node` alternative https://github.com/xHomu/epic-stack-tsx-watch-bug/tree/ts-node
