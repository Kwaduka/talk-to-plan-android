# talk-to-plan-android
Talk to Plan is a native Android application built with Kotlin that converts spoken intentions into structured, actionable plans using speech-to-text transcription and AI-driven task analysis.

````markdown
# Talk to Plan

## Title & Objective

**Talk to Plan** - An Android application that converts spoken intentions into structured, actionable plans using transcription and AI-based task analysis.

**What technology did you choose?**  
Kotlin with native Android development (Android Studio, Android SDK).

**Why did you choose it?**  
To learn modern, first-class Android development using Kotlin while gaining hands-on experience with mobile app architecture, permissions, local storage, and API integration.

**What's the end goal?**  
To build a practical Android app that transforms unstructured voice input into organized plans with tasks, priorities, time frames, and categories, while achieving deep competence in Kotlin and Android fundamentals.

---

## Project Description

Talk to Plan is a voice-driven planning application that allows users to speak about what they want to accomplish over a day, week, or any defined period. The app records the user’s voice, converts speech to text using a transcription API, and then sends the text to an AI service that produces a structured plan.

The resulting plan includes clearly defined tasks, priority levels, suggested time frames when mentioned, and logical categories such as work, health, learning, or personal. Plans are stored locally on the device, with optional user accounts for backup and continuity.

The project prioritizes clarity, usefulness, and technical soundness over visual complexity.

---

## Brief Overview of the Technology

**Kotlin** is a modern, statically typed programming language officially supported by Google for Android development. It emphasizes safety, conciseness, and expressiveness.

Kotlin is widely used in:
- Native Android applications
- Backend services (Ktor, Spring)
- Multiplatform projects
- Desktop applications

**Real-life examples:** Google apps, Pinterest Android app, Trello Android app, Netflix Android client.

Android development with Kotlin enables tight integration with the operating system, predictable performance, and long-term maintainability.

---

## System Requirements

- **OS:** Windows, Linux, or macOS
- **IDE:** Android Studio (recommended)
- **SDK:** Android SDK (installed via Android Studio)
- **Language:** Kotlin (bundled with Android Studio)
- **Optional:** Git for version control
- **Internet:** Required for transcription and AI features

---

## Installation and Setup Instructions

### Install Android Studio

1. Download Android Studio from the official Android developer website.
2. Install using default settings.
3. During setup, ensure the following are selected:
   - Android SDK
   - Android SDK Platform Tools
   - Android Emulator

### Verify Installation

- Open Android Studio
- Create a new project
- Select **Empty Activity**
- Choose **Kotlin** as the language
- Run the project on an emulator

If the default app launches successfully, the environment is ready.

---

## Minimal Working Example

### Basic Kotlin Activity

```kotlin
package com.example.talktoplan

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity

class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
    }
}
````

This confirms:

* Kotlin compilation works
* Android lifecycle methods are understood
* UI rendering is functional

Run the app using the Android Studio Run button or `Shift + F10`.

---

## Enhanced Features

The MVP includes the following core enhancements:

1. **Voice Recording**

   * Uses device microphone with runtime permission handling

2. **Speech-to-Text**

   * Audio is sent to a transcription API
   * Clean text is returned for processing

3. **AI-Based Planning**

   * Text is analyzed to generate tasks, priorities, and categories

4. **Structured Plan Display**

   * Tasks are grouped logically and displayed clearly

5. **Local Storage**

   * Plans are stored on-device for offline access

6. **Optional Authentication**

   * Users may create accounts to sync plans
   * App remains usable without login

---

## Technologies Used

* **Language:** Kotlin
* **Platform:** Android
* **IDE:** Android Studio
* **Architecture Concepts:** Activities, lifecycle management, permissions
* **APIs:** Speech-to-text API, AI planning API
* **Storage:** Local persistence (Room or SharedPreferences)
* **Key Concepts:** Coroutines, data classes, HTTP requests, JSON parsing

---

## AI Prompt Journal

### Prompt 1: Kotlin and Android Fundamentals

**Prompt Used:**
"Explain Kotlin and Android development concepts for a developer transitioning from web development."

**AI Response Summary:**
Clear explanation of Kotlin’s design goals, Android architecture, and how mobile concepts differ from web frameworks.

**How It Helped:**
Established a strong conceptual foundation before writing production code.

---

### Prompt 2: Environment Setup

**Prompt Used:**
"Guide me step by step to set up Android Studio and run a Kotlin app."

**AI Response Summary:**
Detailed setup process including SDK installation, emulator configuration, and project creation.

**How It Helped:**
Prevented common setup errors and ensured a stable development environment.

---

### Prompt 3: Voice-to-Plan Flow

**Prompt Used:**
"Explain how to build an Android app that records audio, transcribes it, and processes it with AI."

**AI Response Summary:**
Outlined audio handling, permission management, asynchronous API calls, and data modeling.

**How It Helped:**
Enabled a clean architectural approach rather than trial-and-error implementation.

---

## Common Issues & Fixes

| Issue                        | Error Message        | Solution                                  |
| ---------------------------- | -------------------- | ----------------------------------------- |
| Microphone permission denied | Audio not recorded   | Request runtime permission explicitly     |
| App crashes on startup       | NullPointerException | Check lifecycle initialization order      |
| API call failure             | Network error        | Validate internet connection and API keys |
| UI freezes                   | App not responding   | Move network calls to coroutines          |
| Data not saved               | Empty plan list      | Verify local storage write operations     |

---

## Reference Resources

* Android Developer Documentation
* Kotlin Language Documentation
* Android Studio Guides
* Android Architecture Components Overview
* Official Android Codelabs

---

## Learning Reflections

Building Talk to Plan reinforced several critical lessons:

* **Thinking in Lifecycles:** Android apps demand lifecycle awareness, not just function calls
* **Asynchronous Discipline:** Network and audio operations must never block the UI
* **Data Modeling:** Clear data structures simplify AI integration and UI rendering
* **Permission Awareness:** Mobile development requires explicit user trust management

The most important insight was that mobile development rewards intentional design more than rapid experimentation.

---

## Next Steps / Tips

* Add reminders and notifications
* Integrate calendar synchronization
* Improve AI prompt tuning for better plans
* Introduce plan editing and task completion tracking
* Add basic testing and logging
* Publish an internal beta build

---

## License

This project is provided as-is for educational and personal learning purposes.

```
```

