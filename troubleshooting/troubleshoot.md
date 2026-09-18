## All these issue facing while building this :
### 1. Virtualization Issue Encountered
When starting the VM, VirtualBox initially reported `VT-x is disabled in the BIOS for all CPU modes`
**Issue:**
- CPU virtualization was disabled in the computer's BIOS/UEFI configuration.

**Solution:**
- Opened the system BIOS/UEFI settings and enabled `Intel Virtualization Technology → Enabled`

*After enabling virtualization, the VM started successfully*