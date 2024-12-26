# SportDesignAI

SportDesignAI is an AI-powered platform for designing custom sportswear sets (shirt and pants) with a friendly conversational interface, interactive 3D visualization, and exportable 2D manufacturing templates. The platform leverages machine learning to generate unique designs based on pre-trained patterns and supports iterative refinements using natural language prompts.

---

## Features

- **AI-Driven Design**:
  - Generate unique sportswear designs (patterns, colors, and styles) with machine learning.
  - Learn from pre-made templates to produce dynamic and engaging designs.

- **Conversational Interface**:
  - Chat with the AI to describe your ideal design, refine existing designs, and receive suggestions.
  - Supports memory to ensure the user's changes build on previous interactions.

- **3D Visualization**:
  - View the designed sportswear in an interactive 3D model.
  - Rotate, zoom, and interact with the design in real-time.

- **Design Memory**:
  - Save and modify designs incrementally.
  - Option to reset to the default all-white template.

- **Export to 2D Templates**:
  - Convert the 3D design into a flat, vector-based 2D template (SVG or PDF) ready for manufacturing.
  - Templates include stitching and cutting guidelines.

---

## How It Works

1. **Start a New Design**:
   - Begin by chatting with the AI. For example: "Create a blue shirt with white stripes and black pants."

2. **Refine the Design**:
   - Make adjustments iteratively. For instance: "Add a logo to the chest" or "Make the pants darker."

3. **View in 3D**:
   - Preview the design in an interactive 3D model with real-time updates.

4. **Export to 2D**:
   - Once finalized, export the design as a 2D template ready for manufacturing.

5. **Reset or Save**:
   - Reset the design to its default state or save it for future use.

---

## Tech Stack

### **Frontend**
- **React.js**: User interface development.
- **Three.js**: 3D model rendering and interaction.

### **Backend**
- **Node.js**: Server-side logic.
- **Express.js**: API for communication between the frontend, AI, and database.

### **AI**
- **PyTorch/TensorFlow**: Training and running the machine learning model for design generation.
- **Hugging Face**: For conversational AI capabilities.

### **Database**
- **MongoDB**: Storing user designs and conversational history.

### **Export Tools**
- **Fabric.js/SVG.js**: Convert 3D models into vector-based 2D templates.

## Folder Structure

SportDesignAI/
├── ai/                          # Machine learning models and scripts
│   ├── models/                  # Pre-trained and fine-tuned models
│   ├── training/                # Scripts and datasets for training the AI
│   ├── inference.py             # AI design generation logic
│   └── utils.py                 # Helper functions for AI-related tasks
│
├── backend/                     # Server-side code
│   ├── models/                  # MongoDB schema definitions
│   │   ├── Design.js            # Schema for storing designs
│   │   ├── User.js              # Schema for user data
│   │   └── ChatHistory.js       # Schema for storing chat history
│   ├── routes/                  # API endpoints
│   │   ├── designRoutes.js      # Endpoints for design-related actions
│   │   ├── chatRoutes.js        # Endpoints for chat and AI interactions
│   │   └── userRoutes.js        # Endpoints for user management
│   ├── controllers/             # Business logic for routes
│   │   ├── designController.js  # Handle design requests
│   │   ├── chatController.js    # Handle chat-based actions
│   │   └── userController.js    # Handle user-related actions
│   ├── memory/                  # Design memory and history management
│   │   ├── memoryManager.js     # Logic for saving and rolling back designs
│   ├── utils/                   # Utility functions for backend
│   │   ├── fileUtils.js         # File handling utilities
│   │   └── errorHandler.js      # Error handling middleware
│   ├── server.js                # Main server file
│   └── package.json             # Node.js dependencies
│
├── frontend/                    # React.js app for the UI
│   ├── public/                  # Public assets (e.g., index.html)
│   │   ├── index.html           # Entry point for React app
│   ├── src/                     # Source files for React
│   │   ├── components/          # Reusable components
│   │   │   ├── ChatBox.js       # Chat interface for user interaction
│   │   │   ├── ThreeDViewer.js  # 3D model viewer
│   │   │   ├── Toolbar.js       # Toolbar for color and pattern selection
│   │   │   ├── DesignMemory.js  # Component for managing design history
│   │   │   └── ExportButton.js  # Button for exporting designs
│   │   ├── pages/               # Page-level components
│   │   │   ├── HomePage.js      # Landing page
│   │   │   ├── DesignPage.js    # Main design interface
│   │   │   ├── ChatPage.js      # Page for interacting with the chat interface
│   │   │   └── ExportPage.js    # Page for downloading templates
│   │   ├── assets/              # Static files (images, icons)
│   │   ├── App.js               # Main React app component
│   │   └── index.js             # Entry point for React
│   ├── package.json             # Node.js dependencies for frontend
│   └── .env                     # Environment variables for frontend
│
├── templates/                   # Logic for generating 2D templates
│   ├── export.js                # Conversion logic (3D to 2D templates)
│   ├── shirtTemplate.svg        # Base template for shirts
│   ├── pantsTemplate.svg        # Base template for pants
│   └── utils.js                 # Helper functions for template generation
│
├── docs/                        # Documentation and guides
│   ├── architecture.md          # Project architecture overview
│   ├── api.md                   # API documentation
│   └── contributing.md          # Contribution guidelines
│
├── scripts/                     # Deployment and automation scripts
│   ├── deploy.sh                # Script for deploying the application
│   ├── build.sh                 # Script for building the project
│   └── test.sh                  # Script for running tests
│
├── tests/                       # Testing files
│   ├── frontend/                # Frontend tests (e.g., Jest)
│   │   ├── components/          # Component-level tests
│   │   └── pages/               # Page-level tests
│   ├── backend/                 # Backend tests (e.g., Mocha/Chai)
│   │   ├── routes/              # Tests for API routes
│   │   ├── controllers/         # Tests for controllers
│   │   └── utils/               # Tests for utility functions
│   └── e2e/                     # End-to-end tests
│
├── .gitignore                   # Files and directories to ignore in Git
├── README.md                    # Project documentation
├── requirements.txt             # Python dependencies for AI
└── LICENSE                      # License file


