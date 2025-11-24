---
annotation-target: slides.kvm.pdf
---


>%%
>```annotation-json
>{"created":"2025-11-24T11:47:40.425Z","text":"**Virutalization in embedded system**\nVirtualization is now entering the embedded sysme and automotive sectro for example, it is  a thecnology that is evelving\n","updated":"2025-11-24T11:47:40.425Z","document":{"title":"slides.kvm.pdf","link":[{"href":"urn:x-pdf:48349584fb6147ebc8ddcf9e94e7605b"},{"href":"vault:/AOS/slides.kvm.pdf"}],"documentFingerprint":"48349584fb6147ebc8ddcf9e94e7605b"},"uri":"vault:/AOS/slides.kvm.pdf","target":[{"source":"vault:/AOS/slides.kvm.pdf","selector":[{"type":"TextPositionSelector","start":2289,"end":2304},{"type":"TextQuoteSelector","exact":"virtual machine","prefix":"p | Politecnico di Milano4Why a ","suffix":"Consolidate and partition hardwa"}]}]}
>```
>%%
>*%%PREFIX%%p | Politecnico di Milano4Why a%%HIGHLIGHT%% ==virtual machine== %%POSTFIX%%Consolidate and partition hardwa*
>%%LINK%%[[#^mr2mxu90mp|show annotation]]
>%%COMMENT%%
>**Virutalization in embedded system**
>Virtualization is now entering the embedded sysme and automotive sectro for example, it is  a thecnology that is evelving
>
>%%TAGS%%
>
^mr2mxu90mp


>%%
>```annotation-json
>{"created":"2025-11-24T11:49:15.478Z","text":"- Translate the access to physical resources into safe actions for the VM, for example the monitor can translate the request of the VM interrupts to a correct and safer version, so that the vm can have its own interrupts handler\n","updated":"2025-11-24T11:49:15.478Z","document":{"title":"slides.kvm.pdf","link":[{"href":"urn:x-pdf:48349584fb6147ebc8ddcf9e94e7605b"},{"href":"vault:/AOS/slides.kvm.pdf"}],"documentFingerprint":"48349584fb6147ebc8ddcf9e94e7605b"},"uri":"vault:/AOS/slides.kvm.pdf","target":[{"source":"vault:/AOS/slides.kvm.pdf","selector":[{"type":"TextPositionSelector","start":2934,"end":2977},{"type":"TextQuoteSelector","exact":"Virtual machine monitor (VMM) or Hypervisor","prefix":"ns on top of the virtual machine","suffix":":Software program that translate"}]}]}
>```
>%%
>*%%PREFIX%%ns on top of the virtual machine%%HIGHLIGHT%% ==Virtual machine monitor (VMM) or Hypervisor== %%POSTFIX%%:Software program that translate*
>%%LINK%%[[#^yc86wqso0yq|show annotation]]
>%%COMMENT%%
>- Translate the access to physical resources into safe actions for the VM, for example the monitor can translate the request of the VM interrupts to a correct and safer version, so that the vm can have its own interrupts handler
>
>%%TAGS%%
>
^yc86wqso0yq


>%%
>```annotation-json
>{"created":"2025-11-24T11:51:22.842Z","text":"- for example kvm is a type 2 hypervisonr.\n- an example for the type 1 is \n- A type 2 hypervisor is much more simpler, a type 1 need to have all the drivers available, the type 2 can use the one of the hosting os.\n","updated":"2025-11-24T11:51:22.842Z","document":{"title":"slides.kvm.pdf","link":[{"href":"urn:x-pdf:48349584fb6147ebc8ddcf9e94e7605b"},{"href":"vault:/AOS/slides.kvm.pdf"}],"documentFingerprint":"48349584fb6147ebc8ddcf9e94e7605b"},"uri":"vault:/AOS/slides.kvm.pdf","target":[{"source":"vault:/AOS/slides.kvm.pdf","selector":[{"type":"TextPositionSelector","start":3112,"end":3128},{"type":"TextQuoteSelector","exact":"Type 1 Hyperviso","prefix":"processor stateEnsures isolation","suffix":"r: Also called native hypervisor"}]}]}
>```
>%%
>*%%PREFIX%%processor stateEnsures isolation%%HIGHLIGHT%% ==Type 1 Hyperviso== %%POSTFIX%%r: Also called native hypervisor*
>%%LINK%%[[#^kf8tale8f0i|show annotation]]
>%%COMMENT%%
>- for example kvm is a type 2 hypervisonr.
>- an example for the type 1 is 
>- A type 2 hypervisor is much more simpler, a type 1 need to have all the drivers available, the type 2 can use the one of the hosting os.
>
>%%TAGS%%
>
^kf8tale8f0i


>%%
>```annotation-json
>{"created":"2025-11-24T12:04:29.882Z","text":"i can have a vm if :\nwhenever the guest os execute a sensitive instruction it traps them in hypervisor. For example now we have hardware support for virtualization.\nPractically speaking ","updated":"2025-11-24T12:04:29.882Z","document":{"title":"slides.kvm.pdf","link":[{"href":"urn:x-pdf:48349584fb6147ebc8ddcf9e94e7605b"},{"href":"vault:/AOS/slides.kvm.pdf"}],"documentFingerprint":"48349584fb6147ebc8ddcf9e94e7605b"},"uri":"vault:/AOS/slides.kvm.pdf","target":[{"source":"vault:/AOS/slides.kvm.pdf","selector":[{"type":"TextPositionSelector","start":3396,"end":3420},{"type":"TextQuoteSelector","exact":"Terminology and theorems","prefix":"e group | Politecnico di Milano6","suffix":"Instruction types: Unprivileged "}]}]}
>```
>%%
>*%%PREFIX%%e group | Politecnico di Milano6%%HIGHLIGHT%% ==Terminology and theorems== %%POSTFIX%%Instruction types: Unprivileged*
>%%LINK%%[[#^tgc7nidazij|show annotation]]
>%%COMMENT%%
>i can have a vm if :
>whenever the guest os execute a sensitive instruction it traps them in hypervisor. For example now we have hardware support for virtualization.
>Practically speaking 
>%%TAGS%%
>
^tgc7nidazij


>%%
>```annotation-json
>{"created":"2025-11-24T12:12:53.409Z","text":"- **Hardware based**\nNot everything that the guest does in the supervisor has to been trap to the virutal machine of the hypervisor.\nIn some case i need that the execution of the su on the guest is stopped and the vm is emulated.\nFor example i have that i want to write in io port of a device, so in those case i exit the guest mode and the virtual machine monitor takes place and start emulating.\nThere is a data structure whitch is used to stop and starting the guest, is used for stroing the register so that the monitor can resume the guest correctly.\n\nWith hardware based i am calling the vmm very less time, i have much better performance.\n","updated":"2025-11-24T12:12:53.409Z","document":{"title":"slides.kvm.pdf","link":[{"href":"urn:x-pdf:48349584fb6147ebc8ddcf9e94e7605b"},{"href":"vault:/AOS/slides.kvm.pdf"}],"documentFingerprint":"48349584fb6147ebc8ddcf9e94e7605b"},"uri":"vault:/AOS/slides.kvm.pdf","target":[{"source":"vault:/AOS/slides.kvm.pdf","selector":[{"type":"TextPositionSelector","start":4264,"end":4279},{"type":"TextQuoteSelector","exact":"c) Vittorio Zac","prefix":"ware vs software virtualization(","suffix":"caria | Advanced Operating Syste"}]}]}
>```
>%%
>*%%PREFIX%%ware vs software virtualization(%%HIGHLIGHT%% ==c) Vittorio Zac== %%POSTFIX%%caria | Advanced Operating Syste*
>%%LINK%%[[#^yezf2qphcih|show annotation]]
>%%COMMENT%%
>- **Hardware based**
>Not everything that the guest does in the supervisor has to been trap to the virutal machine of the hypervisor.
>In some case i need that the execution of the su on the guest is stopped and the vm is emulated.
>For example i have that i want to write in io port of a device, so in those case i exit the guest mode and the virtual machine monitor takes place and start emulating.
>There is a data structure whitch is used to stop and starting the guest, is used for stroing the register so that the monitor can resume the guest correctly.
>
>With hardware based i am calling the vmm very less time, i have much better performance.
>
>%%TAGS%%
>
^yezf2qphcih


>%%
>```annotation-json
>{"created":"2025-11-24T12:19:43.597Z","text":"In a guest OS i have \n- SU in ring 1\n- user in ring 3\nWith this config i can differentiate the two modes.\n","updated":"2025-11-24T12:19:43.597Z","document":{"title":"slides.kvm.pdf","link":[{"href":"urn:x-pdf:48349584fb6147ebc8ddcf9e94e7605b"},{"href":"vault:/AOS/slides.kvm.pdf"}],"documentFingerprint":"48349584fb6147ebc8ddcf9e94e7605b"},"uri":"vault:/AOS/slides.kvm.pdf","target":[{"source":"vault:/AOS/slides.kvm.pdf","selector":[{"type":"TextPositionSelector","start":4619,"end":4631},{"type":"TextQuoteSelector","exact":"Introduction","prefix":" group | Politecnico di Milano10","suffix":"Software-based virtualization me"}]}]}
>```
>%%
>*%%PREFIX%%group | Politecnico di Milano10%%HIGHLIGHT%% ==Introduction== %%POSTFIX%%Software-based virtualization me*
>%%LINK%%[[#^e8pj7sqw8im|show annotation]]
>%%COMMENT%%
>In a guest OS i have 
>- SU in ring 1
>- user in ring 3
>With this config i can differentiate the two modes.
>
>%%TAGS%%
>
^e8pj7sqw8im


>%%
>```annotation-json
>{"created":"2025-11-24T12:55:28.532Z","text":"in vtx i have that the mapping of the registers are not ","updated":"2025-11-24T12:55:28.532Z","document":{"title":"slides.kvm.pdf","link":[{"href":"urn:x-pdf:48349584fb6147ebc8ddcf9e94e7605b"},{"href":"vault:/AOS/slides.kvm.pdf"}],"documentFingerprint":"48349584fb6147ebc8ddcf9e94e7605b"},"uri":"vault:/AOS/slides.kvm.pdf","target":[{"source":"vault:/AOS/slides.kvm.pdf","selector":[{"type":"TextPositionSelector","start":7848,"end":7859},{"type":"TextQuoteSelector","exact":" intel VT-x","prefix":"Politecnico di Milano21Example »","suffix":" » Extended page tables(c) Vitto"}]}]}
>```
>%%
>*%%PREFIX%%Politecnico di Milano21Example »%%HIGHLIGHT%% ==intel VT-x== %%POSTFIX%%» Extended page tables(c) Vitto*
>%%LINK%%[[#^mt5n3xiwmps|show annotation]]
>%%COMMENT%%
>in vtx i have that the mapping of the registers are not 
>%%TAGS%%
>
^mt5n3xiwmps


>%%
>```annotation-json
>{"created":"2025-11-24T13:00:13.881Z","text":"every vm runs as a thread in the kernle,\n- you start the vm\n- you get the vmEntry","updated":"2025-11-24T13:00:13.881Z","document":{"title":"slides.kvm.pdf","link":[{"href":"urn:x-pdf:48349584fb6147ebc8ddcf9e94e7605b"},{"href":"vault:/AOS/slides.kvm.pdf"}],"documentFingerprint":"48349584fb6147ebc8ddcf9e94e7605b"},"uri":"vault:/AOS/slides.kvm.pdf","target":[{"source":"vault:/AOS/slides.kvm.pdf","selector":[{"type":"TextPositionSelector","start":8848,"end":8859},{"type":"TextQuoteSelector","exact":"Introductio","prefix":" group | Politecnico di Milano25","suffix":"n(c) Vittorio Zaccaria | Advance"}]}]}
>```
>%%
>*%%PREFIX%%group | Politecnico di Milano25%%HIGHLIGHT%% ==Introductio== %%POSTFIX%%n(c) Vittorio Zaccaria | Advance*
>%%LINK%%[[#^9bdjsvmf3p8|show annotation]]
>%%COMMENT%%
>every vm runs as a thread in the kernle,
>- you start the vm
>- you get the vmEntry
>%%TAGS%%
>
^9bdjsvmf3p8
