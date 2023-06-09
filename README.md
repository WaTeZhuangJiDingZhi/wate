USB restriction patches for MacOS11 to 14 systems, Check XhciPortLimit and then all USB ports can be used, breaking the limit of 15 ports
<img width="986" alt="截屏2023-06-10 上午5 36 30" src="https://github.com/WaTeZhuangJiDingZhi/wate/assets/134581706/256b137a-6afa-47bd-93da-9b755a7accc5">
**Problem:**

The XhciPortLimit patch is invalid from 11.2.3+ onwards. USB is limited to 15 by macOS

**Solution:**

Check the 2 patches and XhciPortLimit to remove the restriction, and hope to integrate it into opencore
**Patch Details:**
