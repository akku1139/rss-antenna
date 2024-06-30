# rss-antenna

TODO: 書く

Cloudflare Pages対応です

多分

```ts
import { Hono } from "hono"
import { antenna, scheduled } from "rss-antenna"
const app = new Hono()

app.route("/", antenna({
  title: "アンテナ名",
}))

export default {
  fetch: app.fetch,
  scheduled,
}
```

みたいな感じで動くように作ります
