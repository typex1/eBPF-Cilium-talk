# eBPF-Cilium-talk
Resources of my talk on eBPF and Cilium

To enable you to review the contents and redo the demos I showed during my talk, please find the resources here:

## eBPF

* Thomas Graf (Isovalent): "eBPF - Everything you need to now in 5 minutes" [https://youtu.be/KhPrMW5Rbbc](https://youtu.be/KhPrMW5Rbbc)
* Official eBPF sources: [https://en.wikipedia.org/wiki/EBPF](https://en.wikipedia.org/wiki/EBPF), [https://ebfp.io](https://ebfp.io)
* Brendan Gregg (Netflix): Performance Wins with eBPF https://www.youtube.com/watch?v=bGAVrtb_tFs
* Who is using eBPF? [https://www.infoq.com/articles/ebpf-cloud-native-platforms/](https://www.infoq.com/articles/ebpf-cloud-native-platforms/)
* Since when is eBPF available? Since Linux kernel 3.15: [https://github.com/iovisor/bcc](https://github.com/iovisor/bcc)

## BCC = BPF Compiler Collection

* Installation and usage: [https://github.com/iovisor/bcc](https://github.com/iovisor/bcc)
* Hello World example from slides: [https://github.com/iovisor/bcc/blob/master/examples/hello_world.py](https://github.com/iovisor/bcc/blob/master/examples/hello_world.py)
* Available Linux system calls: [https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md](https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md)
* Hello World with map / ring buffer to persist e.g. a counter variable: [https://gist.github.com/lizrice/47ad44a15cce912502f8667a403f5649](https://gist.github.com/lizrice/47ad44a15cce912502f8667a403f5649)
* Precompiled binaries in BCC: e.g. "sudo /usr/share/bcc/tools/execsnoop"
* eBPF map example to persist data: https://gist.github.com/lizrice/47ad44a15cce912502f8667a403f5649
* Free O'Reilly book available: "Learning eBPF" by Liz Rize (Isovalent): [https://isovalent.com/learning-ebpf/](https://isovalent.com/learning-ebpf/)
* More free books: [https://isovalent.com/resource-library/books/](https://isovalent.com/resource-library/books/)

## Alternative to BCC: bumblebee by solo.io

* Intro: [https://www.solo.io/blog/solo-announces-bumblebee/](https://www.solo.io/blog/solo-announces-bumblebee/)
* Example used in demo: sudo env "PATH=$PATH" bee run ghcr.io/solo-io/bumblebee/exitsnoop:$(bee version)

## Cilium

* Recap: Kubernetes Cluster architecture: https://kubernetes.io/docs/concepts/overview/components/
* Cilium start: [https://cilium.io](https://cilium.io)
* Free Tutorials (bottom right of page): [https://cilium.io/enterprise/#trainings](https://cilium.io/enterprise/#trainings)
* Installation steps used in my demo: [https://docs.cilium.io/en/stable/gettingstarted/k8s-install-default/](https://docs.cilium.io/en/stable/gettingstarted/k8s-install-default/)
* K8s example application used in demo: [https://istio.io/latest/docs/examples/bookinfo/](https://istio.io/latest/docs/examples/bookinfo/)
* Cilium multi-cloud use case: [https://youtu.be/6CZ_SSTqb4g?t=377](https://youtu.be/6CZ_SSTqb4g?t=377)
