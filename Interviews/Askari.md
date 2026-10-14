## C++ fundamentals and performance
- 45 min: Pointers, references, `const`, RAII, smart pointers, move semantics, and object lifetimes.
- 75 min: Implement a detection-processing program using `std::vector`, structs, filtering, and sorting.
- 45 min: Practice producer–consumer queues, mutexes, and thread safety.
- 15 min: Profile or inspect allocations and unnecessary copies

Build: A C++ detection pipeline that takes timestamped bounding boxes, filters low-confidence detections, and reports processing time.

Resource: [LearnCpp](https://www.learncpp.com/)
## CUDA fundamentals and GPU profiling
- 45 min: Threads, blocks, grids, kernels, host/device memory, synchronization.
- 45 min: Understand CPU/GPU transfers, kernel-launch overhead, and memory bandwidth.
- 60 min: Run a GPU workload if CUDA is available; profile it or compare timings across batch sizes and input sizes.
- 30 min: Identify likely bottlenecks and explain what you'd investigate next.

Build: A small profiling report showing workload, measurement method, timings, and bottleneck hypotheses. If CUDA isn't available, use a CPU benchmark and study GPU profiling concepts separately.

Resource: [CUDA Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/)
## TensorRT and embedded inference
- 30 min: Review ONNX export and the inference deployment pipeline.
- 45 min: Study TensorRT engines, FP16, INT8 calibration, and precision trade-offs.
- 75 min: Export a pretrained detector to ONNX and benchmark it, or inspect an existing ONNX model if export dependencies are problematic.
- 30 min: Write down how you would build and benchmark a TensorRT engine on Jetson Orin.

Build: A model benchmark comparing at least two configurations, where feasible. Record model/input settings, warm-up, timing methodology, and accuracy implications. Do not treat desktop timings as Jetson results.

Resource: [TensorRT documentation](https://docs.nvidia.com/deeplearning/tensorrt/developer-guide/index.html)
## ROS 2 integration in C++
- 45 min: Nodes, publishers/subscribers, messages, executors, and QoS.
- 90 min: Implement or adapt a simple `rclcpp` node that subscribes to input messages and publishes processed output.
- 30 min: Review timestamps, `tf2`, queue depth, and callback execution.
- 15 min: Test what happens when processing falls behind the incoming data rate.

Build: A minimal ROS 2 C++ processing node. If your environment isn't set up, sketch the node interfaces and work through a small existing ROS 2 C++ example.

Resource: [ROS 2 documentation](https://docs.ros.org/en/jazzy/)
## Object tracking and state estimation
- 45 min: Tracking-by-detection, IoU matching, track lifecycle, and identity switches.
- 60 min: Implement a simple tracker using detections from recorded video.
- 45 min: Learn Kalman filter prediction/update, state vectors, and measurement uncertainty.
- 30 min: Evaluate track continuity and behavior when detections disappear.

Build: A video with persistent track IDs and a short evaluation of tracking failures. Use a standard benchmark or labeled data if readily available; don't claim rigorous accuracy without suitable ground truth.

Resource: [SORT paper](https://arxiv.org/abs/1602.00763)

| Priority | Topic                       |
| -------- | --------------------------- |
| 1        | CUDA / TensorRT             |
| 2        | C++                         |
| 3        | ROS 2 integration           |
| 4        | Tracking / state estimation |
| 5        | More basic computer vision  |
## C++

- [Learn Modern C++ — sequential, focused guide](https://learnmoderncpp.com/)
- [LearnCpp — comprehensive tutorial](https://www.learncpp.com/)
- [C++ Core Guidelines — best practices](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines)
- [Compiler Explorer — run C++ in your browser](https://godbolt.org/)

## CUDA
- [NVIDIA CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-programming-guide/02-basics/intro-to-cuda-cpp.html)
- [CUDA Samples](https://github.com/NVIDIA/cuda-samples)
## ROS 2
- [ROS 2 Jazzy tutorials](https://docs.ros.org/en/jazzy/Tutorials.html)
- [C++ publisher/subscriber tutorial](https://docs.ros.org/en/jazzy/Tutorials/Beginner-Client-Libraries/Writing-A-Simple-Cpp-Publisher-And-Subscriber.html)
- [ROS 2 QoS](https://docs.ros.org/en/jazzy/Concepts/Intermediate/About-Quality-of-Service-Settings.html)
## ONNX
- [PyTorch ONNX export tutorial](https://docs.pytorch.org/tutorials/beginner/onnx/export_simple_model_to_onnx_tutorial.html)
- [ONNX tutorials](https://onnx.ai/onnx/intro/python.html)
- [Netron model viewer](https://netron.app/)

## TensorRT

- [Build Your First TensorRT Engine](https://docs.nvidia.com/deeplearning/tensorrt/latest/getting-started/build-your-first-engine.html)
- [TensorRT Quick Start Guide](https://docs.nvidia.com/deeplearning/tensorrt/latest/getting-started/quick-start-guide.html)
## Python

- [Official Python tutorial](https://docs.python.org/3/tutorial/)
- [NumPy quickstart](https://numpy.org/doc/stable/user/quickstart.html)
## PyTorch
- [PyTorch 60-Minute Blitz](https://docs.pytorch.org/tutorials/beginner/blitz/)
- [Torchvision object detection tutorial](https://docs.pytorch.org/tutorials/intermediate/torchvision_tutorial.html)