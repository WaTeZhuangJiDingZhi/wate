USB restriction patches for MacOS11 to 14 systems, Check XhciPortLimit and then all USB ports can be used, breaking the limit of 15 ports
<img width="986" alt="截屏2023-06-10 上午5 36 30" src="https://github.com/WaTeZhuangJiDingZhi/wate/assets/134581706/256b137a-6afa-47bd-93da-9b755a7accc5">
Patch Details:

Identifier	com.apple.iokit.IOUSBHostFamily
Base	__ZN11IOPCIBridge20addBridgeMemoryRangeEyyb
Comment	Wate - Fix XhciPortLimit in 12.3+
Find	EB0A4183 E60F41D3
Replace	EB0A4183 E63F41D3
MinKernel	20.0.0
Count	1
Enabled	True
