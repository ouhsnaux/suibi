# script 异步加载

`script` 异步加载有两种，分别是 `defer` 和 `async`。

## defer

立即下载，但是等待DOM解析之后再执行

## async

立即下载并执行，但是不阻塞 `DOM` 解析，多个 `script` 文件不保证执行顺序。
