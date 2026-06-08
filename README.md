# TALKING BOT CONTROLLER
  A browser-based interactive robot controller with a 3D robot model, mood controls, movement commands, voice recognition,  
  and a built-in chat interface — all running in a single HTML file with no backend required.


# FEATURES
  3D Robot Viewer — loads a .glb model using Three.js with ambient and directional lighting
  Mood Control — set the robot's mood to Happy, Sad, Angry, or Neutral with visual feedback
  Movement Controls — D-pad layout (Forward, Back, Left, Right, Stop) that moves and rotates the robot in 3D space
  Voice Commands — speak movement or mood commands using the Web Speech API
  Chat Interface — type messages and get rule-based responses from the bot
  Text-to-Speech — the robot speaks its replies out loud using the browser's speech synthesis


# Project Structure
robot/
├── talkingbot_main.html       # Main application file (all HTML, CSS, JS in one file)
└── robot.glb                  # 3D robot model (GLTF binary format)

The entire app lives in talkingbot_main.html. The only external dependency is robot.glb which must be in the same folder.



# HOW TO USE

MOOD CONTROLS
Click any mood button on the left panel. The status indicator updates and the robot speaks the new mood.
ButtonEffect:
😄 Happy: Sets mood to happy
😢 Sad: Sets mood to sad
😠 Angry: Sets mood to angry
😐 Neutral: Resets to neutral

MOVEMENT CONTROLS
Use the D-pad to move the robot within the 3D scene.
ButtonAction: 
▲ Forward: Moves robot forward (Z+)
▼ Back: Moves robot backward (Z−)
◀ Left: Rotates robot left
▶ Right: Rotates robot right
■ Stop: Robot says "Stopped"

VOICE COMMAND
Click the 🎙 Speak mood or movement button, then say a command like:
"forward", "back", "left", "right"
"happy", "sad", "angry", "neutral"

CHAT
Type any message in the input box and press Send or hit Enter. The bot replies based on a built-in keyword rule set and speaks the response aloud.
Sample things to say:
hello, what's your name, tell me a joke
how are you, who made you, what can you do
bye, thank you


# TECH STACK
HTML / CSS / JS -> UI and application 
Three.js r128 -> 3D rendering and model loading
GLTFLoader -> Loading the .glb robot model
Web Speech API -> Voice recognition (input) and speech synthesis (output)
No frameworks. No build tools. No npm install. Just open and run.


