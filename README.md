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



