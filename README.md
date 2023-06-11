USB restriction patches for MacOS11 to 14 systems, Check XhciPortLimit and then all USB ports can be used, breaking the limit of 15 ports
<img width="986" alt="截屏2023-06-10 上午5 36 30" src="https://github.com/WaTeZhuangJiDingZhi/wate/assets/134581706/256b137a-6afa-47bd-93da-9b755a7accc5">

**Problem:**

The XhciPortLimit patch is invalid from 11.2.3+ onwards. USB is limited to 15 by macOS

**Solution:**

Check the 2 patches and XhciPortLimit to remove the restriction, and hope to integrate it into opencore
**Patch Details:**

当然 你还需要给原来的USB端口补丁取消，重新注入USBInjectAll.kext或者XHCI-unsupported.kext（最高支持Z690）
USBToolBox.kext+UTBMap.kext (适用于700和AMD)

Of course, you still need to cancel the original USB port patch and re-inject USBInjectAll.kext or XHCI-unsupported.kext (up to Z690)
USBToolBox.kext+UTBMap.kext (for 700 and AMD)


抱歉Sonoma apple已经更换补丁，我需要重新查找，所以以上补丁适用于11-13，Sonoma的 我准备重新查找，最近比较忙。有x86汇编专家协助我就好了。微信：zmlk1213 请与我联系

Sorry Sonoma apple has changed the patch, I need to search again, so the above patch is applicable to 11-13, Sonoma I am going to search again, I am busy recently. It would be nice to have an x86 assembler expert assist me. WeChat: zmlk1213 Please contact me
