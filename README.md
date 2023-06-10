## This branch uses `ts-node with nodemon` as alternative to TSX

ts-node with nodemon doesn't experience the same issue as `tsx watch`, and we can mostly make up the performance difference with the swc plugin by adding `{ "ts-node": { "swc": true } }` to `tsconfig.json`:

![image](https://github.com/remix-run/remix/assets/84349818/8bd797ea-0fd8-407a-ab94-606b774e9dee)
