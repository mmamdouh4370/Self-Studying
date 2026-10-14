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


****About Askari Defense****

Modern warfare is dictated by robotics. Autonomous drones and robotic ground systems are reshaping every battlefield on Earth.

Askari develops high-performance, fully-autonomous kinetic intercept systems that counter unmanned aerial and robotic threats in the world's most demanding operational environments. We build deployable systems for real-world constraints, urgent missions, and operators who cannot wait years for capability, and are continuously evolving our systems because the robotic threat evolves daily.

We are a tight team of top engineers and scientists from Skydio, Hermeus, Near Earth Autonomy, Area-I/Anduril, Raytheon, Sandia National Laboratories, and GTRI. We work directly with elite end-users, turning emerging battlefield requirements into rugged, scalable, mission-ready defenses.

Come build alongside elite engineers on a generational mission to defend the Western world. We hold ourselves to an exceptionally high bar: the work is demanding, the pace is intense, and the mission requires people willing to go all in. For the right person, it will be more rewarding than any previous job. Askari is a place for builders serious about mastery, ownership, exponential growth, and delivering capability when it matters most.

As warfare becomes increasingly robotic, distributed, and fast-moving, the defense industrial base needs a new model: Askari is defining that model.

If protecting humanity from the coming age of robotic warfare is the mission you have been waiting for, this is where you do it.

****About the role****

This role is designed for a ****perception engineer**** who can build, evaluate, and deploy the sensing and embedded vision systems that allow our autonomous intercept platforms to detect, track, and act on fast-moving aerial threats.

You will work across the full perception stack, from ****camera and lens selection**** through image formation, signal processing, embedded deployment, model evaluation, and integration with the autonomy system. Machine learning is part of the job, but not the whole job. We are looking for someone who understands that perception performance starts before the model: with the sensor, optics, scene, exposure, motion, latency, compute, and data pipeline.

You will support camera and lens trade studies, evaluate sensor characteristics against mission requirements, develop image- and signal-processing techniques that improve detection of small, low-contrast objects, and help translate range data into better embedded perception performance. This is not a research-only role. Your work will run onboard real vehicles, integrate with the autonomy stack, and be tested against demanding field data.

We are looking for ****evidence-driven engineers:**** individuals who ****prioritize physical reality over opinion****, care about end-to-end system performance, and can debug problems across the full chain from photons hitting the sensor to detections reaching the autonomy system.

This is a strong fit for someone who wants to build perception systems that leave the laptop, run on embedded compute, and directly determine whether an autonomous system succeeds in the real world.

****What you'll do****

You will develop and deploy the optical sensing, image-processing, and embedded perception capabilities that enable our autonomous systems to detect, classify, track, and reason about fast-moving aerial targets in real time.

You will focus on problems in all of the following areas:

- ****Optical Sensor & Lens Trade Studies:**** Support camera and lens trade studies, evaluating sensor characteristics such as pixel size, sensitivity, noise, dynamic range, resolution, and optical performance against application requirements.
- ****Image & Signal Processing:**** Develop and evaluate image- and signal-processing techniques, including denoising, filtering, temporal extraction, and contrast enhancement, to improve detection of small, low-contrast objects.
- ****Aerial-Object Data Collection:**** Design and execute data-collection experiments for aerial-object detection and tracking, then use field data to improve the next system iteration.
- ****Embedded Vision Deployment:**** Deploy, benchmark, and maintain perception software on embedded edge compute aboard autonomous vehicles.
- ****Real-Time Performance:**** Optimize perception pipelines for latency, throughput, and reliability on NVIDIA Jetson Orin-class hardware using tools such as ****CUDA**** and ****TensorRT**** where appropriate.
- ****Computer Vision & ML Models:**** Design, train, fine-tune, and evaluate vision models for detection, classification, tracking, and state estimation on fast-moving aerial targets.
- ****Autonomy Stack Integration:**** Integrate perception outputs into our autonomy stack using ****ROS 2**** and write production-quality ****C++**** for real-time processing.
- ****End-to-End Debugging:**** Debug problems across the entire stack, from photons hitting the sensor to detections reaching the autonomy system.
- ****Performance Characterization:**** Analyze perception performance across flight data, edge cases, false positives, false negatives, latency, lighting, motion blur, vibration, target size, and engagement conditions.
- ****Cross-Functional Development:**** Work closely with autonomy, GNC, state estimation, flight test, electrical, and data teams to ensure perception outputs are useful, timely, and aligned with the needs of the full system.
- ****Dataset Improvement:**** Help identify data gaps, improve labeling workflows, and guide future data collection so perception development reflects the environments and target behaviors that matter most.

****Basic Qualifications****

- ****Education:**** BS in Computer Science, Robotics, Electrical Engineering, Computer Engineering, Aerospace Engineering, or a related field plus 1+ years of industry or applied robotics experience, or an MS in a related discipline.
- ****Perception or Computer Vision:**** Experience developing perception, computer vision, image-processing, or sensor-processing systems for real-world applications.
- ****Software Skills:**** Proficiency in ****C++**** for performance-sensitive systems.
- ****Image Processing:**** Familiarity with image-processing fundamentals such as filtering, denoising, contrast enhancement, feature extraction, or temporal analysis.
- ****Embedded or Real-Time Systems:**** Experience building, profiling, or deploying software where latency, compute, or hardware constraints matter.
- ****Computer Vision Models:**** Experience training, fine-tuning, or evaluating vision models, including CNNs, Vision Transformers, detection, tracking, or related approaches.
- ****Execution Tempo:**** Ability to work in a fast-paced engineering environment where field data, hardware constraints, and measured system performance drive rapid iteration.

  

****Preferred Qualifications****

Experience in any of the following areas is a plus:

- ****Camera & Lens Evaluation:**** Experience evaluating cameras, lenses, image sensors, or optical systems against application requirements.
- ****Sensor Characteristics:**** Familiarity with sensor characteristics such as pixel size, sensitivity, noise, dynamic range, resolution, exposure, and optical performance.
- ****Embedded Edge Deployment:**** Experience deploying perception software or models on embedded edge platforms, including ****Jetson Orin**** or Xavier.
- ****GPU Optimization:**** Hands-on GPU programming or profiling experience, including ****CUDA****, TensorRT, or related tools.
- ****ROS 2:**** Experience with ROS 2 nodes, lifecycle management, QoS, custom interfaces, or related robotics middleware.
- ****Sensor Fusion:**** Experience with sensor fusion, including visual-inertial odometry, camera + radar, camera + LiDAR, or related multimodal perception systems.
- ****Field Robotics or UAS Testing:**** Prior field-robotics or UAS test experience.
- ****Dataset & Evaluation Workflows:**** Experience building or using datasets, labeling workflows, evaluation metrics, and model regression tools for perception systems.
- ****Production CV Systems:**** Experience taking perception algorithms or models beyond notebooks into deployed, maintainable software systems.

https://www.hypepotamus.com/askari-defense-launches-in-atlanta/
https://www.techsquareatl.com/tech-square-news/2026/4/7/now-out-of-stealth-askari-is-building-smarter-decentralized-defense-systems
https://www.dhs.gov/science-and-technology/news/2025/12/02/feature-article-taking-nefarious-drones-out-fight
https://create-x.gatech.edu/2025-demo-day
https://askaridefense.com/press/lore