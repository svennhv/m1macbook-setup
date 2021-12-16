
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


# NEXT
Then I went to installing the Postgres database. See the database-setup file.

# Working Notes 

Todo:
- Check Erlang installation output. See if there are any necessary things to fix there.

## Erlang installation output

I got this. Seems like there is no Java compiler. Not sure if it matters.

Missing:
- jinterface: No Java compiler
- odbc: Link check failed
- wxWidgets
- fop missing
```
Building Erlang/OTP 24.1.2 (asdf_24.1.2), please wait...
APPLICATIONS DISABLED (See: /Users/svennhv/.asdf/plugins/erlang/kerl-home/builds/asdf_24.1.2/otp_build_24.1.2.log)
 * jinterface     : No Java compiler found
 * odbc           : ODBC library - link check failed

APPLICATIONS INFORMATION (See: /Users/svennhv/.asdf/plugins/erlang/kerl-home/builds/asdf_24.1.2/otp_build_24.1.2.log)
 * wx             : wxWidgets was not compiled with --enable-webview or wxWebView developer package is not installed, wxWebView will NOT be available
 *         wxWidgets must be installed on your system.
 *         Please check that wx-config is in path, the directory
 *         where wxWidgets libraries are installed (returned by
 *         'wx-config --libs' or 'wx-config --static --libs' command)
 *         is in LD_LIBRARY_PATH or equivalent variable and
 *         wxWidgets version is 3.0.2 or above.

DOCUMENTATION INFORMATION (See: /Users/svennhv/.asdf/plugins/erlang/kerl-home/builds/asdf_24.1.2/otp_build_24.1.2.log)
 * documentation  : 
 *                  fop is missing.
 *                  Using fakefop to generate placeholder PDF files.

Erlang/OTP 24.1.2 (asdf_24.1.2) has been successfully built
Installing Erlang/OTP 24.1.2 (asdf_24.1.2) in /Users/svennhv/.asdf/installs/erlang/24.1.2...
You can activate this installation running the following command:
. /Users/svennhv/.asdf/installs/erlang/24.1.2/activate
Later on, you can leave the installation typing:
kerl_deactivate
Cleaning up compilation products for 
Cleaned up compilation products for  under /Users/svennhv/.asdf/plugins/erlang/kerl-home/builds
ln: ./erl_call: File exists


Articles:
- https://medium.com/@miguel.coba/creating-a-phoenix-1-6-application-with-asdf-f7a4e7b46ba0

