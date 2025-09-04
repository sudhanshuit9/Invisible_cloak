# Invisible Cloak using OpenCV

Turn yourself invisible just like Harry Potter’s cloak!
This project uses OpenCV and image processing techniques to create a magical invisibility effect by replacing the cloak area with the captured background.

# Features

🎥 Real-time webcam feed processing

🎨 Supports multiple cloak colors (Red, Blue, Green)

🖼️ Background capture & recalibration (b key)

💾 Record output video (r key)

📸 Take snapshots (s key)

❌ Quit anytime (q key)

⚙️ Configurable cloak color, camera index, and debug masks

# ⚙️ How It Works

Background Capture – The camera records a static background before you step into the frame.

Color Detection – A specific cloak color (e.g., red, blue, green) is detected using HSV color space.

Mask Creation – Morphological operations clean the mask for smooth edges.

Background Replacement – The detected cloak area is replaced with the saved background.

# 🚀 Installation & Setup
1. Clone the repository
git clone https://github.com/your-username/invisible-cloak.git
cd invisible-cloak

# Create & activate virtual environment 
python -m venv venv

source venv/bin/activate   # Mac/Linux

venv\Scripts\activate      # Windows

# Install dependencies
pip install opencv-python numpy

# Run the project
python cloak.py
