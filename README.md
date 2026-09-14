NeuroEdge AI

Real-time, privacy-focused AI that runs directly on-device using Snapdragon®.

NeuroEdge AI is an intelligent, real-time AI solution designed to deliver fast, personalized, and privacy-focused experiences directly on the device. By leveraging on-device AI capabilities powered by Snapdragon®, the project minimizes dependence on cloud processing — enabling low-latency responses, improved privacy, and efficient performance. NeuroEdge AI demonstrates how edge intelligence can make everyday applications smarter, faster, and more accessible while reducing reliance on constant internet connectivity
How to run the HTML prototype (works immediately)
Bashcd NeuroEdgeAI/web
python3 -m http.server 8080
Open http://localhost:8080 in Chrome / Edge.
What you can do right now:

Type messages and get intelligent on-device-style replies
Click the microphone → speak (Web Speech API)
Upload an image → visual analysis
Upload a document (try models/sample_confidential.txt) → private summarization + key points
Watch the live latency, component status, and “🔒 On-Device” privacy indicators


Project contents









































PathDescriptionweb/Fully working HTML/JS/CSS prototypesrc/orchestration/Central AI engine + routersrc/models/LLM, ASR, Vision, OCR, Embeddings (mock + Snapdragon-ready hooks)src/rag/Document chunking + retrieval pipelinesrc/monitoring/Real-time latency & status trackerdocs/Architecture + Snapdragon optimization guidemodels/sample_confidential.txtTest documentandroid/Notes for native Snapdragon port

Next steps toward real Snapdragon hardware

Replace the mock methods in src/models/* with quantized models running on QNN / SNPE / ONNX Runtime Qualcomm EP
Port the same orchestration logic to Kotlin + Jetpack Compose
Measure real NPU latency, memory, and power on target Snapdragon device

The architecture, response contracts, privacy badges, and performance dashboard are already designed for that path
