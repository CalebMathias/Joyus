# Joyus: Your Sentient AI Assistant

Joyus is an advanced AI assistant designed to integrate seamlessly into your environment, combining real-time computer vision, audio processing, and machine learning to monitor, analyze, and assist in various tasks. Inspired by the concept of a proactive AI like Jarvis from Iron Man, Joyus is capable of detecting anomalies, analyzing environments, and interacting with users through intelligent decision-making and natural language responses.

---

## Table of Contents
1. [What is Joyus?](#what-is-joyus)
2. [How Joyus Works](#how-joyus-works)
3. [Detailed Examples of Joyus in Action](#detailed-examples-of-joyus-in-action)
4. [How to Use Joyus](#how-to-use-joyus)

---

## What is Joyus?

Joyus is a fully autonomous and context-aware AI assistant capable of:
- **Surveillance**: Tracks objects and detects anomalies in real-time using video input and YOLO-based object detection.
- **Audio Analysis**: Monitors audio to detect specific events such as gunshots, screams, or explosions using Google's YAMNet.
- **Decision-Making**: Leverages Deep Q-Networks (DQN) to take autonomous actions based on environmental data and detected anomalies.
- **Environment Analysis**: Trains and utilizes multiple machine learning models to detect physics, chemistry, environmental, and space-based anomalies.
- **User Interaction**: Provides natural language responses to user commands and queries.

Joyus is designed to assist in various contexts, such as security monitoring, environmental analysis, and general inquiries, making it a versatile and proactive AI companion.

---

## How Joyus Works

1. **Consciousness Module**:
   - Tracks "alertness" and "confidence" levels based on environmental inputs, such as anomalies and audio activity.
   - Maintains a memory of recent events for context-aware decision-making.

2. **Policy Neural Network (DQN)**:
   - Uses deep reinforcement learning to decide actions such as increasing sensitivity, notifying users, or analyzing the environment.
   - Trains continuously using experience replay to optimize decision-making over time.

3. **Surveillance and Audio Processing**:
   - **Video Input**: Uses YOLO for object detection and DeepSORT for tracking objects.
   - **Audio Input**: Uses YAMNet to detect and classify audio anomalies like gunshots or screams.

4. **Scientific Models**:
   - **Physics Model**: Detects motion-based anomalies.
   - **Chemistry Model**: Identifies hazardous substances.
   - **Environmental Model**: Predicts weather anomalies.
   - **Space Model**: Detects celestial objects.

5. **User Interaction**:
   - Joyus responds to commands such as `status`, `weather`, `people count`, and `anomalies`.
   - Provides natural language responses using pre-trained transformer models (TinyLlama).

---

## Detailed Examples of Joyus in Action

### **Scenario 1: Anomaly Detection and Response**
**Input**: A loud scream is detected in the environment.  
**Output**:
```
I have detected a scream sound, which might indicate distress or emergency.
```

**Action**:  
Joyus logs the event, updates its alertness state, and notifies the user.

### **Scenario 2: User Query - Status**
**Command**: `status`  
**Output**:
```
Alertness: 0.75, Confidence: 0.85, Monitoring 3 entities.
```

### **Scenario 3: User Query - Weather**
**Command**: `weather`  
**Output**:
```
The current weather is clear sky with a temperature of 22.5°C.
```

### **Scenario 4: Environment Analysis**
**Event**: Joyus detects a hazardous substance in a chemistry lab environment.  
**Output**:
```
Analysis complete. Detected anomalies:
- Chemistry: Hazardous substance detected
```

**Action**:  
Logs the event, notifies the user, and increases sensitivity for further monitoring.

### **Scenario 5: Decision-Making**
**Event**: Joyus detects high-speed movement from a tracked entity.  
**Output**:
```
I have detected a high-speed movement from entity ID 12. The speed is 150 pixels per second.
```

**Action**:  
Logs the anomaly, updates its consciousness module, and decides whether to notify the user or take other actions.

---

## How to Use Joyus

### **Prerequisites**
1. **Hardware**:
   - A computer with a webcam or video source.
   - A microphone for audio input.

2. **Software Requirements**:
   - Python 3.8+ installed.
   - Required libraries: TensorFlow, PyTorch, OpenCV, Transformers, Mediapipe, YOLO, and others listed in the source code.

3. **Pre-trained Models**:
   - Download and set up the required models for YOLO, TinyLlama, and YAMNet as specified in the code.

### **Setup Instructions**
1. Clone the repository:
   ```bash
   git clone https://github.com/CalebMathias/Joyus.git
   cd Joyus
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run Joyus:
   ```bash
   python Joyus.py
   ```

### **Available Commands**
- **`status`**: Get the current status of Joyus, including alertness, confidence, and tracked entities.
- **`weather`**: Fetch real-time weather data.
- **`people count`**: Get the number of people currently detected.
- **`anomalies`**: View recent anomalies detected by Joyus.
- **`help`**: List available commands.

### **Interacting with Joyus**
Once Joyus is running:
- Use the **command line** to input commands.
- Joyus will respond with natural language outputs and log events.

### **Exiting Joyus**
To safely shut down Joyus:
1. Press `q` in the video display window.
2. Terminate the application in the terminal.

---

Joyus is a powerful AI assistant capable of adapting to various scenarios. Whether for personal use or professional tasks, Joyus is here to assist you every step of the way! 🚀
