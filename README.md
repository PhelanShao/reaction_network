# ReacNet Analyzer Pro

[![Version](https://img.shields.io/badge/version-2.0-blue.svg)](https://github.com/PhelanShao/reaction_network)
[![License](https://img.shields.io/badge/license-Citation%20Required-orange.svg)](#citation)
[![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)](#system-requirements)

> **A powerful tool for visualizing and analyzing reaction networks from computational chemistry data**

## 🎯 Overview

ReacNet Analyzer Pro is a comprehensive software solution designed for computational chemists and researchers to visualize, analyze, and interpret complex reaction networks. Built with modern GUI frameworks and equipped with advanced molecular rendering capabilities, it transforms raw reaction data into interactive, publication-ready visualizations.

### ✨ Key Features

- **🔬 Advanced Molecular Visualization**: High-quality 3D and 2D molecular structure rendering
- **🌐 Interactive Network Analysis**: Dynamic reaction pathway visualization with energy profiles
- **📊 Multiple Export Formats**: Publication-ready PNG and SVG outputs
- **🔐 Secure Data Handling**: Encrypted file processing with authentication
- **🎨 Modern Interface**: Intuitive drag-and-drop GUI with real-time progress tracking
- **⚡ High Performance**: Optimized for large-scale reaction networks

## 📦 Installation & Quick Start

### Option 1: Standalone Executable (Recommended)

1. **Download**: Get `ReacNetAnalyzer_Pro.exe` (~500MB)
2. **Launch**: Double-click the executable
3. **Authenticate**: Enter password: `github.com/PhelanShao/reaction_network`
4. **Start Analysis**: Load your `.reacnet` file and begin!

### Option 2: Python Source

```bash
# Clone or download the source code
cd reacnet_analyzer
python modern_secure_gui_english.py
```

**Dependencies Required:**
```bash
pip install numpy scipy matplotlib networkx rdkit-pypi pillow cryptography
```

## 🚀 Usage Guide

### Step 1: Authentication
- Launch the application
- Enter the required password when prompted
- Review citation requirements

### Step 2: File Selection
- **Browse**: Use the "Browse Files" button to select your input file(*.reacnet)
- **Supported Formats**: `.reacnet` encrypted reaction network files

### Step 3: Configuration
| Setting | Options | Description |
|---------|---------|-------------|
| **Render Mode** | `3D`, `2D`, `Both` | Choose visualization style |
| **Output Format** | `PNG`, `SVG` | Select image format |
| **Output Directory** | Custom path | Specify where results are saved |

### Step 4: Processing
1. Click **"Start Processing"**
2. Monitor progress in real-time
3. View detailed status updates
4. Wait for completion notification

### Step 5: Results
- **Interactive HTML**: Browse the generated reaction network
- **Molecular Images**: High-quality 3D/2D structure visualizations
- **Energy Profiles**: MEP analysis and pathway energetics
- **Network Data**: Topology and connectivity information

## 🔧 Advanced Configuration

### Custom Settings

```python
# Example configuration options
settings = {
    "render_mode": "3d",        # 3d, 2d, both
    "output_format": "svg",     # png, svg
    "image_quality": "high",    # low, medium, high
    "energy_analysis": True,    # Include MEP data
    "filter_ts": True          # Filter transition states
}
```

## 📊 File Formats & Data Structures

### Input Formats

**Primary Input:**
- `.reacnet` - Encrypted reaction network files containing:
  - Molecular coordinates (XYZ format)
  - Reaction connectivity data
  - Energy information
  - Metadata and parameters

**Auxiliary Data:**
- `orca_MEP.xyz` - ORCA minimum energy path trajectories
- Individual `.xyz` files - Molecular coordinate files

### Output Structure

```
output_directory/
├── reaction_network.html          # Interactive visualization
├── molecule_images/               # Individual structure images
│   ├── node_001_3d.svg          # 3D molecular structures
│   └── node_002_2d.png          # 2D chemical diagrams
├── energy_profiles/              # MEP analysis
└── network_data.json            # Raw network topology
```

## 🛠️ System Requirements

### Minimum Requirements
- **OS**: Windows 10 (64-bit)
- **RAM**: 4GB
- **Storage**: 1GB free space
- **Graphics**: OpenGL 2.0 support

### Recommended Specifications
- **OS**: Windows 11 (64-bit)
- **RAM**: 8GB or more
- **Storage**: SSD with 2GB+ free space
- **Graphics**: Dedicated GPU with 1GB VRAM
- **CPU**: Multi-core processor (Intel i5/AMD Ryzen 5 or better)

### Software Dependencies (for Python version)
- Python 3.8+
- NumPy ≥ 1.19
- SciPy ≥ 1.5
- Matplotlib ≥ 3.3
- NetworkX ≥ 2.5
- RDKit ≥ 2020.09 (optional, for 2D rendering)
- Pillow ≥ 8.0
- Cryptography ≥ 3.0

## 📚 Citation Requirements

### Primary Citation
When using ReacNet Analyzer in your research, please cite:

```bibtex
@article{ReacNetAnalyzer2024,
  title={ReacNet Analyzer: Advanced Reaction Network Visualization Tool},
  author={[Author Names]},
  journal={[Journal Name]},
  year={2024},
  volume={[Volume]},
  pages={[Pages]},
  doi={[DOI]}
}
```

### Additional References
Please also cite the underlying methodologies and tools:
- **RDKit**: For 2D molecular visualization
- **NetworkX**: For graph analysis algorithms
- **Matplotlib**: For plotting and rendering
- **Original ReacNet methodology**: [Original paper citations]

**Problem**: Large files cause memory errors
```
Solution:
1. Increase system RAM
2. Close other applications
3. Process smaller subsets
4. Use 64-bit Python version
```

### Performance Optimization

**For Large Networks:**
- Use PNG format for faster processing
- Disable 2D rendering if not needed
- Process in smaller batches
- Ensure sufficient disk space

**For High Quality Output:**
- Use SVG format for publications
- Enable both 3D and 2D rendering
- Increase image resolution settings
- Verify font availability

---

*For the latest updates and downloads, visit: [Project Repository](https://github.com/PhelanShao/reaction_network)* 
