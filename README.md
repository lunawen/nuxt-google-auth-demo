# nuxt-google-auth-demo

## Luna 说

这个 demo 结合了 google oauth 来做 sign-in，你需要根据教程来创建一个 google oAuth clientID，然后确保以下三件事：

1. 这个 app 里面的配置文件正确（修改 nuxt.config.js 里面的 google client id）；
2. google 配置的端口和你 app 运行的端口一致；
3. 你的 google user 被加入到了 test user 里面。

PS：我删掉了很多跟 demo 无关的文件。

## Run Project

```bash
cd nuxt-google-auth-demo
npm install
npm run dev
```