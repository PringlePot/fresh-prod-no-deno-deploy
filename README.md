# fresh in prod, without deno deploy

### How to use in prod?

Set the DENO_DEPLOYMENT_ID to a random string

```sh
# This sets it to a random string
export DENO_DEPLOYMENT_ID=$RANDOM | md5sum | head -c 20
```

Then start the server

```
deno run -A main.ts
```

This will make fresh think its running on deno deploy.

### Dev Usage

Start the project:

```
deno task start
```

This will watch the project directory and restart as necessary.
