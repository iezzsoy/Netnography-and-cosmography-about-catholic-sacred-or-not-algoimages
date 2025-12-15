# Sacred Art AI Visualization Project

## Overview

This project consists of two interactive visualizations that explore the process of algorithmization and potential degradation of sacred references through Artificial Intelligence systems. Using Sankey diagrams in D3.js, the project graphically illustrates the transformation flows from traditional sacred sources to AI-generated digital outputs.

## Included Visualizations

### 1. Flow of Algorithmization of Sacred References
**File:** `flow-algorithmization.html`

Demonstrates the positive flow of sacred art digitalization, from its original divine sources to the creation of digital inspiration banks.

**Visualized categories:**
- **Divine Sources**: Canonized saints, iconographic tradition, sacred scriptures
- **Traditional Art**: Renaissance paintings, Baroque sculptures, Byzantine mosaics
- **Technical Processes**: Digitalization, cataloging, iconographic analysis
- **AI Systems**: Databases, recognition algorithms, neural networks
- **Digital Outputs**: Synthetic images, identified patterns, creative suggestions

### 2. Degradation of Sacred Representation in AI
**File:** `degradation-sacred-ai.html`

Presents a critical analysis of common errors and problems that occur when generic algorithms process sacred symbols without proper theological context.

**Visualized categories:**
- **Authentic Sources**: Traditional iconography, historical sacred art
- **Contaminated Datasets**: Fantasy images, commercial art, memes
- **Generic Processing**: Context-less algorithms, blind interpolation
- **Critical Errors**: Swapped symbols, distorted anatomy, inadequate halos
- **Problematic Outputs**: Unrecognizable saints, profane aesthetics, theological confusion

## Technologies Used

- **HTML5**: Page structure
- **CSS3**: Styling and gradients
- **JavaScript (ES6+)**: Interaction logic
- **D3.js v7.8.5**: Data visualization library
- **d3-sankey v0.12.3**: Sankey diagram plugin

## How to Use

### Option 1: Run Locally
1. Download the HTML files
2. Open directly in browser (double-click the file)
3. No local server required (all dependencies loaded via CDN)

### Option 2: Host Online
```bash
# Place files on any web server
# Example with Python:
python -m http.server 8000

# Access in browser:
http://localhost:8000/flow-algorithmization.html
http://localhost:8000/degradation-sacred-ai.html
```

## Interactive Features

- **Informative Tooltip**: Hover over nodes and connections to see details
- **Color Legend**: Quickly identify categories
- **Proportional Flows**: Connection width represents flow volume
- **Responsive Design**: Adapts to different screen sizes

## Data Structure

Each visualization uses a data structure with:
- **Nodes**: Represent process stages
- **Links (Connections)**: Represent flows between stages
- **Values**: Intensity/volume of each connection

Example structure:
```javascript
{
  nodes: [
    { name: "Node Name", category: "category", error: boolean }
  ],
  links: [
    { source: 0, target: 5, value: 15 }
  ]
}
```

## Use Cases

- **Educational**: Teaching about AI and sacred art
- **Academic**: Research on digitalization of cultural heritage
- **Theological**: Discussions about sacred representation in digital media
- **Technical**: Analysis of generative AI systems

## Important Warnings

### Degradation Diagram
The second diagram (`degradation-sacred-ai.html`) contains alerts about common errors:
- Swapped symbols (e.g., St. Peter with St. Paul's keys)
- Incorrect colors in garments
- Distorted anatomy (extra hands, deformed faces)
- Inadequate halos
- Lost contexts

## Customization

### Change Colors
Modify the `colorScale` object:
```javascript
const colorScale = {
  divine: "#FFD700",      // Gold for divine
  traditional: "#8B4513", // Brown for traditional
  // ...
};
```

### Add Nodes/Connections
Edit the `nodes` and `links` arrays:
```javascript
nodes: [
  { name: "New Node", category: "category" }
],
links: [
  { source: source_index, target: target_index, value: intensity }
]
```

### Adjust Layout
Configure Sankey parameters:
```javascript
const sankey = d3.sankey()
  .nodeWidth(15)        // Node width
  .nodePadding(35)      // Spacing between nodes
  .extent([[1, 1], [width - 1, height - 6]]);
```

## Compatibility

- Chrome/Edge (v90+)
- Firefox (v88+)
- Safari (v14+)
- Opera (v76+)
- IE11 (not supported)

## License

Educational visualization project. Feel free to use and modify for academic and educational purposes.

## Contributions

Improvement suggestions are welcome:
- New relevant nodes and connections
- Color palette improvements
- Performance optimizations
- Translations to other languages

---

**Last updated:** December 2025  
**Version:** 1.0  
**Author:** Sacred Art and AI Visualization Project
