🌿 Leaf Health Analysis System

AI-powered modular plant health evaluation using computer vision and generative AI.

This system performs end-to-end leaf analysis including:

🌿 Leaf Detection

🦠 Disease Classification

💧 Dryness Assessment

🌱 Vegetation & Green Index Metrics

🐛 Pest Detection

🧠 AI-Generated Farmer-Friendly Report

Built with a modular architecture where each component runs independently.

🚀 Features
1️⃣ Leaf Detection

Uses YOLO object detection to isolate the leaf region from background noise.

2️⃣ Disease Classification

ONNX-based deep learning model (MobileNetV2 backbone) predicts leaf disease with confidence score.

3️⃣ Dryness Analysis

Composite dryness metrics derived from:

Green ratio

Brown ratio

Saturation mean

Texture variance

Structural roughness

Provides:

Dryness score (0–1)

Dryness level (Low / Moderate / High)

4️⃣ Green Index Metrics

Includes vegetation indices such as:

Excess Green (ExG)

Normalized Green

Green Score

Used for detecting early stress and chlorosis.

5️⃣ Pest Detection

YOLO-based insect detection returning:

Pest count

Class labels

Bounding boxes

Confidence scores

6️⃣ GenAI Report

Gemini API generates:

Structured health summary

Risk level assessment

Farmer-friendly explanation

Actionable recommendations

🧠 System Architecture

Vision Layer:

Leaf Detection (YOLO)

Pest Detection (YOLO)

Disease Classification (ONNX)

Dryness Analyzer

Green Index Calculator

Reasoning Layer:

Gemini LLM generates interpretive plant health reports.

Each module executes independently.
Failure in one module does NOT break the pipeline.
