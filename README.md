# DutyNote
[中文 README](./README-zh_cn.md)

A duty schedule application

> Part of this application was developed with Trae AI assistance. Please ignore if you find it uncomfortable.

> This project is currently in early development phase ~~(planning)~~. Actual features may differ from the roadmap.

## Main Features

- [ ] Duty schedule display and editing
- [ ] Duty schedule export
- [ ] ClassIsland integration (duty monitor display, duty reminders, automation access)
- [ ] LanMountainDesktop integration (weekly duty schedule widget)
- [ ] SecScore integration (duty monitor permissions, labor score adjustments)

## Tech Stack

- Frontend: Vue 3 + TypeScript + Vite
- Backend: Tauri + Rust

## Development & Build

### Development Environment

This project uses npm for dependency management. The following tools are required:

- [VS Code](https://code.visualstudio.com/) + [Vue - Official](https://marketplace.visualstudio.com/items?itemName=Vue.volar) + [Tauri](https://marketplace.visualstudio.com/items?itemName=tauri-apps.tauri-vscode) + [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)
- [gcc](https://gcc.gnu.org/) (Linux) or [MSVC](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022) (Windows)
- [Rust](https://www.rust-lang.org/tools/install) (usually includes cargo automatically)
- [Node.js](https://nodejs.org/) (usually includes npm automatically)

### Development Workflow

1. **Install Dependencies**
```bash
npm install
```

2. **Start Development Server**
```bash
npm run tauri dev
```

3. **Build Production Version**
```bash
npm run tauri build
```

## Project Structure

```
DutyNote/
├── src/                    # Vue frontend source code
│   ├── App.vue            # Main application component
│   ├── main.ts            # Frontend entry point
│   └── style.css          # Global styles
├── src-tauri/             # Tauri/Rust backend
│   ├── src/
│   │   ├── lib.rs        # Library entry (Tauri commands)
│   │   └── main.rs       # Main program entry
│   ├── Cargo.toml        # Rust dependencies
│   └── tauri.conf.json   # Tauri configuration
├── package.json           # Node.js dependencies
└── vite.config.ts         # Vite build configuration
```

## Common Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start frontend dev server |
| `npm run build` | Build frontend for production |
| `npm run tauri dev` | Start full Tauri development environment |
| `npm run tauri build` | Build desktop application installer |

## License

GNU GENERAL PUBLIC LICENSE Version 3
