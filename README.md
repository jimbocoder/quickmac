

## quickmac

A reasonable, quick default mac setup, the way I like things. I'll try to be flexible at the same time so it is useful to others without being too opinionated.

### prerequisites

1. Install MacOS command-line developer tools (ie. Install "XCode Dev Tools" in the app store)
1. `pip3 install --user ansible`
1. Add `~/Library/Python/3.8/bin` to your path, so ansible can be found

### setup

`ansible-galaxy install -r requirements.yml`

### setup

`ansible-galaxy install -r requirements.yml`

### usage


put your sudo password into `become-pass.txt`

First run basics.yml

Reboot

Then run playbook.yml

See what would change:
```
ansible-playbook playbook.yml --check --diff
```


If you like what you see, apply:
```
ansible-playbook playbook.yml --diff
```


### TODO list

1. [x] defaults write -g InitialKeyRepeat -float 10.0 # normal minimum is 15 (225 ms)
1. [x] defaults write -g KeyRepeat -float 1.0 # normal minimum is 2 (30 ms)
1. [ ] defaults write -g ApplePressAndHoldEnabled -bool false
1. [ ] Make a plist to run `/usr/libexec/locate.updatedb` as root periodically so `locate` stays reasonably fresh
1. [ ] Disable natural trackpad scroll direction
1. [ ] disable "smart" quotes and dashes
1. [ ] 3-finger drag
1. [ ] install and configure moom/amethyst

