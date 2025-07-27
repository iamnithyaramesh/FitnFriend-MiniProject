

# FitnFriend

**FitnFriend** is an immersive fitness engagement platform that leverages **WebXR (A-Frame)** for interactive fitness guidance and motivation. Built as a mini-project, the application helps users build consistent workout habits, track performance, and stay encouraged with virtual fitness companions in an AR/VR-enhanced environment.

---

## Features

* **User Authentication**: Secure login and session-based access
* **Workout Logging**: Track daily workouts (type, reps, duration)
* **Virtual Fitness Companion**: Encouraging avatar rendered using A-Frame
* **AR/VR Workout Visualization**: Render personalized workout scenes in browser via WebXR
* **Progress Tracking**: View summaries and weekly consistency reports
* **Companion Logic**: Mood and motivation-based interaction model

---

## AR/VR Integration

* **A-Frame**: Used for rendering virtual fitness scenes, environments, and avatars
* **Scene Embedding**: Virtual gym scene rendered on specific pages using `<a-scene>`
* **Interaction**: User actions (clicks, progress logs) trigger animation or voice prompts

---

## Tech Stack

* **Frontend**: HTML, CSS, JavaScript, A-Frame (WebXR)
* **Backend**: Python (Flask)
* **Templating**: Jinja2
* **Assets**: 3D models and environment via A-Frame primitives or custom `.glb/.gltf` models

---

## Folder Structure

```
FitnFriend/
├── app.py                # Flask backend
├── database/             # SQLite DB files
├── sql_queries/          # SQL scripts
├── static/               # Stylesheets and image assets
├── templates/            # HTML templates with embedded A-Frame
├── bugs.txt              # Bug log
├── to_do.txt             # Task log
├── images.jpeg, ssn.png  # Visual assets
```

---

## Getting Started

### Prerequisites

* Python 3.8+
* Flask
* A-Frame JS (included via CDN in HTML)

### Installation

```bash
git clone https://github.com/iamnithyaramesh/FitnFriend-MiniProject.git
cd FitnFriend-MiniProject
pip install flask
```

### Running the Application

```bash
python app.py
```

Access the app at `http://localhost:5000` in your browser.

---

## Example A-Frame Integration (in template)

```html
<a-scene embedded>
  <a-box position="0 1 -3" color="#4CC3D9" animation="property: rotation; to: 0 360 0; loop: true; dur: 5000"></a-box>
  <a-sky color="#ECECEC"></a-sky>
</a-scene>
```

This renders an animated workout object in 3D to gamify the user experience.

---

## Future Enhancements

* Voice-guided fitness sessions
* Multiplayer fitness buddy environment in VR
* Integration with smart wearables for real-time feedback
* Firebase-based user analytics

---

