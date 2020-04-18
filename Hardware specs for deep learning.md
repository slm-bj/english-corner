# Hardware Specs for Deep Learning Computer

Most important: GPU, CPU, memory, storage.

Supproted parts: motherboard, PSU, cooler, case.

## GPU

All Nvida Geforce Series.

Good cost/performance: RTX 2080ti: 16-bit models

Mainstream setup: GTX 1080ti: 32-bit models

### GPU selections (GDL)

* Best GPU overall (by a small margin): Titan Xp

* Cost efficient but expensive: GTX 1080 Ti, GTX 1070, GTX 1080

* Cost efficient and cheap: GTX 1060 (6GB)

* I work with data sets > 250GB: GTX Titan X (Maxwell), NVIDIA Titan X Pascal, or NVIDIA Titan Xp

* I have little money: GTX 1060 (6GB)

* I have almost no money: GTX 1050 Ti (4GB)

* I do Kaggle: GTX 1060 (6GB) for any normal competition, or GTX 1080 Ti for deep learning competitions

* I am a competitive computer vision researcher: NVIDIA Titan Xp; do not upgrade from existing Titan X (Pascal or Maxwell)

* I am a researcher: GTX 1080 Ti. In some cases, like natural language processing, a GTX 1070 or GTX 1080 might also be a solid choice �� check the memory requirements of your current models

* I want to build a GPU cluster: This is really complicated, you can get some ideas here

* I started deep learning and I am serious about it: Start with a GTX 1060 (6GB). Depending of what area you choose next (startup, Kaggle, research, applied deep learning) sell your GTX 1060 and buy something more appropriate

* I want to try deep learning, but I am not serious about it: GTX 1050 Ti (4 or 2GB)

### Memory requirements of GPU (FHG)

* Research that is hunting state-of-the-art scores: >=11 GB

* Research that is hunting for interesting architectures: >=8 GB

* Any other research: 8 GB

* Kaggle: 4 – 8 GB

* Startups: 8 GB (but check the specific application area for model sizes)

* Companies: 8 GB for prototyping, >=11 GB for training

## RAM

* Larger than GPU memeory (FHG).

* Clock rates do not matter — buy the cheapest RAM (FHG).

* More RAM can be useful if you frequently work with large datasets (FHG).

## CPU

2 cores per GPU, > 2GHz (FHG).

HRM:
> Keep in mind that the CPU must not bottleneck the GPU.
> For instance, an i7-7500U will work flawlessly with a GTX 1080 GPU.



### PCI-e lanes

PCI-e lane denotes the maximum bandwidth that is available for graphics cards communication with the CPU.

* PCIe lanes do not matter (FHG).
  Do not waste your money on PCIe lanes if you are using a single GPU (FHG).

* GPU:PCI-e lanes: 1:16 (CCP), at least 1:8 (HBP).

## Hard drive

* SSD for calculation, >= 128GB

* HDD for storage, >= 2TB, 7200 RPM

## PSU

Power supply unit

* Add up watts of GPUs + CPU. Then multiply the total by 110% for required Wattage.
* Get a high efficiency rating if you use a multiple GPUs.
* Make sure the PSU has enough PCIe connectors (6+8pins)

## Cooling system

For 1 GPU air cooling is best (FHG).

## Motherboard

## Computer Case

## Other devices

Monitor setup for a data scientist by Tim Dettmers:

![Monitor Setup](https://i2.wp.com/timdettmers.com/wp-content/uploads/2015/03/2015-03-04-13-58-10.jpg)

> Typical monitor layout when I do deep learning:
>
> * Left: Papers, Google searches, gmail, stackoverflow;
> * Middle: Code;
> * Right: Output windows, R, folders, systems monitors, GPU monitors, to-do list, and other small applications.

## Reference Summarizations

### CCP

1. Dual GPU

1. PCI-e lane, GPU:PCI-e lanes: 1:16
   PCI-e lane denotes the maximum bandwidth that is available for graphics cards�� communication with the CPU.

1. Motherboard chipset, Z170/270/370

1. CPU, Intel preprocessor, 4 cores

1. RAM, >= 16GB, 32GB prefered, clock: 2400 MHz

1. Storage, SSD (for calculation): >= 128GB, HDD (for storage): >= 2TB, 7200 RPM

1. GPU: 1080ti prefered, 1060 6GB for beginners, 1070ti for serious beginners

1. PSU: EVGA G2 series

## References

* CCP: [Choosing Components for Personal Deep Learning Machine](https://medium.com/mlreview/choosing-components-for-personal-deep-learning-machine-56bae813e34a)

* HBP: [How to build the perfect Deep Learning Computer and save thousands of dollars](https://medium.com/the-mission/how-to-build-the-perfect-deep-learning-computer-and-save-thousands-of-dollars-9ec3b2eb4ce2)

* FHG: [A Full Hardware Guide to Deep Learning](https://timdettmers.com/2018/12/16/deep-learning-hardware-guide/)

* HRM: [Everything you Need to Know About Hardware Requirements for Machine Learning](https://www.einfochips.com/blog/everything-you-need-to-know-about-hardware-requirements-for-machine-learning/)

* GDL: [Which GPU(s) to Get for Deep Learning: My Experience and Advice for Using GPUs in Deep Learning](https://timdettmers.com/2019/04/03/which-gpu-for-deep-learning/)

* [Which hardware components (CPU, RAM, GC, etc.) are needed for a machine learning/deep learning home PC/computer to run fast?](https://www.quora.com/Which-hardware-components-CPU-RAM-GC-etc-are-needed-for-a-machine-learning-deep-learning-home-PC-computer-to-run-fast)

* DLR: [How to create your own deep learning rig: A complete hardware guide](https://hackernoon.com/how-to-create-your-own-deep-learning-rig-a-complete-hardware-guide-7cdc71e174aa)

* [Recommended Systems for Machine Learning / AI TensorFlow](https://www.pugetsystems.com/recommended/Recommended-Systems-for-Machine-Learning-AI-TensorFlow-174)