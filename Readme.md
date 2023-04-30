# Open AI - API Proxy


### Using with node SDK
```diff
import { Configuration } from "openai";

const configuration = new Configuration({
  apiKey: OPENAI_API_KEY,
+ basePath: "https://closeai.deno.dev/v1",
});
```

### Using with Python SDK

```diff
  import openai

  openai.api_key = os.getenv("OPENAI_API_KEY")
+ openai.api_base = "https://closeai.deno.dev/v1"
```

### Usage
```bash
deno run --allow-net --allow-read --allow-env --watch main.ts
```

### One click deployment
https://dash.deno.com/new?url=https://raw.githubusercontent.com/justjavac/openai-proxy/main/main.ts
