<div align="center">
  <img src="./public/assets/logo.png" alt="Maxi Web Components Logo" width="400"/>

# Maxi Angular Components Test

![Angular](https://img.shields.io/badge/Angular-18.2.0-red)
![TypeScript](https://img.shields.io/badge/TypeScript-5.5.2-blue)
![License](https://img.shields.io/badge/license-Private-lightgrey)

</div>

## 📖 Overview

This is a test and demonstration project for **Maxi Angular Components** library. It showcases various UI components built with Angular 18 and provides examples of how to integrate and use them in your applications.

## ✨ Features

- **Modern UI Components**: Pre-built, customizable components
- **Angular 18**: Latest Angular version with standalone components
- **TypeScript**: Type-safe development experience
- **Responsive Design**: Mobile-first approach
- **Easy Integration**: Simple import and usage

## 📦 Available Components

The project includes examples of the following components:

- 🔽 **Dropdown** - Select components with customizable options
- 🔘 **Button** - Interactive button elements
- 🎴 **Card** - Container components for content organization
- 📅 **Calendar** - Date picker and calendar widgets
- ☑️ **Checkbox** - Checkbox input components
- 🎯 **Badge** - Status and notification badges
- 🔤 **Input Field** - Text input components
- 🔢 **Input Number** - Numeric input with controls
- 🔢 **Control Number** - Numeric control input for managing numeric values
- 🔄 **Input Switch** - Toggle switch components
- 📊 **Table** - Data table with sorting and filtering
- 🔔 **Notifications** - Toast and notification system
- 💬 **Dialog** - Modal dialogs and popups
- 📨 **Messages** - Contextual messages for displaying different types of feedback with multiple variants
- 🎨 **Chips** - Tag and chip components
- 📑 **Tabs** - Tabbed navigation
- 📋 **Accordion** - Collapsible content sections
- 🍔 **Cascade Menu** - Hierarchical dropdown menu
- 📊 **Menubar** - Horizontal navigation menu with dropdowns
- 🍞 **Breadcrumb** - Navigation breadcrumb trail showing current page location
- 🪜 **Steps** - Step-by-step navigation component - Click on each step to navigate
- ⏱️ **Timeline** - Timeline visualization
- 📄 **Paginator** - Pagination controls
- 🔍 **Autocomplete** - Search with suggestions
- 🔘 **Radio** - Radio button groups
- 🎯 **Multi-select** - Multiple selection dropdown
- 🌐 **Sidebar** - Navigation sidebar
- 💀 **Skeleton** - Loading placeholder
- ⚡ **Spinner** - Loading indicators
- ⚙️ **Preload** - Content preloading
- 📊 **Progress Bar** - Progress indicator for showing completion status or loading state
- 💡 **Tooltip** - Contextual tooltips
- 🎠 **Carousel** - Interactive carousel for displaying multiple items with navigation
- 📦 **Fieldset** - Grouped form fields with collapsible legend for organizing related inputs
- 📊 **Meter Group** - Visualize categorized data in a segmented bar
- 🖼️ **Image** - Advanced image component with preview mode (light box)
- 💬 **Popover** - Contextual popup triggered by click, hover, or focus
- ✍️ **Text Editor** - Rich text editor with formatting toolbar
- 🎛️ **Knob** - Circular dial control for selecting numeric values
- 🔑 **Input Password** - Password input with strength indicator and mask toggling
- 🔘 **Select Button** - Button-based selection component
- 📊 **Chart** - Interactive charts (bar, line, pie, doughnut, radar, bubble, polar area, scatter, stacked, mixed) with animation support
- 🔣 **Icon** - Scalable SVG icons with size and color customization

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Angular CLI

### Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd maxi-angular-components-test
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm start
```

4. Open your browser and navigate to:

```
http://localhost:4200
```

## 🛠️ Available Scripts

| Script          | Description              |
| --------------- | ------------------------ |
| `npm start`     | Start development server |
| `npm run build` | Build for production     |
| `npm run watch` | Build in watch mode      |
| `npm test`      | Run unit tests           |

## 🏗️ Project Structure

```
maxi-angular-components-test/
├── src/
│   ├── app/
│   │   ├── components/
│   │   │   └── maxi/          # Component examples
│   │   ├── app.component.ts   # Root component
│   │   └── app.routes.ts      # Application routes
│   ├── assets/                # Static assets
│   └── styles.scss            # Global styles
├── public/                    # Public assets
└── package.json              # Dependencies
```

## 📚 Component Usage Example

```typescript
import { Component } from "@angular/core";
import { MsDropdown } from "maxi-angular-components";

@Component({
  selector: "app-example",
  standalone: true,
  imports: [MsDropdown],
  template: ` <ms-dropdown [options]="options" [(value)]="selectedValue" (onSelect)="handleSelection($event)"> </ms-dropdown> `,
})
export class ExampleComponent {
  options = [
    { label: "Option 1", value: "1" },
    { label: "Option 2", value: "2" },
  ];

  selectedValue = null;

  handleSelection(event: any) {
    console.log("Selected:", event.detail);
  }
}
```

## 📚 Detailed Component Documentation

---

### 📊 MsMeterGroup

Component for visualizing categorized data in a segmented bar.

#### Props

- `values`: `MeterValue[]` - Array of objects with `label`, `value`, `color`, `icon`.
- `orientation`: `'horizontal' | 'vertical'` (default: `'horizontal'`).

---

### 🖼️ MsImage

Advanced image component with preview (light box) functionality.

#### Props

- `src`: `string` (required) - Image URL.
- `alt`: `string` (required) - Alt text.
- `preview`: `boolean` (default: `false`) - Enables light box.

---

### 💬 MsPopover

Contextual popup component.

#### Props

- `trigger`: `'click' | 'hover' | 'focus'` (default: `'click'`).
- `placement`: `'top' | 'bottom' | 'left' | 'right'` (default: `'bottom'`).

---

### ✍️ MsTextEditor

Rich text editor with formatting toolbar.

#### Props

- `placeholder`: `string`.
- `readonly`: `boolean` (default: `false`).

#### Events

- `textChange`: Emits the HTML string on content change.

---

### 🎛️ MsKnob

Circular dial control for selecting numeric values.

#### Props

- `value`: `number`.
- `min`: `number` (default: `0`).
- `max`: `number` (default: `100`).

---

### 🔑 MsInputPassword

Password input with strength meter.

#### Props

- `label`: `string`.
- `feedback`: `boolean` (default: `false`) - Shows strength indicator.
- `toggleMask`: `boolean` (default: `false`) - Shows eye icon.

---

### 🔘 MsSelectButton

Button-based selection.

#### Props

- `options`: `string[] | Item[]`.
- `multiple`: `boolean` (default: `false`).

---

### 📊 MsChart

Interactive chart component powered by Chart.js.

#### Props

- `type`: `'bar' | 'line' | 'pie' | 'doughnut' | 'radar' | 'bubble' | 'polarArea' | 'scatter'` - Chart type.
- `data`: `object` - Chart.js data object with `labels` and `datasets`.
- `options`: `object` - Chart.js options object (supports animations, scales, plugins, etc.).
- `variant`: `'primary' | 'secondary' | 'success' | 'warning' | 'info' | 'mixed'` - Color palette.
- `height`: `string` (e.g. `'280px'`) - Chart height.
- `width`: `string` - Chart width.

#### Events

- `chartReady`: Emits when the chart is initialized.
- `chartClick`: Emits `ChartClickEvent` when a chart element is clicked.

---

### 🔣 MsIcon

Scalable SVG icon component.

#### Props

- `name`: `string` - Icon identifier (e.g. `'home'`, `'search'`, `'bell'`).
- `size`: `number` (default: `24`) - Icon size in pixels.
- `color`: `string` - Icon color (CSS color value).
- `customClass`: `string` - Additional CSS class.

### Main Dependencies

- **@angular/core**: ^18.2.0
- **maxi-angular-components**: ^7.0.2
- **rxjs**: ~7.8.0

### Dev Dependencies

- **@angular/cli**: ^18.2.10
- **typescript**: ~5.5.2

## 📝 License

This project is private and for testing purposes only.

## 🤝 Contributing

This is a test project. For contributions to the main library, please refer to the `maxi-angular-components` repository.

---

<div align="center">
  Made with ❤️ using Angular and Maxi Angular Components
</div>
