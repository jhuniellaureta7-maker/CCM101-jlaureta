# Virtual Machines vs Containers

**Student Name:** Jhuniel Laureta
**Subject:** CCM101 – Cloud Computing

## Comparison Table

| Category | Virtual Machines (VMs) | Containers |
|---|---|---|
| Architecture | Each VM has its own guest OS and runs on top of a virtualized hardware layer, basically simulating a whole computer. | Containers skip the guest OS entirely — they share the host's kernel and just isolate the app and its dependencies. |
| Boot Time | Booting a VM can take a minute or two since it has to start up a full operating system from scratch. | Containers spin up in seconds because there's no OS to boot — just the app and what it needs. |
| Resource Efficiency | Heavier on RAM and storage since every VM is carrying around its own OS. | Lighter and leaner since containers piggyback on the host OS instead of duplicating it. |
| Isolation Level | Stronger isolation — hardware-level virtualization keeps VMs separated from each other. | Isolation happens at the process level, so it's not as strict as a VM's, but it's usually enough for most apps. |

## Summary

When it comes to deploying web apps, containers are generally the faster and lighter option compared to traditional VMs. Instead of packing a whole operating system, a container just bundles the app with whatever dependencies it needs, while relying on the host OS's kernel underneath. That's why containers tend to boot quicker and use fewer resources than VMs. So for web apps where speed and efficiency matter, containers are a solid alternative worth considering over the traditional VM setup.
