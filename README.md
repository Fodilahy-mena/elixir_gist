# ElixirGist

# Setup project locally

1. Setup phoenix app, see "Phoenix App" below

## Requirements

- asdf
- Docker

## Build

### PostgreSQL:
For local development, you can use Docker:

```bash
docker run --name bs_db_local -p 5432:5432 -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=your_password -d postgres
```
### Phoenix App:

Install dependencies using asdf and mix
```bash
asdf plugin add erlang
asdf plugin add elixir
asdf plugin add nodejs
asdf install

mix local.hex
mix deps.get
mix ecto.setup

```
To start your Phoenix server:

  * Run `mix setup` to install and setup dependencies
  * Start Phoenix endpoint with `mix phx.server` or inside IEx with `iex -S mix phx.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](https://hexdocs.pm/phoenix/deployment.html).

## Learn more

  * Official website: https://www.phoenixframework.org/
  * Guides: https://hexdocs.pm/phoenix/overview.html
  * Docs: https://hexdocs.pm/phoenix
  * Forum: https://elixirforum.com/c/phoenix-forum
  * Source: https://github.com/phoenixframework/phoenix
