
Make sure to do the initial setup first.

## Install the asdf version manager

Install `asdf` using Brew:
`brew install asdf`

Make sure to follow the step adding asdf to your zsh config:
"To use asdf, add the following line to your ~/.zshrc:
`. /opt/homebrew/opt/asdf/libexec/asdf.sh` 
"

Add the erlang and elixir plugins:
```
asdf plugin-add erlang
asdf plugin-add elixir
```

## Installing Elixir

```
asdf install erlang 24.1.2
asdf global erlang 24.1.2
asdf install elixir 1.12.3-otp-24
asdf global elixir 1.12.3-otp-24
```

Install Hex:
`mix local.hex`

## Installing Phoenix

Run:
`mix archive.install hex phx_new`

## Issues with Node

Getting some issues with Sass. To fix it, go to the assets folder and run:
`npm install node-sass@npm:sass`
Then run the ordinary `npm install` to install the rest. 

# NEXT
Then I went to installing the Postgres database. See the database-setup file.

# Working Notes 

Todo:
- Check Erlang installation output. See if there are any necessary things to fix there.

Articles:
- https://medium.com/@miguel.coba/creating-a-phoenix-1-6-application-with-asdf-f7a4e7b46ba0

