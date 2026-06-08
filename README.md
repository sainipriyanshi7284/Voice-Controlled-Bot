# TALKING BOT CONTROLLER
  A browser-based interactive robot controller with a 3D robot model, mood controls, movement commands, voice recognition,  
  and a built-in chat interface — all running in a single HTML file with no backend required.


# FEATURES
  3D Robot Viewer — loads a .glb model using Three.js with ambient and directional lighting <br>
  Mood Control — set the robot's mood to Happy, Sad, Angry, or Neutral with visual feedback <br>
  Movement Controls — D-pad layout (Forward, Back, Left, Right, Stop) that moves and rotates the robot in 3D space <br>
  Voice Commands — speak movement or mood commands using the Web Speech API <br>
  Chat Interface — type messages and get rule-based responses from the bot <br>
  Text-to-Speech — the robot speaks its replies out loud using the browser's speech synthesis <br>


# Project Structure
robot/ <br>
├── talkingbot_main.html       # Main application file (all HTML, CSS, JS in one file) <br>
└── robot.glb                  # 3D robot model (GLTF binary format) <br>

The entire app lives in talkingbot_main.html. The only external dependency is robot.glb which must be in the same folder.



# HOW TO USE

MOOD CONTROLS <br>
Click any mood button on the left panel. The status indicator updates and the robot speaks the new mood. <br>
ButtonEffect: <br>
😄 Happy: Sets mood to happy <br>
😢 Sad: Sets mood to sad <br>
😠 Angry: Sets mood to angry <br>
😐 Neutral: Resets to neutral <br> <br>

MOVEMENT CONTROLS <br>
Use the D-pad to move the robot within the 3D scene. <br>
ButtonAction:  <br>
▲ Forward: Moves robot forward (Z+) <br>
▼ Back: Moves robot backward (Z−) <br>
◀ Left: Rotates robot left <br>
▶ Right: Rotates robot right <br>
■ Stop: Robot says "Stopped" <br> <br>

VOICE COMMAND <br>
Click the 🎙 Speak mood or movement button, then say a command like: <br>
"forward", "back", "left", "right" 
"happy", "sad", "angry", "neutral"  <br><br>

CHAT <br>
Type any message in the input box and press Send or hit Enter. The bot replies based on a built-in keyword rule set and speaks the response aloud. <br>
Sample things to say: 
hello, what's your name, tell me a joke
how are you, who made you, what can you do
bye, thank you


# TECH STACK
HTML / CSS / JS -> UI and application  <br>
Three.js r128 -> 3D rendering and model loading <br>
GLTFLoader -> Loading the .glb robot model <br>
Web Speech API -> Voice recognition (input) and speech synthesis (output) <br>
No frameworks. No build tools. No npm install. Just open and run. <br>


