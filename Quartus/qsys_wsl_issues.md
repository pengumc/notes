# Errors when generating QSys in Quartus

```
Error: s0: Error during execution of "{C:/intelfpga_lite/19.1/quartus/../nios2eds/Nios II Command Shell.bat} make all 2>> stderr.txt": child process exited abnormally
```

issue still exists in Quartus 22

Cleanly described here:
https://community.intel.com/t5/Intel-Quartus-Prime-Software/Error-s0-Cannot-find-sequencer-sequencer-elf/td-p/1233588

nios II stuff and the the DDR2 or 3 ram IP need WSL 1, not 2

Show the used version for a system:
```
wsl --list --verbose
```

Use another wsl command to force it to use 1.

https://www.intel.com/content/www/us/en/support/programmable/articles/000074066.html

https://www.intel.com/content/www/us/en/support/programmable/articles/000086438.html