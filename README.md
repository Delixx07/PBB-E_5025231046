# 📱 Flutter Demo App

A simple Flutter application demonstrating core widget usage including layout, networking, and state management.

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

| Level | Widget | Notes |
|-------|--------|-------|
| 1 | `MaterialApp` | App root |
| 2 | `Scaffold` | Page frame |
| 3 | `AppBar` | Top bar |
| 4 | `Text` | Title: *"My First App"* |
| 3 | `Column` | Main body |
| 4 | `Container` → `AspectRatio` → `Center` → `Image.network` | Image section |
| 4 | `Container` → `Text` | Description: *"What image is that"* |
| 4 | `Container` → `Row` | Category icon row |
| 5 | `Column` → [`Icon`, `Text`] | Food |
| 5 | `Column` → [`Icon`, `Text`] | Scenery |
| 5 | `Column` → [`Icon`, `Text`] | People |
| 4 | `CounterCard` → `Container` → `Row` | Counter card |
| 5 | `Text` | Dynamic counter display |
| 5 | `Container` → `IconButton` | Increment button (+) |

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
