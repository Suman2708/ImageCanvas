🖼️ Stencil Image Editor
This is a React-based image editor built with Fabric.js. It allows users to upload images, view them within a fixed stencil (cut-out area), and interactively zoom, reset, and drag the image.

🚀 Features
📤 Upload an image (JPEG, PNG, etc.)

🖼️ Image fits into a fixed stencil frame

🔍 Zoom in and zoom out on the uploaded image

🎯 Drag the image inside the stencil to adjust view

♻️ Reset the image to its initial size and position

📱 Responsive canvas that adjusts with the browser window

🧩 Key Parts of the Implementation
Canvas Initialization
A Fabric canvas is created and initialized inside a useEffect.

The canvas resizes dynamically based on the screen size (80vw x 60vh).

Stencil Area
A non-selectable fabric.Rect is added as a clip path to simulate a stencil window.

Only the content inside this stencil area is visible.

Image Upload
User uploads an image using a file input.

The uploaded image is automatically scaled and positioned to fit nicely inside the stencil.

If another image is uploaded, the previous one is removed.

Zoom Functionality
Users can zoom in or out using buttons.

Zooming adjusts the scale of the image while constraining it within the stencil.

Dragging
After upload, the image is draggable in all directions within the canvas.

Locking is removed to allow manual adjustments.

Reset
Resets the image back to the initial scaled size and position (like after upload).

🛠️ Tech Stack
React

Redux (for state management)

Tailwind CSS (for UI styling)

Fabric.js (for canvas operations)

📂 How to Run Locally
bash
Copy
Edit
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
npm install
npm start
