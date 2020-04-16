A: Hi [Bob], what are you doing?

B: Hi [Alice]. I am building a virtual machine on my laptop.

A: What are the specs of your laptop?

B: 4 cores Intel i5 CPU, 8 GB memories, 128 GB SSD.

A: Is it enough for running virtual machines?
   I've heard it's very resource-consuming for running VMs.

B: You got the point. The VMs are really heavy in regard of Virtualbox or VMware.
   However, the VMs on my laptop are Linux containers, which are much lighter than 
   that in Virtualbox.

A: Why Linux containers can achieve this?

B: Have you ever heard Docker?

A: Yes, it's the superstar in tech world these days. Everybody knows it.

B: It's based on Linux container technics.

A: Wow, why not explain to me the magic of the containers?

B: Well, the hardwares of Virtualbox style VM are virtualized by software,
   while that of Containers are real metal.
   The VMs are just "isolated" instead of "created".

A: What does "created" mean?

B: For example you created a VM in Virtualbox with a 2-cores CPU.
   There isn't a real metal CPU in you Virtualbox.
   But the softwares in your VM have no sense about whether the world is physical or virtualized.
   They give instructions as what they do in real world.
   But the CPU of the VM is actually made up of some bits.

A: Like people in the Matrix?

B: Absolutely. You have no way to find out whether the world is real or virtualized.

A: That's horrible. What about containers?

B: Containers and their host share the same kernel space, while living in isolated file systems.
   So the CPU and memory of the containers are the same ones of the host's.

A: Do the softwares in the containers know they are living in a fake world?

B: No. To them, everything is as real as that in real world.

A: Is it possible that we are living in a VM or container now?

B: Did you see the movie "The Truman Show"?

A: Yes. Trueman finally found out the secrets of the show, and left bravely.

B: That's a happy ending. But for people lived in VM or containers, I'm afraid it would be much harder to find out the truth.
