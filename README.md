# calculator-android-ui
A simple Android calculator app built using XML layouts with ripple effects, supporting basic arithmetic operations.

## 🧩 Code Overview

The app is structured using native Android XML for UI and Java/Kotlin for logic. The layout file defines all calculator buttons and display fields using `ConstraintLayout` and nested `LinearLayouts`.

### 🔹 activity_main.xml

Defines the entire UI:
- Two `TextView`s at the top for expression and result
- Five rows of buttons (numbers, operations, and functions)
- Each row uses horizontal `LinearLayout` with `layout_weight` to ensure equal-sized buttons

### 🔹 UI Features
- Ripple effects for number and operation buttons (via `ripple_effect_numbers.xml` and `ripple_effect_operations.xml`)
- Gradient background for the equal (`=`) button via `red_button.xml`
- Responsive design with `weightSum` and `layout_weight`

### 🔹 Drawable Files
- `ripple_effect_numbers.xml`: Custom touch feedback for number keys
- `ripple_effect_operations.xml`: Visual feedback for operators
- `gradient_effect.xml`: Red gradient for the equals button background

### 🔹 Color References
- Uses color resources defined in `colors.xml` like `@color/colorWhite`, `@color/colorGrey`, etc.

### 🔹 Java/Kotlin Code (MainActivity)
- Will handle:
  - Button click listeners
  - String expression building
  - Calculation logic using `eval()` or a custom parser
  - Display updates for both input and result


