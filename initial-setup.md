# Initial setup

This installs the basics needed for a developer.

## Basic dependencies and some nice to have's
Install Homebrew

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
You should be prompted to install dependencies, such as the x-code command line tools. This may take a while. Several of the next steps are dependent on this one, so just be patient.

Install *oh-my-zsh*:
`sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

Install x-code command line tools:
`xcode-select --install`
Then install. Run `xcode-select -p` and the output should be `/Library/Developer/CommandLineTools`

