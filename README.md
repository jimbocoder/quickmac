

## quickmac

A reasonable, quick default mac setup, the way I like things. I'll try to be flexible at the same time so it is useful to others without being too opinionated.

### prerequisites

You have `ansible-playbook` installed.

### usage


See what would change:
```
ansible-playbook playbook.yml --check --diff
```


If you like what you see, apply:
```
ansible-playbook playbook.yml --diff
```


### TODO list

1. [ ] defaults write -g InitialKeyRepeat -float 10.0 # normal minimum is 15 (225 ms)
1. [ ] defaults write -g KeyRepeat -float 1.0 # normal minimum is 2 (30 ms)

