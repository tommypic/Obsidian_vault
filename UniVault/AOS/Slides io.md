---
annotation-target: slides.io.pdf
---


>%%
>```annotation-json
>{"created":"2025-11-14T11:38:56.612Z","text":"- bus type is used to represent how the linux kernel can interact with the device\n- bus type is connecting the device and device driver.\n- there is a function in the bus_type that is called match that is called to understand whitch driver should be used for that periferal.\n- **Device Driver Datat structure**\n- probe method: is used fro setting up that the device after the kernel recognise the device driver, after it has been called the kernel can actally use the device.\n- remove, suspend and resume are doing normal.\n\n**Two method for linking a decice to the device driver**\n1. with platform_device name and the list of platform_device_id\n2.  matching is done through the device tree\n","updated":"2025-11-14T11:38:56.612Z","document":{"title":"slides.io.pdf","link":[{"href":"urn:x-pdf:95e45d14f968082a4624771c2efe8636"},{"href":"vault:/AOS/slides.io.pdf"}],"documentFingerprint":"95e45d14f968082a4624771c2efe8636"},"uri":"vault:/AOS/slides.io.pdf","target":[{"source":"vault:/AOS/slides.io.pdf","selector":[{"type":"TextPositionSelector","start":15943,"end":15948},{"type":"TextQuoteSelector","exact":"vance","prefix":"riplet(c) Vittorio Zaccaria | Ad","suffix":"d Operating Systems | Systems ar"}]}]}
>```
>%%
>*%%PREFIX%%riplet(c) Vittorio Zaccaria | Ad%%HIGHLIGHT%% ==vance== %%POSTFIX%%d Operating Systems | Systems ar*
>%%LINK%%[[#^nhnhgq2s36e|show annotation]]
>%%COMMENT%%
>- bus type is used to represent how the linux kernel can interact with the device
>- bus type is connecting the device and device driver.
>- there is a function in the bus_type that is called match that is called to understand whitch driver should be used for that periferal.
>- **Device Driver Datat structure**
>- probe method: is used fro setting up that the device after the kernel recognise the device driver, after it has been called the kernel can actally use the device.
>- remove, suspend and resume are doing normal.
>
>**Two method for linking a decice to the device driver**
>1. with platform_device name and the list of platform_device_id
>2.  matching is done through the device tree
>
>%%TAGS%%
>
^nhnhgq2s36e


>%%
>```annotation-json
>{"created":"2025-11-14T11:49:17.884Z","text":"- Driver informs that can handle different type of devices\n- Driver probe is invoked if i found a matching driver for the device that has been just connected\n- ","updated":"2025-11-14T11:49:17.884Z","document":{"title":"slides.io.pdf","link":[{"href":"urn:x-pdf:95e45d14f968082a4624771c2efe8636"},{"href":"vault:/AOS/slides.io.pdf"}],"documentFingerprint":"95e45d14f968082a4624771c2efe8636"},"uri":"vault:/AOS/slides.io.pdf","target":[{"source":"vault:/AOS/slides.io.pdf","selector":[{"type":"TextPositionSelector","start":16022,"end":16044},{"type":"TextQuoteSelector","exact":"Driver/Device matching","prefix":" group | Politecnico di Milano52","suffix":"(c) Vittorio Zaccaria | Advanced"}]}]}
>```
>%%
>*%%PREFIX%%group | Politecnico di Milano52%%HIGHLIGHT%% ==Driver/Device matching== %%POSTFIX%%(c) Vittorio Zaccaria | Advanced*
>%%LINK%%[[#^j1tvh4q7ok|show annotation]]
>%%COMMENT%%
>- Driver informs that can handle different type of devices
>- Driver probe is invoked if i found a matching driver for the device that has been just connected
>- 
>%%TAGS%%
>
^j1tvh4q7ok


>%%
>```annotation-json
>{"created":"2025-11-14T12:16:48.712Z","text":"Phisically the pcle is like a bus.\nPheriperals can be attached directly to the cpu or to the **cs**.\nSome sort of abstraction need to be given to the kernel to managing devices, so the kernel can see only list of devices collegated with the PCIe connections.\n\nPCIe logical view assigns to each peripheral an address.\nThe host bridge is representig essentialy the **CPU + CS** so that i can see every pheripheral attached to only one thing.\n\nEach device is linked to this host bridge with\n- bus\n- dev\n- fun(if the device has multiple exposed functionalities)\n\nIn this logical view i can see that GPU and SSD are attached to the same host bridge with the same bus this is because cpu and cs are merged.\n\nThe yellow bus of the network is attached with the bus1. to reach the bus i need a routing abstract obj that is called the bridge, when i have multiple busses in my system i have multiple prdges that allow me link theese buses to the root bridge.\n\n","updated":"2025-11-14T12:16:48.712Z","document":{"title":"slides.io.pdf","link":[{"href":"urn:x-pdf:95e45d14f968082a4624771c2efe8636"},{"href":"vault:/AOS/slides.io.pdf"}],"documentFingerprint":"95e45d14f968082a4624771c2efe8636"},"uri":"vault:/AOS/slides.io.pdf","target":[{"source":"vault:/AOS/slides.io.pdf","selector":[{"type":"TextPositionSelector","start":17505,"end":17550},{"type":"TextQuoteSelector","exact":"The PCI bus framework » Logical/Physical view","prefix":" group | Politecnico di Milano56","suffix":"(c) Vittorio Zaccaria | Advanced"}]}]}
>```
>%%
>*%%PREFIX%%group | Politecnico di Milano56%%HIGHLIGHT%% ==The PCI bus framework » Logical/Physical view== %%POSTFIX%%(c) Vittorio Zaccaria | Advanced*
>%%LINK%%[[#^uquv5h2v9m|show annotation]]
>%%COMMENT%%
>Phisically the pcle is like a bus.
>Pheriperals can be attached directly to the cpu or to the **cs**.
>Some sort of abstraction need to be given to the kernel to managing devices, so the kernel can see only list of devices collegated with the PCIe connections.
>
>PCIe logical view assigns to each peripheral an address.
>The host bridge is representig essentialy the **CPU + CS** so that i can see every pheripheral attached to only one thing.
>
>Each device is linked to this host bridge with
>- bus
>- dev
>- fun(if the device has multiple exposed functionalities)
>
>In this logical view i can see that GPU and SSD are attached to the same host bridge with the same bus this is because cpu and cs are merged.
>
>The yellow bus of the network is attached with the bus1. to reach the bus i need a routing abstract obj that is called the bridge, when i have multiple busses in my system i have multiple prdges that allow me link theese buses to the root bridge.
>
>
>%%TAGS%%
>
^uquv5h2v9m
