# Initial setup

This installs the basics needed for a developer. I don't have a lot of descriptions, so you'll have to Google/DuckDuckGo/.. things if you want to know what it is, or if you're stuck.

## Homebrew
Install Homebrew

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
You should be prompted to install dependencies, such as the x-code command line tools. This may take a while. Several of the next steps are dependent on this one, so just be patient.

Make sure to do the *next steps*, which at the time of writing this was:
```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/svennhv/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

Note:
Brew `cask` commands have been deprecated. Now `--cask` is used instead.

## Rosetta 

You might need rosetta for some things, to run with an emulated x86 architecture:
`softwareupdate --install-rosetta`

## Oh-my-zsh

Install *oh-my-zsh*:
`sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

## Window Manager Amethyst

`brew install --cask amethyst`

Amethyst must be given permissions to use the accessibility APIs under the Privacy tab of the Security & Privacy preferences. Check the link if you're lost: https://github.com/ianyh/Amethyst

## Docker
Install Docker from here: https://docs.docker.com/desktop/mac/apple-silicon/ 

This is a good sign:
"Docker Desktop for Apple silicon also supports multi-platform images, which allows you to build and run images for both x86 and ARM architectures without having to set up a complex cross-compilation development environment. "
(I had some issues with Neo4j last time I installed it using Docker. But maybe it works now)

## Settings in MacOS
I would recommend fixing the following.
**More space:**
cmd+space, then write `displays`. Select "scaled". Select "more space". This is if you're able to read stuff.

**Hide the dock:**
cmd+space, then write `dock & menu bar`. Position: *right*. Select "Automatically hide and show ..". This seems to interfere the least, and give more room for work.

