# Java Paint App (Spring GUI)

A simple Java-based paint application that allows users to draw geometric shapes such as points, lines, circles, donuts, and rectangles. Users can interact with the shapes via GUI dialogs and manipulate them using sort and stack operations.
This is one of my early Java projects focused on building a hands-on understanding of object-oriented design and GUI development. All shape behaviors (like drawing, moving, comparing, etc.) are abstracted through a flexible class hierarchy.

This project was created as a personal practice and learning project using Java and Swing.

---

## Features

- Draw and manipulate geometric shapes (Point, Line, Circle, Donut, Rectangle)
- GUI dialogs for shape input (e.g., `DlgCircle`, `DlgRectangle`)
- Sorting functionality for drawn shapes
- Undo/Redo operations using a custom stack implementation
- Intuitive drawing interface (`FrmDrawing`, `PnlDrawing`)

  ## • Technologies Used

- Java
- Swing (AWT & Swing components)
- Object-Oriented Programming

## Components

### `geometry/`
Contains all shape definitions and behavior:
- `Circle`, `Donut`, `Line`, `Rectangle`, `Point`
- Abstract base classes/interfaces: `Shape`, `SurfaceShape`, `Moveable`

### `drawing/`
Main application interface:
- `FrmDrawing`: main window
- `PnlDrawing`: drawing area (custom JPanel)
- `Dlg<Shape>` dialogs: input dialogs for creating/editing shapes

### `sort/`
GUI for sorting:
- `FrmSort`: sorting window
- `DlgSort`: confirmation/input dialog for sort settings

### `stack/`
Manages undo/redo functionality using stacks:
- Stores command objects or snapshots to revert/redo actions
