Talk: Observable Elixir Services
================================

## Cheatsheet (fish shell)

Generate simple Phoenix service with HTTP API:

```
mix archive.install hex phx_new 1.4.8
mix phx.new demo \
  --umbrella --no-html --no-webpack --no-ecto
```

Test locally:
```
forego run iex -S mix phx.server
http -v :4000/calls from=1111 to=2222
http -v :4000/calls/ea2c6243-6858-4d5d-8287-4e39d6b5141d/actions/play url="http://example.com/hello.mp3"
```

Run release: 
```
env MIX_ENV=prod mix release
forego run _build/prod/rel/demo/bin/demo foreground
```
