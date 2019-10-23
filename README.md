## Open-DLA-Performance-Profiler

Performance profiling for neural network, deep learning and machine learning models on different openDLA architectures

The **openDLA** is based on [NVDLA](http://nvdla.org/index.html).

This tool is developed based on [**netron**](https://github.com/lutzroeder/netron).

### Key Words
- Summary Table :  
  - MAC Utilization: average MAC utilization under aggressive FPS
  - Roofline Factor: the ratio of memory access cycles / total cycles
  - Conservative FPS: consider the memory access and computation is fully overlapped 
  - Aggressive FPS: consider the memory access and computation is fully interleaved

- Traffic Table :
  - IFM	: input feature maps
  - OFM	: output feature maps
  - WM : weights

- Detail Table :
  - type	:  computation type
  - attributes	: 	fused layers
  - ch_in	: input channel number
  - dim_in	: 	input dimension
  - ch_out	: 	output channel number
  - kernel_w	: 	kernel width
  - kernel_h	: 	kernel height
  - pad_w	: padding size of width direction
  - pad_h	: padding size of height direction
  - stride_w	:  stride size of width direction
  - stride_h	:  stride size of height direction
  
  
---------------------------------

### Deferences between the free version here and commercial version

| Features | Free Version (here) | Commercial Version |
| ------   | -----------  | ------------------ |
| Layer Fuse Info  | o | o |
| Performance Table DRAM only          | o | o |
| Performance Table Hybrid memory (SRAM + DRAM)   | X | o |
| DRAM/SRAM Policy | X | o |
| DRAM/SRAM data footprint | X | o |
| Configurable Freq./MEM BW | X | o |
| Model Format | Caffe | ONNX, TensorFlow, Caffe...|
| Source Codes | X | o |
