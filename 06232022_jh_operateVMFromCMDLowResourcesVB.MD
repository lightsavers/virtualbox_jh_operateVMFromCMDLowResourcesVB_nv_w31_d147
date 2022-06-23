```
Author: lightsavers
Created: 06232022
```

# Operate VM from CMD headless for low resources computing

Operating headless VMs from CMD saves computing resources in scarce environments.

# Sample Scenario

1. Put VBoxmanage in user path, under environmental variables

2. Open Command Prompt(CMD)

3. List all available VMs in current environment

```
vboxmanage list vms 
```

4. Start a headless VM

```
vboxmanage startvm "CI-CD" --type headless 
```

5. Pause a VM

```
vboxmanage controlvm "CI-CD" pause --type headless
```

6. Resume a VM

```
vboxmanage controlvm "CI-CD" resume --type headless
```

6. Poweroff a VM

```
vboxmanage controlvm "CI-CD" poweroff --type headless
```

7. Done
