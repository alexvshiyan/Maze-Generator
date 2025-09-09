# 🌀 Maze Generator

A sophisticated web-based maze generation and pathfinding platform designed for testing and visualizing maze algorithms. Built with vanilla HTML, CSS, and JavaScript.

![Maze Generator Screenshot](https://via.placeholder.com/800x400/667eea/ffffff?text=Maze+Generator+Interface)

## 🚀 Live Demo

**[Try the Maze Generator →](https://yourusername.github.io/maze-generator)**

## ✨ Features

### Core Functionality
- **3 Advanced Generation Algorithms**: Each creating unique maze structures
- **Customizable Parameters**: Size, start/end positions, algorithm-specific settings
- **Interactive Visualization**: Real-time rendering with customizable cell sizes
- **Path Solver**: Built-in pathfinding with visual solution display
- **Export Capabilities**: Download mazes as PNG images

### User Interface
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Intuitive Controls**: Logically organized parameter groups
- **Debug Console**: Optional development/testing console (hidden by default)
- **Real-time Feedback**: Instant parameter updates and visual feedback

## 🧩 Algorithms

### 1. Recursive Backtracking 🌿
- **Type**: Classic maze generation
- **Characteristics**: Long winding paths, many dead ends
- **Best for**: Testing pathfinding efficiency on complex mazes
- **Complexity**: High - creates challenging navigation problems

### 2. Sidewinder 🔄
- **Type**: Row-based generation
- **Characteristics**: Horizontal corridors with random vertical passages
- **Best for**: Medium complexity testing scenarios
- **Complexity**: Medium - balanced between open spaces and obstacles

### 3. Maze Islands 🏝️
- **Type**: Multi-level maze generation
- **Characteristics**: Main maze + isolated sub-mazes accessible only through special entrances
- **Parameters**: Number of islands (0.3-0.9 range)
- **Best for**: Testing advanced pathfinding algorithms
- **Complexity**: Very High - requires strategic exploration

## 🎯 Quick Start

### Option 1: Direct Usage
1. **Download** `index.html` from this repository
2. **Open** in any modern web browser
3. **Start generating** mazes immediately!

### Option 2: Clone and Customize
```bash
git clone https://github.com/yourusername/maze-generator.git
cd maze-generator
# Open index.html in your browser
```

### Option 3: GitHub Pages
1. **Fork** this repository
2. **Enable GitHub Pages** in repository settings
3. **Access** your live version at `https://yourusername.github.io/maze-generator`

## 📋 Usage Guide

### Basic Workflow
1. **Configure Maze**: Set dimensions (5-100) and choose generation algorithm
2. **Set Parameters**: Define start/end positions and algorithm-specific settings
3. **Generate**: Click "🎲 Generate Maze" to create the maze structure
4. **Test**: Use "🔍 Check Solvability" to verify and visualize path
5. **Export**: Click "💾 Download PNG" to save results

### Advanced Features
- **🔀 Randomize Start/End**: Quickly test different start/end combinations on the same maze
- **🔧 Debug Console**: Monitor generation process and performance metrics
- **Parameter Validation**: Automatic coordinate range updates and error checking

## 🎨 Interface Layout

### Parameter Organization
**Row 1 - Maze Configuration:**
- Width × Height (5-100 range)
- Algorithm Selection  
- Algorithm-specific parameters (when applicable)

**Row 2 - Visualization & Navigation:**
- Cell Size (5-30px)
- Start Position (X, Y coordinates)
- End Position (X, Y coordinates)

## 🔬 Technical Specifications

### Architecture
- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Rendering**: HTML5 Canvas API
- **Dependencies**: None - completely self-contained
- **Browser Support**: Modern browsers (Chrome 80+, Firefox 75+, Safari 13+, Edge 80+)

### Core Classes
- **`MazeGenerator`**: Handles all maze generation algorithms
- **`MazeRenderer`**: Canvas-based visualization engine
- **`MazeSolver`**: Depth-first search pathfinding implementation

### Performance
- **Small Mazes** (up to 50×50): Instant generation
- **Medium Mazes** (up to 100×100): Under 1 second
- **Large Mazes** (100×100+): May require processing time for Maze Islands
- **Memory Usage**: ~50 bytes per cell, optimized for efficiency

## 🛠️ Customization

### Adding New Algorithms
```javascript
// Add to MazeGenerator class
newAlgorithm() {
    // Your algorithm implementation
}

// Add to switch statement in generateMaze()
case 'new-algorithm':
    currentMaze.newAlgorithm();
    break;
```

### Visual Themes
```css
/* Custom color scheme */
:root {
    --wall-color: #2c3e50;
    --path-color: #ffeb3b;
    --start-color: #4caf50;
    --end-color: #f44336;
}
```

## 📚 Educational Value

### Computer Science Concepts
- **Graph Theory**: Mazes as graphs, traversal algorithms
- **Algorithm Design**: Different approaches to problem-solving
- **Data Structures**: Stacks, queues, and their applications
- **Complexity Analysis**: Time/space trade-offs in algorithms

### Practical Applications
- **Game Development**: Procedural level generation
- **Robotics**: Path planning and navigation
- **Network Routing**: Shortest path algorithms
- **AI Research**: Search strategies and heuristics

## 🎓 Use Cases

### For Developers
- Algorithm testing and benchmarking
- Pathfinding algorithm development (A*, Dijkstra, BFS, DFS)
- Performance optimization research
- Educational tool for computer science concepts

### For Researchers
- Pathfinding research and analysis
- Complexity studies on different maze structures
- Visualization of algorithmic behavior
- Publication-ready maze generation

### For Students
- Interactive learning of graph algorithms
- Understanding maze generation techniques
- Experimentation with different parameters
- Visual algorithm comprehension

## 🚧 Future Enhancements

### Planned Features
- [ ] Additional algorithms (Kruskal's, Prim's, Wilson's)
- [ ] Advanced pathfinding (A*, Dijkstra, Best-First Search)
- [ ] Animation system for step-by-step visualization
- [ ] Export formats (JSON, SVG, data structures)
- [ ] Performance metrics and timing analysis
- [ ] Batch generation for statistical analysis

### Technical Improvements
- [ ] WebGL rendering for large mazes
- [ ] Web Workers for background processing
- [ ] Progressive enhancement features
- [ ] API integration capabilities

## 🤝 Contributing

We welcome contributions! Here are areas where you can help:

### Algorithm Implementations
- New maze generation algorithms
- Advanced pathfinding implementations
- Optimization improvements

### UI/UX Enhancements
- Mobile interface improvements
- Accessibility features
- Visual theme options

### Documentation
- Algorithm explanations
- Code documentation
- Tutorial creation

### Getting Started with Contributions
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-algorithm`)
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 Project Structure

```
maze-generator/
├── index.html              # Main application (single file)
├── README.md               # This file
├── screenshots/            # Example images
│   ├── recursive-backtracking.png
│   ├── sidewinder.png
│   └── maze-islands.png
└── docs/                   # Additional documentation
    ├── algorithms.md       # Detailed algorithm explanations
    └── api-reference.md    # Code documentation
```

## 🔧 Development

### Local Development
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server

# Using PHP  
php -S localhost:8000
```

### Testing Checklist
- [ ] All algorithms generate solvable mazes
- [ ] Start/end positions validate correctly
- [ ] UI responds to parameter changes
- [ ] Console shows/hides properly
- [ ] PNG export works across browsers
- [ ] Mobile interface functions correctly

## 📊 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 80+ | ✅ Fully Supported |
| Firefox | 75+ | ✅ Fully Supported |  
| Safari | 13+ | ✅ Fully Supported |
| Edge | 80+ | ✅ Fully Supported |
| Mobile Safari | 13+ | ✅ Supported |
| Chrome Mobile | 80+ | ✅ Supported |

## 🎮 Controls & Shortcuts

### Mouse Controls
- **Generate**: Click "🎲 Generate Maze"
- **Randomize**: Click "🔀 Randomize Start/End"
- **Solve**: Click "🔍 Check Solvability"
- **Export**: Click "💾 Download PNG"
- **Debug**: Click "🔧 Show/Hide Console"

### Parameter Controls
- **Dimensions**: 5-100 range for width/height
- **Algorithms**: Dropdown selection with auto-parameter display
- **Coordinates**: Automatic validation and range updating
- **Cell Size**: 5-30px for optimal viewing

## 📈 Performance Tips

### For Large Mazes
- Use smaller cell sizes (5-10px) for better performance
- Consider using simpler algorithms for very large mazes
- Monitor memory usage with browser dev tools

### For Smooth Experience
- Generate mazes incrementally (start small, increase size)
- Use the debug console to monitor performance
- Clear previous mazes before generating new ones

## 🔍 Troubleshooting

### Common Issues

**Maze not generating:**
- Check browser console for JavaScript errors
- Ensure coordinates are within valid ranges
- Verify browser supports Canvas API

**Console not hiding:**
- Try refreshing the page
- Check if browser blocks certain CSS properties
- Use browser dev tools to inspect element

**PNG download not working:**
- Ensure Canvas is rendered properly
- Check browser download permissions
- Try right-click → "Save image as"

### Browser-Specific Issues

**Safari:**
- May require additional security permissions
- Canvas export might need user interaction

**Firefox:**
- Older versions may have Canvas performance issues
- Enable hardware acceleration for better performance

## 📞 Support & Feedback

### Getting Help
- **Issues**: Open an issue on GitHub
- **Questions**: Check existing discussions
- **Feature Requests**: Create a feature request issue

### Community
- Share your generated mazes!
- Contribute algorithm improvements
- Help improve documentation

## 🏆 Acknowledgments

### Inspiration
- Classic maze generation algorithms research
- Modern web development best practices
- Educational programming resources

### Technologies
- **Canvas API**: For efficient 2D rendering
- **CSS Grid**: For responsive parameter layout
- **ES6+ JavaScript**: For modern, clean code

## 📜 License

This project is open source and available under the MIT License.

```
MIT License - feel free to use, modify, and distribute
See LICENSE file for full details
```

## 🌟 Star History

If you find this project useful, please consider giving it a star! ⭐

## 🔗 Related Projects

- [Algorithm Visualizer](https://algorithm-visualizer.org/) - Broader algorithm visualization
- [Pathfinding Visualizer](https://clementmihailescu.github.io/Pathfinding-Visualizer/) - Focus on pathfinding
- [Maze Solving Algorithms](https://github.com/topics/maze-solving) - Related repositories

---

**Built with ❤️ for algorithms, education, and beautiful code.**

*Ready to explore the fascinating world of maze algorithms? [Get Started →](https://yourusername.github.io/maze-generator)*
