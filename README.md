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
- 🔄 **Input Switch** - Toggle switch components
- 📊 **Table** - Data table with sorting and filtering
- 🔔 **Notifications** - Toast and notification system
- 💬 **Dialog** - Modal dialogs and popups
- 🎨 **Chips** - Tag and chip components
- 📑 **Tabs** - Tabbed navigation
- 📋 **Accordion** - Collapsible content sections
- 🍔 **Cascade Menu** - Hierarchical dropdown menu
- 📊 **Menubar** - Horizontal navigation menu with dropdowns
- ⏱️ **Timeline** - Timeline visualization
- 📄 **Paginator** - Pagination controls
- 🔍 **Autocomplete** - Search with suggestions
- 🔘 **Radio** - Radio button groups
- 🎯 **Multi-select** - Multiple selection dropdown
- 🌐 **Sidebar** - Navigation sidebar
- 💀 **Skeleton** - Loading placeholder
- ⚡ **Spinner** - Loading indicators
- ⚙️ **Preload** - Content preloading
- 💡 **Tooltip** - Contextual tooltips
- 🔐 **InputOTP** - One-Time Password verification 

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

| Script | Description |
|--------|-------------|
| `npm start` | Start development server |
| `npm run build` | Build for production |
| `npm run watch` | Build in watch mode |
| `npm test` | Run unit tests |

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
import { Component } from '@angular/core';
import { MsDropdown } from 'maxi-angular-components';

@Component({
  selector: 'app-example',
  standalone: true,
  imports: [MsDropdown],
  template: `
    <ms-dropdown
      [options]="options"
      [(value)]="selectedValue"
      (onSelect)="handleSelection($event)">
    </ms-dropdown>
  `
})
export class ExampleComponent {
  options = [
    { label: 'Option 1', value: '1' },
    { label: 'Option 2', value: '2' }
  ];
  
  selectedValue = null;
  
  handleSelection(event: any) {
    console.log('Selected:', event.detail);
  }
}
```

## 🔧 Dependencies

### Main Dependencies
- **@angular/core**: ^18.2.0
- **maxi-angular-components**: ^4.0.13
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
  Made with ❤️ using Angular and Maxi Web Components
</div>

