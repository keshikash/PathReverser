# Line Direction Plugin for QGIS

The **Line Direction** plugin is a QGIS tool designed to manage and visualize the direction of linear features (e.g., fiber optic cables, pipelines, roads) in vector layers. It provides an intuitive interface for selecting, reversing, and saving line directions with real-time visual feedback.


## Overview

This plugin is particularly useful for:
- **Fiber Optic Network Management**
- **Utility Infrastructure Directional Flow**
- **Transportation Network Planning**
- **Hydrological Flow Modeling**


##  Interface Preview

###  Initial View (No Features Selected)
![Image](https://github.com/user-attachments/assets/282aff54-e00a-4ccb-a3d5-c3be21aa900e)

###  After Features Are Selected
![Image](https://github.com/user-attachments/assets/67e931f6-77ac-4759-99bc-0619cebbeef1)


##  Key Features

### Core Functionality
-  **Direction Visualization**: Displays arrows along lines to show current direction.
-  **Interactive Selection**: Choose lines directly on the map or from a list.
-  **Bulk Operations**: Reverse directions for multiple lines simultaneously.
-  **Undo Capabilities**: Reset to original state before saving.
-  **Visual Feedback**: Color-coded indicators show modified vs original directions.

### Technical Capabilities
-  Works with **single-part** and **multi-part** geometries.
-  Preserves all **original attributes** during direction changes.
-  Supports **curved** and **multi-segment** line geometries.
-  Tracks changes for safe and reversible edits.


##  Installation

1. Download or clone this repository.
2. Copy the plugin folder to your QGIS plugins directory:
   - **Linux**: `~/.qgis2/python/plugins/` or `~/.local/share/QGIS/QGIS3/profiles/default/python/plugins/`
   - **Windows**: `%APPDATA%\QGIS\QGIS3\profiles\default\python\plugins\`
3. Launch QGIS and enable the plugin via **Plugin Manager**.


##  Usage Guide

### Basic Workflow
1. **Launch** the plugin via the *Vector* menu or toolbar.
2. **Select Lines**:
   - Interactively on the map with the *Select Lines* tool.
   - Or manually from the feature list.
3. **Modify Directions**:
   - Check desired features and click *Reverse Directions*.
4. **Review Changes**:
   - Arrows update instantly to reflect the new direction.
   - Use *Reset* to undo unsaved changes.
5. **Save or Discard**:
   - Click *Save* to apply the changes.
   - Click *Close* to discard modifications.

### Advanced Tools
-  **Direction Indicators**: Temporary layer with arrows at regular intervals.
-  **Feature Filtering**: Filter by attribute values for precise selection.
-  **Label Integration**: Display cable/feature names during selection.
-  **Change Tracking**: Prompts before exiting unsaved work.


##  Target Use Cases
- **Fiber Optic Cable Networks**
- **Water/Gas Pipeline Management**
- **One-Way Road Systems**
- **Stream Flow in Hydrological Studies**


## Requirements
- QGIS 3.x
- Python 3
- Line vector layers with proper CRS


## Known Limitations
- Optimized for `fiber_cable` layers (but supports all line layers).
- Complex curved lines may show simplified direction arrows.


## Support

For issues, bugs, or feature requests, contact:
b22ee040@iitj.ac.in


## License

This project is licensed under the [MIT License](LICENSE).





