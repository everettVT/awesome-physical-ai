# awesome-physical-ai

A curated list of open source projects for Physical AI — robotics, embodied intelligence, simulation, and the infrastructure that makes it work.

Curated from the stuff I actually use, star, and interest me. PRs welcome.

**Legend:** ★ = in [my stars](https://github.com/everettVT?tab=stars) · unmarked = well-known projects on my to-star list

---

## Contents

- [Foundation models & policies](#foundation-models--policies)
- [Simulation & environments](#simulation--environments)
- [World models](#world-models)
- [Training & RL infrastructure](#training--rl-infrastructure)
- [Robot operating systems & middleware](#robot-operating-systems--middleware)
- [Perception & sensing](#perception--sensing)
- [GPU & compute primitives](#gpu--compute-primitives)
- [Data & datasets](#data--datasets)
- [Evaluation & benchmarks](#evaluation--benchmarks)
- [Orchestration & deployment](#orchestration--deployment)
- [Papers & meta-lists](#papers--meta-lists)

---

## Foundation models & policies

VLA models, behavior cloning, action models, robot foundation models.

- ★ [Physical-Intelligence/openpi](https://github.com/Physical-Intelligence/openpi) — π₀ and π₀.₅ open vision-language-action models and fine-tuning code from Physical Intelligence.
- ★ [openvla/openvla](https://github.com/openvla/openvla) — The open-source VLA baseline for robotic manipulation; the reference point most VLA papers compare against.
- ★ [starVLA/starVLA](https://github.com/starVLA/starVLA) — Lego-like codebase for composing and developing VLA models.
- ★ [ginwind/VLA-JEPA](https://github.com/ginwind/VLA-JEPA) — Enhancing VLA models with a latent world model (ECCV 2026).
- ★ [NVlabs/GR00T-WholeBodyControl](https://github.com/NVlabs/GR00T-WholeBodyControl) — Unified platform for developing and deploying humanoid whole-body control.
- ★ [ShuangLI59/unified_video_action](https://github.com/ShuangLI59/unified_video_action) — Unified Video Action Model (RSS 2025): one model for video prediction and action generation.
- ★ [x-robotics-lab/minbc](https://github.com/x-robotics-lab/minbc) — Minimal behavior cloning; the nanoGPT of imitation learning.
- ★ [MineDojo/NitroGen](https://github.com/MineDojo/NitroGen) — Foundation model for generalist gaming agents; embodied action models beyond robot arms.
- [huggingface/lerobot](https://github.com/huggingface/lerobot) — End-to-end robot learning: datasets, policies (ACT, diffusion, SmolVLA), and real-hardware drivers.
- [NVIDIA/Isaac-GR00T](https://github.com/NVIDIA/Isaac-GR00T) — GR00T N1.x, NVIDIA's foundation model for generalist humanoid robots.
- [octo-models/octo](https://github.com/octo-models/octo) — Transformer robot policy pretrained on 800k trajectories from Open X-Embodiment.
- [real-stanford/diffusion_policy](https://github.com/real-stanford/diffusion_policy) — Visuomotor policy learning via action diffusion; spawned an entire policy-class.
- [tonyzhaozh/act](https://github.com/tonyzhaozh/act) — Action Chunking with Transformers, the policy behind ALOHA bimanual teleop.
- [thu-ml/RoboticsDiffusionTransformer](https://github.com/thu-ml/RoboticsDiffusionTransformer) — RDT-1B: diffusion foundation model for bimanual manipulation.
- [moojink/openvla-oft](https://github.com/moojink/openvla-oft) — Optimized fine-tuning recipe for VLAs; big speed and success-rate gains over vanilla OpenVLA.

## Simulation & environments

Physics engines, robot sim benchmarks, multi-agent environments, digital twins.

- ★ [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco) — The physics engine of record for robot learning; MJX brings it to GPU/TPU.
- ★ [mani-skill/ManiSkill](https://github.com/mani-skill/ManiSkill) — GPU-parallelized manipulation simulator and benchmark built on SAPIEN.
- ★ [Genesis-Embodied-AI/genesis-world](https://github.com/Genesis-Embodied-AI/genesis-world) — Generative, differentiable simulation platform for general-purpose robotics.
- ★ [google-deepmind/dm_control](https://github.com/google-deepmind/dm_control) — DeepMind's MuJoCo-based stack for physics-based RL environments.
- ★ [Unity-Technologies/ml-agents](https://github.com/Unity-Technologies/ml-agents) — Turn any Unity scene into a training environment.
- ★ [Farama-Foundation/PettingZoo](https://github.com/Farama-Foundation/PettingZoo) — The standard API for multi-agent RL environments.
- ★ [google-deepmind/meltingpot](https://github.com/google-deepmind/meltingpot) — Test suite for multi-agent RL social scenarios.
- ★ [google-deepmind/lab2d](https://github.com/google-deepmind/lab2d) — Customizable 2D platform for agent-based research.
- ★ [openai/gym](https://github.com/openai/gym) — The original RL environment API (maintained successor below).
- ★ [NVIDIA-Omniverse/kit-app-template](https://github.com/NVIDIA-Omniverse/kit-app-template) — Build Omniverse digital-twin apps from a template.
- ★ [MineDojo/Voyager](https://github.com/MineDojo/Voyager) — Open-ended embodied agent with LLMs in Minecraft; the canary for lifelong embodied learning.
- [isaac-sim/IsaacLab](https://github.com/isaac-sim/IsaacLab) — Unified robot-learning framework on Isaac Sim; where most humanoid RL happens today.
- [NVIDIA/warp](https://github.com/NVIDIA/warp) — Python framework for GPU-accelerated simulation and differentiable physics kernels.
- [google-deepmind/mujoco_playground](https://github.com/google-deepmind/mujoco_playground) — GPU-accelerated robot learning and sim-to-real on MJX.
- [google-deepmind/mujoco_menagerie](https://github.com/google-deepmind/mujoco_menagerie) — High-quality MuJoCo models of real robots, curated by DeepMind.
- [facebookresearch/habitat-sim](https://github.com/facebookresearch/habitat-sim) — High-performance 3D simulator for embodied AI navigation and rearrangement.
- [ARISE-Initiative/robosuite](https://github.com/ARISE-Initiative/robosuite) — Modular MuJoCo simulation framework and benchmark for robot learning.
- [robocasa/robocasa](https://github.com/robocasa/robocasa) — Large-scale simulation of everyday household tasks for generalist robots.
- [haosulab/SAPIEN](https://github.com/haosulab/SAPIEN) — Embodied AI platform with part-level interactive objects (PartNet-Mobility).
- [google/brax](https://github.com/google/brax) — Massively parallel rigid-body physics in JAX.
- [bulletphysics/bullet3](https://github.com/bulletphysics/bullet3) — Bullet/PyBullet: the workhorse physics SDK before GPU sim ate the world.
- [RobotLocomotion/drake](https://github.com/RobotLocomotion/drake) — Model-based design and verification for robotics from Toyota Research Institute.
- [Farama-Foundation/Gymnasium](https://github.com/Farama-Foundation/Gymnasium) — The maintained standard API for single-agent RL environments.
- [kevinzakka/mink](https://github.com/kevinzakka/mink) — Differential inverse kinematics in MuJoCo.

## World models

Video prediction, latent imagination, environment modeling.

- ★ [NVIDIA/cosmos](https://github.com/NVIDIA/cosmos) — NVIDIA's open platform of world foundation models, datasets, and tooling for Physical AI.
- ★ [NVIDIA/Cosmos-Tokenizer](https://github.com/NVIDIA/Cosmos-Tokenizer) — Image and video neural tokenizers that feed world-model training.
- ★ [lucas-maes/le-wm](https://github.com/lucas-maes/le-wm) — LeWorldModel: stable end-to-end JEPA world models from pixels.
- [danijar/dreamerv3](https://github.com/danijar/dreamerv3) — Mastering diverse domains through latent imagination; the reference world-model agent.
- [facebookresearch/vjepa2](https://github.com/facebookresearch/vjepa2) — V-JEPA 2: self-supervised video world models, Meta's bet on predictive latents over pixels.
- [eloialonso/diamond](https://github.com/eloialonso/diamond) — DIAMOND: RL agents trained inside a diffusion world model.
- [1x-technologies/1xgpt](https://github.com/1x-technologies/1xgpt) — 1X's world-modeling challenge for humanoid robots, with real robot video data.

## Training & RL infrastructure

RL frameworks, GRPO, reward modeling, distributed training.

- ★ [verl-project/verl](https://github.com/verl-project/verl) — HybridFlow: the flexible, high-throughput RL post-training framework everyone forks.
- ★ [PrimeIntellect-ai/prime-rl](https://github.com/PrimeIntellect-ai/prime-rl) — Agentic RL training at scale, built for decentralized compute.
- ★ [PrimeIntellect-ai/verifiers](https://github.com/PrimeIntellect-ai/verifiers) — Library of RL environments and verifiable rewards.
- ★ [NousResearch/atropos](https://github.com/NousResearch/atropos) — LLM RL environments framework for collecting and evaluating trajectories.
- ★ [OpenPipe/ART](https://github.com/OpenPipe/ART) — Agent Reinforcement Trainer: GRPO for multi-step agents on real tasks.
- ★ [NVlabs/GDPO](https://github.com/NVlabs/GDPO) — Group reward-decoupled normalization for multi-reward RL.
- ★ [policy-gradient/GRPO-Zero](https://github.com/policy-gradient/GRPO-Zero) — DeepSeek R1's GRPO implemented from scratch; best way to actually understand it.
- ★ [huggingface/trl](https://github.com/huggingface/trl) — Train transformers with RL: SFT, DPO, GRPO, reward modeling.
- ★ [huggingface/open-r1](https://github.com/huggingface/open-r1) — Fully open reproduction of DeepSeek-R1.
- ★ [allenai/open-instruct](https://github.com/allenai/open-instruct) — AI2's post-training codebase (Tülu recipes).
- ★ [sii-research/siiRL](https://github.com/sii-research/siiRL) — RL framework for advanced LLMs and multi-agent systems.
- ★ [Zhiyuan-Zeng/RLVE](https://github.com/Zhiyuan-Zeng/RLVE) — Scaling RL with adaptively verifiable environments (ICML 2026).
- ★ [ypwang61/One-Shot-RLVR](https://github.com/ypwang61/One-Shot-RLVR) — RL for reasoning with one training example (NeurIPS 2025).
- ★ [NVlabs/ToolOrchestra](https://github.com/NVlabs/ToolOrchestra) — End-to-end RL for orchestrating tools and agentic workflows.
- ★ [NVIDIA/Megatron-LM](https://github.com/NVIDIA/Megatron-LM) — The reference for training transformers at scale.
- ★ [ray-project/ray](https://github.com/ray-project/ray) — Distributed compute substrate under half the RL frameworks on this list.
- [OpenRLHF/OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) — Easy-to-use, scalable agentic RL framework on Ray (PPO, DAPO, REINFORCE++).
- [NovaSky-AI/SkyRL](https://github.com/NovaSky-AI/SkyRL) — Modular full-stack RL library for LLMs from Berkeley Sky Computing.
- [leggedrobotics/rsl_rl](https://github.com/leggedrobotics/rsl_rl) — Fast, simple RL for robotics; the PPO behind most legged-locomotion results.
- [unitreerobotics/unitree_rl_gym](https://github.com/unitreerobotics/unitree_rl_gym) — RL environments and sim-to-real pipelines for Unitree robots.
- [ARISE-Initiative/robomimic](https://github.com/ARISE-Initiative/robomimic) — Modular framework for robot learning from demonstration.
- [DLR-RM/stable-baselines3](https://github.com/DLR-RM/stable-baselines3) — Reliable PyTorch implementations of classic deep RL algorithms.
- [vwxyzjn/cleanrl](https://github.com/vwxyzjn/cleanrl) — Single-file deep RL implementations for research clarity.
- [pytorch/rl](https://github.com/pytorch/rl) — TorchRL: modular, primitive-first RL library for PyTorch.

## Robot operating systems & middleware

Real-time control, ROS alternatives, hardware abstraction.

- ★ [copper-project/copper-rs](https://github.com/copper-project/copper-rs) — Deterministic robot OS in Rust: build, run, and replay your entire robot.
- ★ [elodin-sys/elodin](https://github.com/elodin-sys/elodin) — Simulation and flight software monorepo for drones and space systems, ECS-based, in Rust.
- ★ [mcarfagno/mpc_python](https://github.com/mcarfagno/mpc_python) — Simple MPC controller for path tracking; a readable intro to receding-horizon control.
- ★ [IntelligentControlSystems/l4acados](https://github.com/IntelligentControlSystems/l4acados) — Learning-based models inside acados real-time MPC.
- ★ [bevyengine/bevy](https://github.com/bevyengine/bevy) — Data-driven ECS engine in Rust; increasingly the substrate for robotics tooling and viz.
- ★ [skypjack/entt](https://github.com/skypjack/entt) — The C++ entity-component-system powering real-time architectures (and Minecraft).
- ★ [meshtastic/firmware](https://github.com/meshtastic/firmware) — Open LoRa mesh networking for off-grid device comms.
- [ros2/ros2](https://github.com/ros2/ros2) — The Robot Operating System; still the lingua franca of robot software.
- [dora-rs/dora](https://github.com/dora-rs/dora) — Dataflow-oriented robotic architecture in Rust; the ROS alternative the LeRobot crowd uses.
- [eclipse-zenoh/zenoh](https://github.com/eclipse-zenoh/zenoh) — Pub/sub + storage + compute protocol unifying robot-to-cloud data in motion.
- [PX4/PX4-Autopilot](https://github.com/PX4/PX4-Autopilot) — The open flight-control stack for drones and VTOL.
- [ArduPilot/ardupilot](https://github.com/ArduPilot/ardupilot) — Autopilot for planes, copters, rovers, subs; two decades of field hours.
- [NVlabs/curobo](https://github.com/NVlabs/curobo) — CUDA-accelerated motion planning and IK.
- [NVIDIA-ISAAC-ROS/isaac_ros_common](https://github.com/NVIDIA-ISAAC-ROS/isaac_ros_common) — GPU-accelerated ROS 2 packages for NVIDIA Jetson and beyond.
- [rerun-io/rerun](https://github.com/rerun-io/rerun) — Visualize, query, and stream multimodal robotics data; the log-everything debugger for embodied AI.
- [foxglove/mcap](https://github.com/foxglove/mcap) — Serialization-agnostic container format for robotics logs.
- [TheRobotStudio/SO-ARM100](https://github.com/TheRobotStudio/SO-ARM100) — The open-hardware arm that made robot learning a $200 hobby (LeRobot's default platform).

## Perception & sensing

Depth estimation, segmentation, motion capture, pose estimation.

- ★ [facebookresearch/segment-anything](https://github.com/facebookresearch/segment-anything) — SAM: promptable segmentation for anything.
- ★ [facebookresearch/sam2](https://github.com/facebookresearch/sam2) — SAM 2: segmentation extended to video.
- ★ [facebookresearch/sam3](https://github.com/facebookresearch/sam3) — SAM 3: concept-prompted detection, segmentation, and tracking.
- ★ [apple/ml-depth-pro](https://github.com/apple/ml-depth-pro) — Sharp monocular metric depth in under a second.
- ★ [cuevhv/mamma](https://github.com/cuevhv/mamma) — MAMMA: markerless accurate multi-person motion capture (CVPR 2026).
- ★ [nv-tlabs/vipe](https://github.com/nv-tlabs/vipe) — ViPE: video pose engine for geometric 3D perception (camera pose, depth, SLAM).
- ★ [google-deepmind/videoprism](https://github.com/google-deepmind/videoprism) — Foundational visual encoder for video understanding.
- ★ [facebookresearch/detectron2](https://github.com/facebookresearch/detectron2) — The detection and segmentation platform much of robot perception is prototyped on.
- ★ [google-ai-edge/mediapipe](https://github.com/google-ai-edge/mediapipe) — Cross-platform, on-device ML for live and streaming media (hands, pose, face).
- ★ [xinyu1205/recognize-anything](https://github.com/xinyu1205/recognize-anything) — Strong open-set image tagging and recognition models.
- ★ [apple/ml-4m](https://github.com/apple/ml-4m) — Massively multimodal masked modeling across vision modalities.
- [NVlabs/FoundationPose](https://github.com/NVlabs/FoundationPose) — Unified 6D pose estimation and tracking of novel objects (CVPR 2024 highlight).
- [DepthAnything/Depth-Anything-V2](https://github.com/DepthAnything/Depth-Anything-V2) — Foundation model for monocular depth estimation.
- [IDEA-Research/GroundingDINO](https://github.com/IDEA-Research/GroundingDINO) — Open-set object detection from language prompts; SAM's usual partner.
- [facebookresearch/co-tracker](https://github.com/facebookresearch/co-tracker) — Track any pixel through a video.
- [naver/mast3r](https://github.com/naver/mast3r) — Image matching grounded in 3D; DUSt3R lineage for metric reconstruction.

## GPU & compute primitives

Kernel programming, CUDA tooling, inference engines, quantization.

- ★ [NVIDIA/cutile-python](https://github.com/NVIDIA/cutile-python) — cuTile: tile-based parallel kernel programming model for NVIDIA GPUs.
- ★ [NVlabs/cutile-rs](https://github.com/NVlabs/cutile-rs) — Safe, tile-based kernel DSL for Rust.
- ★ [NVIDIA/TileGym](https://github.com/NVIDIA/TileGym) — Kernel tutorials, examples, and agent SKILLs for tile-based GPU programming.
- ★ [NVlabs/cuda-oxide](https://github.com/NVlabs/cuda-oxide) — Experimental Rust-to-CUDA compiler: SIMT kernels in safe(ish) idiomatic Rust.
- ★ [uccl-project/mKernel](https://github.com/uccl-project/mKernel) — Fast multi-node, multi-GPU fused kernels.
- ★ [RyanCodrai/turbovec](https://github.com/RyanCodrai/turbovec) — TurboQuant-based vector index in Rust; quantized similarity search at SIMD speed.
- ★ [vllm-project/vllm](https://github.com/vllm-project/vllm) — The default high-throughput LLM inference engine.
- ★ [vllm-project/vllm-omni](https://github.com/vllm-project/vllm-omni) — Efficient inference for omni-modality models: video, audio, world models.
- ★ [vllm-project/llm-compressor](https://github.com/vllm-project/llm-compressor) — Quantization and compression pipeline feeding vLLM deployment.
- ★ [sgl-project/sglang](https://github.com/sgl-project/sglang) — High-performance serving for LLMs and VLMs; strong on structured output.
- ★ [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) — Inference at the edge: CPU/GPU/NPU, the format the whole local-AI world ships in.
- ★ [triton-inference-server/server](https://github.com/triton-inference-server/server) — Optimized cloud and edge inference serving from NVIDIA.
- ★ [GeeeekExplorer/nano-vllm](https://github.com/GeeeekExplorer/nano-vllm) — vLLM distilled to its readable essence.
- ★ [meta-pytorch/BackendBench](https://github.com/meta-pytorch/BackendBench) — Ship correct and fast kernels to PyTorch.
- ★ [NVIDIA/AMGX](https://github.com/NVIDIA/AMGX) — Distributed multigrid linear solvers on GPU; the numerics under implicit physics.
- ★ [Blaizzy/mlx-vlm](https://github.com/Blaizzy/mlx-vlm) — VLM inference and fine-tuning on Apple Silicon via MLX.
- ★ [gpu-mode/lectures](https://github.com/gpu-mode/lectures) — The GPU MODE lecture series; the on-ramp for kernel engineering.
- [triton-lang/triton](https://github.com/triton-lang/triton) — The tile-level language and compiler most custom kernels are written in.
- [NVIDIA/cutlass](https://github.com/NVIDIA/cutlass) — CUDA templates and Python DSLs for high-performance linear algebra.
- [NVIDIA/TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) — NVIDIA's optimized LLM inference stack for datacenter GPUs.

## Data & datasets

Robot datasets, synthetic data, data processing for Physical AI.

- ★ [Eventual-Inc/Daft](https://github.com/Eventual-Inc/Daft) — High-performance data engine for multimodal AI: images, video, audio, embeddings, and structured data at any scale. (Disclosure: I work on this.)
- ★ [droid-dataset/droid](https://github.com/droid-dataset/droid) — DROID: large-scale distributed robot interaction dataset.
- ★ [mlfoundations/dclm](https://github.com/mlfoundations/dclm) — DataComp for Language Models; the data-curation benchmark playbook.
- ★ [macrodata-labs/refiner](https://github.com/macrodata-labs/refiner) — Data processing framework for large-scale ML datasets.
- ★ [Eventual-Inc/marlin](https://github.com/Eventual-Inc/marlin) — Highly efficient video dataloader in Rust.
- ★ [lancedb/lancedb](https://github.com/lancedb/lancedb) — Embedded multimodal retrieval; Lance format for versioned tensor/vector data.
- ★ [ray-project/deltacat](https://github.com/ray-project/deltacat) — Portable multimodal lakehouse on Ray with ACID and CDC.
- ★ [deepseek-ai/smallpond](https://github.com/deepseek-ai/smallpond) — Lightweight data processing on DuckDB and 3FS.
- ★ [rapidsai/cudf](https://github.com/rapidsai/cudf) — GPU DataFrames; preprocessing at the speed of the accelerator.
- ★ [mostly-ai/mostlyai](https://github.com/mostly-ai/mostlyai) — Synthetic data SDK with differential privacy.
- ★ [zarrs/zarrs](https://github.com/zarrs/zarrs) — Rust implementation of Zarr for chunked multidimensional sensor arrays.
- [google-deepmind/open_x_embodiment](https://github.com/google-deepmind/open_x_embodiment) — Open X-Embodiment: the cross-robot dataset behind RT-X and most VLA pretraining mixes.
- [OpenDriveLab/AgiBot-World](https://github.com/OpenDriveLab/AgiBot-World) — Large-scale manipulation platform and dataset (IROS 2025 best-paper finalist).
- [facebookresearch/Ego4d](https://github.com/facebookresearch/Ego4d) — Massive egocentric video dataset; human demonstrations at world scale.
- [google-research/rlds](https://github.com/google-research/rlds) — Reinforcement Learning Datasets: the episodic data format under Open X-Embodiment.
- [voxel51/fiftyone](https://github.com/voxel51/fiftyone) — Curate and debug visual datasets and models.

## Evaluation & benchmarks

VLA evaluation, sim-to-real, terminal and agent benchmarks.

- ★ [allenai/vla-evaluation-harness](https://github.com/allenai/vla-evaluation-harness) — One framework to evaluate any VLA on any robot sim benchmark.
- ★ [simpler-env/SimplerEnv](https://github.com/simpler-env/SimplerEnv) — Real-to-sim evaluation of real-robot manipulation policies (RT-1, Octo, ...).
- ★ [PKU-Alignment/VLA-Arena](https://github.com/PKU-Alignment/VLA-Arena) — Open benchmark for systematic VLA evaluation.
- ★ [Lifelong-Robot-Learning/LIBERO](https://github.com/Lifelong-Robot-Learning/LIBERO) — Benchmarking knowledge transfer in lifelong robot learning; the default VLA eval suite.
- ★ [NVIDIA/cosmos-evaluator](https://github.com/NVIDIA/cosmos-evaluator) — Automated grading for synthetic video from world models.
- ★ [sierra-research/tau2-bench](https://github.com/sierra-research/tau2-bench) — τ²-bench: tool-agent-user interaction in real-world domains.
- ★ [harbor-framework/terminal-bench](https://github.com/harbor-framework/terminal-bench) — Benchmark for agents on complicated terminal tasks.
- ★ [stanford-iris-lab/meta-harness-tbench2-artifact](https://github.com/stanford-iris-lab/meta-harness-tbench2-artifact) — Meta-Harness: what a tuned harness adds on Terminal-Bench 2.0.
- ★ [eval-protocol/python-sdk](https://github.com/eval-protocol/python-sdk) — SDK for the Eval Protocol spec.
- [Farama-Foundation/Metaworld](https://github.com/Farama-Foundation/Metaworld) — Multi-task and meta-RL manipulation benchmark.
- [stepjam/RLBench](https://github.com/stepjam/RLBench) — Large-scale robot learning benchmark (100+ tasks).
- [mees/calvin](https://github.com/mees/calvin) — Language-conditioned long-horizon manipulation benchmark.
- [StanfordVL/BEHAVIOR-1K](https://github.com/StanfordVL/BEHAVIOR-1K) — 1,000 everyday household activities as an embodied AI benchmark.

## Orchestration & deployment

Fleet management, cloud-to-edge, Physical AI platforms.

- ★ [NVIDIA/OSMO](https://github.com/NVIDIA/OSMO) — Developer-first platform for scaling Physical AI workloads across heterogeneous compute.
- ★ [ai-dynamo/dynamo](https://github.com/ai-dynamo/dynamo) — Datacenter-scale distributed inference serving (disaggregated prefill/decode).
- ★ [skypilot-org/skypilot](https://github.com/skypilot-org/skypilot) — Run AI workloads on any infra: k8s, 16+ clouds, on-prem.
- ★ [NVIDIA-NeMo/Run](https://github.com/NVIDIA-NeMo/Run) — Configure, launch, and manage ML experiments across environments.
- ★ [vllm-project/production-stack](https://github.com/vllm-project/production-stack) — K8s-native cluster-wide vLLM deployment reference.
- ★ [vllm-project/aibrix](https://github.com/vllm-project/aibrix) — Cost-efficient, pluggable infrastructure components for GenAI inference.
- ★ [anduril/lattice-sdk-python](https://github.com/anduril/lattice-sdk-python) — SDK for Lattice, Anduril's command-and-control platform for autonomous systems ([Rust](https://github.com/anduril/lattice-sdk-rust) too).
- ★ [dusty-nv/jetson-containers](https://github.com/dusty-nv/jetson-containers) — The ML container ecosystem for NVIDIA Jetson edge deployment.
- ★ [NVIDIA-AI-IOT/deepstream_python_apps](https://github.com/NVIDIA-AI-IOT/deepstream_python_apps) — DeepStream Python bindings for edge video-analytics pipelines.
- [open-rmf/rmf](https://github.com/open-rmf/rmf) — Open Robotics Middleware Framework: multi-fleet robot coordination in shared spaces.

## Papers & meta-lists

- ★ [FoundationAgents/awesome-foundation-agents](https://github.com/FoundationAgents/awesome-foundation-agents) — Papers and repos toward foundation agents.
- ★ [davanstrien/awesome-synthetic-datasets](https://github.com/davanstrien/awesome-synthetic-datasets) — Curated synthetic dataset resources.
- ★ [jslee02/awesome-entity-component-system](https://github.com/jslee02/awesome-entity-component-system) — ECS libraries and resources; the architecture pattern under real-time robot software.
- [GT-RIPL/Awesome-LLM-Robotics](https://github.com/GT-RIPL/Awesome-LLM-Robotics) — Comprehensive list of LLM/VLM-for-robotics papers with code.
- [jslee02/awesome-robotics-libraries](https://github.com/jslee02/awesome-robotics-libraries) — The classic curated list of robotics libraries and simulators.

---

Maintained by [@everettVT](https://github.com/everettVT). If a project belongs here and isn't, open a PR.
