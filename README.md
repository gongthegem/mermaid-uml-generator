# Mermaid UML Generator

A sophisticated web application for visualizing, editing, and managing UML diagrams using Mermaid syntax. This tool streamlines the process of creating, modifying, and maintaining UML diagrams for software architecture documentation.

![Mermaid UML Generator](https://placeholder-for-project-screenshot.com)

## 🚀 Features

- **Interactive Diagram Gallery**: Browse and manage multiple diagrams in a visual grid
- **Advanced Diagram Editing**: Edit Mermaid syntax with real-time preview
- **Class Manipulation**: Drag-and-drop classes between diagrams
- **Smart Rendering**: Incremental, cached rendering for performance optimization
- **Expandable/Collapsible Classes**: Toggle visibility of class details
- **Asynchronous Processing**: Background rendering with prioritized queue
- **Batch Operations**: Process multiple diagrams simultaneously
- **Export Options**: Save diagrams in various formats (SVG, PNG, PDF)
- **Zoom & Pan**: Navigate large diagrams with intuitive controls
- **Selection Tools**: Select and manipulate diagram elements
- **Contextual UI**: Minimal interface with context-sensitive controls

## 📋 Installation & Usage

### Prerequisites
- Node.js (v14.0.0 or higher)
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/mermaid-uml-generator.git
cd mermaid-uml-generator

# Install dependencies
npm install
# or
yarn install
```

### Running the Application

```bash
# Development mode
npm run dev
# or
yarn dev

# Production build
npm run build
npm run start
# or
yarn build
yarn start
```

### Basic Usage

1. **Load Diagrams**: Upload Mermaid files or select a directory
2. **Browse Gallery**: View thumbnails of all available diagrams
3. **Edit Diagrams**: Click on a thumbnail to open the diagram editor
4. **Modify Classes**: Drag classes between diagrams or edit directly
5. **Save Changes**: Export diagrams in your preferred format

## 🛠️ Tech Stack

- **Frontend Framework**: React with TypeScript
- **Backend/Server**: Node.js & Express.js
- **Core Libraries**:
  - mermaid.js (UML syntax parsing and rendering)
  - D3.js (Enhanced SVG manipulation)
  - SVG.js (Additional SVG capabilities)
- **State Management**: Redux or Context API
- **Processing & Rendering**:
  - Web Workers (Background rendering)
  - Canvas/WebGL (High-performance rendering)
- **Build Tools**: Webpack/Vite & Jest
- **CSS Framework**: Tailwind CSS
- **Storage**:
  - IndexedDB/localStorage (Client-side caching)
  - File System Access API (Direct file interactions)

## 📂 Project Structure

```
src/
├── components/           # React components (UI Layer)
│   ├── GalleryView/      # Diagram gallery and thumbnails
│   ├── DiagramViewer/    # Expanded diagram view
│   ├── ContextualControls/ # Minimal UI controls
│   └── common/           # Shared UI components
├── services/             # Core services
│   ├── FileSystemService/ # File operations
│   ├── MermaidParser/    # Mermaid syntax parsing
│   ├── DiagramRenderer/  # SVG rendering
│   └── RenderCache/      # Caching system
├── models/               # Data models
│   ├── DiagramData/      # Diagram structure
│   ├── ClassNode/        # Class representation
│   ├── Relationship/     # Class relationships
│   └── RenderedDiagram/  # Processed diagrams
├── processors/           # Processing system
│   ├── RenderProcessor/  # Parallel rendering
│   └── ProcessingQueue/  # Priority queue
├── editors/              # Editing system
│   ├── DiagramEditor/    # Diagram modification
│   └── InteractionManager/ # User interactions
├── utils/                # Utility functions
├── store/                # State management
├── workers/              # Web Workers
└── App.tsx               # Main controller
```

## 🌟 Performance Optimizations

The application implements several performance strategies:
- **Caching**: Fast access to previously rendered SVGs
- **Parallel Processing**: Controlled concurrency for rendering tasks
- **Incremental Rendering**: Only re-render modified diagram parts
- **Prioritized Queue**: Visible elements rendered first for better UX

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.