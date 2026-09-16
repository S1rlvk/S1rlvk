# Sarthak Sattigeri
**ML Researcher | Vision-Language Models, Robotics & Evaluation**

Email: ssattigeri65@gmail.com  
Research interests: VLM/VLA evaluation, robot manipulation, part grounding, 3D vision, benchmark design

## Education
**Manipal University Jaipur** — B.Tech, Computer Science & Biosciences, 2025–Present  
Second-year undergraduate focused on multimodal learning, robotics, and empirical ML research.

## Research Publications & Manuscripts

### GroundBench: A Factorized, Counterfactual Benchmark for Locating VLM Affordance Failures
**arXiv:2609.13308** — Sep 2026  
- Designed a six-condition branch-and-merge benchmark separating target identity, target region, and mechanics across three OpenAI VLMs and 1,068 scored predictions.
- Found that target region alone stayed at or below a 0.53 majority baseline (0.26/0.26/0.53), while identity alone reached 0.74/0.68/0.68; no-vision controls exposed category-to-action shortcuts.
- Built a frozen 32-object, 74-pair action-contrast set with object-clustered bootstrap reporting; GPT-5 reached 0.86 pooled compliance but failed all 9 observed push-to-lift-vertical transitions.
- Submitted to NeurIPS 2026 RoboPAD workshop.

### Part Grounding, Not Action Knowledge: Locating the Bottleneck in VLM Affordance Prediction
**arXiv:2609.13225** — Sep 2026  
- Evaluated 8 VLMs across Alibaba, OpenAI, and Anthropic on 19 articulated GAPartNet objects plus 28 real-tool images.
- Naming the target part increased action accuracy by 0.32–0.63 for every model, moving the range from 0.158–0.474 to 0.684–0.947 and push recall from 0–1/8 to 7–8/8.
- Audited the benchmark against trivial baselines, catching a localization threshold that let a constant center score 0.929/0.947 and an action-label rule wrong on 4 of 19 objects.
- Submitted to NeurIPS 2026 VLM4RWD and CoRL 2026 RoboFineMani workshops.

### Geometry Helps Grounded Action Selection Only Under the Right Interface
**Manuscript in progress** — Sep 2026  
- Extended GroundBench with VGGT-derived visual geometry on the same frozen 74 counterfactual pairs, holding target identity and localization fixed.
- For Qwen3-VL-8B, a matched VGGT geometry tile improved compliance from 0.554 to 0.689 over an RGB-only crop (+0.135 [0.000, 0.288]), while serialized 9-parameter geometry reduced compliance to 0.324.
- Repeated the image-vs-geometry contrast on three Claude models; the Qwen effect did not replicate cleanly, indicating strong model and interface dependence.

### Extending Beacon to Hindi: Cultural Adaptation Drives Cross-Lingual Sycophancy
**arXiv:2602.00046** — Jan 2026  
- Designed a three-condition English/Hindi experiment across four open-weight instruction-tuned models to separate language encoding from cultural adaptation.
- Measured 12–16 pp higher sycophancy in Hindi and isolated cultural adaptation as the dominant driver (delta 14 pp, 95% CI [4, 26]) versus language encoding (delta 2 pp).

## Research Experience

### Fidelity Dynamics — Research Intern, Vision-Only Manipulation
**Feb–Mar 2026**  
- Built a Qwen2.5-VL pipeline for egocentric screwdriver videos using 30-second chunks and sparse frame sampling to segment REACH, ALIGN, INSERT, ROTATE, WITHDRAW, and IDLE phases.
- Compared semantic next-phase prediction with a 10D kinematic representation from MediaPipe and optical flow: 93.0% vs. 9.3% accuracy, diagnosing occlusion and temporal aliasing as key failure modes.
- Integrated depth estimation, hand tracking, temporal filtering, and structured manifests for downstream manipulation learning experiments.

## Selected Technical Projects

### IMU vs. Vision for Activity Boundary Detection — WEAR Dataset
**2026**  
- Ran 18-subject leave-one-subject-out evaluation comparing wrist IMU with precomputed I3D video features for subtask-boundary detection.
- IMU outperformed video features for boundary detection (F1 0.200 vs. 0.149); majority-vote smoothing improved raw boundary F1 from 0.069 to 0.108.

### Structure-from-Motion Pipeline
**2024–2025**  
- Implemented feature extraction, matching, pose recovery, triangulation, and bundle adjustment for iPhone imagery, reaching 3.3 px mean reprojection error.
- Used the project to study monocular scale ambiguity and camera geometry from first principles.

### VLM Force Prediction — Robotic Grasping
**Feb 2026**  
- Built a 50-object zero-shot benchmark for gripper-force prediction with physics-based ground truth; observed weak non-significant correlation (Pearson r=0.237, p=0.097) and strongly quantized model outputs.
- Identified a 66.7% safety-violation rate on fragile objects and proposed separating semantic material/fragility estimation from physics-based force computation.

## Technical Skills
- **Research:** Benchmark design, counterfactual evaluation, ablations, bootstrap confidence intervals, error analysis, dataset auditing
- **ML / VLMs:** PyTorch, Hugging Face Transformers, Qwen-VL, multimodal prompting, LLM/VLM evaluation, scikit-learn
- **Vision / Robotics:** OpenCV, MediaPipe, MiDaS, VGGT, SfM, egocentric video, IMU processing, Kalman filtering
- **Programming:** Python (primary), C/C++, SQL, Rust (basic), TypeScript
- **Tools:** Git/GitHub, NumPy, Pandas, Matplotlib, LM Studio, LaTeX, Linux/macOS

## Additional
Languages: English (fluent), Hindi (native). Open-source research artifacts and evaluation code available on GitHub.
