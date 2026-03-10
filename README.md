# Task 2 web-programming

---

## 🧩 Widget Overview

### App-level Widgets

| Widget | Description |
|--------|-------------|
| `MaterialApp` | Root of the application; configures theme and entry page |
| `ThemeData` | Defines global theme using `ColorScheme.fromSeed` with Material 3 |
| `Scaffold` | Provides the page skeleton with `appBar` and `body` |

---

### Layout Widgets

| Widget | Description |
|--------|-------------|
| `Column` | Arranges children **vertically** |
| `Row` | Arranges children **horizontally** |
| `Container` | Multi-purpose widget for padding, margin, size, and background color |
| `AspectRatio` | Forces child to maintain a fixed aspect ratio (`1:1`) |
| `Center` | Centers its child within the available space |

---

### Content & Display Widgets

| Widget | Description |
|--------|-------------|
| `AppBar` | Top navigation bar with title and background color |
| `Text` | Displays static or dynamic text |
| `TextStyle` | Configures font size, weight, and color for `Text` |
| `Image.network` | Loads and displays an image from a URL |
| `Icon` | Displays a Material Design icon |
| `IconButton` | Interactive button displayed as an icon |

---

### Utility Widgets

| Widget | Description |
|--------|-------------|
| `MediaQuery` | Retrieves device screen dimensions for responsive layout |

---

## 🔄 State Management

| Component | Type | Description |
|-----------|------|-------------|
| `CounterCard` | `StatefulWidget` | Custom widget that holds a mutable counter state |
| `_counter` | `int` | State variable, initialized to `0` |
| `setState()` | Method | Triggers UI rebuild when `_counter` is incremented |

---

## 🗂️ Widget Hierarchy

```
MyApp (StatelessWidget)
└── MaterialApp
    └── RowColumnPage (StatelessWidget)
        └── Scaffold
            ├── AppBar
            │   └── Text ('My First App')
            │       └── TextStyle (color: black)
            │
            └── Column
                ├── Container
                │   └── AspectRatio (ratio: 1.0)
                │       └── Container (color: lightBlue[100])
                │           └── Center
                │               └── Image.network
                │
                ├── Container (color: pink[200])
                │   └── Text ('What image is that')
                │       └── TextStyle (fontSize: 16)
                │
                ├── Container (color: yellow[200])
                │   └── Row
                │       ├── Column
                │       │   ├── Icon (Icons.food_bank)
                │       │   └── Text ('Food')
                │       ├── Column
                │       │   ├── Icon (Icons.landscape)
                │       │   └── Text ('Scenery')
                │       └── Column
                │           ├── Icon (Icons.people)
                │           └── Text ('People')
                │
                └── CounterCard (StatefulWidget)
                    └── Container (color: cyan[100])
                        └── Row
                            ├── Text ('Counter here: $_counter')
                            │   └── TextStyle (fontSize: 16)
                            └── Container (color: cyan[200])
                                └── IconButton (Icons.add)
```

---

## 🚀 Getting Started

```bash
flutter pub get
flutter run
```

## 📋 Requirements

| Tool | Version |
|------|---------|
| Flutter | ≥ 3.0.0 |
| Dart | ≥ 3.0.0 |
| Android SDK / Windows | Latest |
