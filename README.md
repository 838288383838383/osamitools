# CatDot - A Modern Game Engine

CatDot is a modern, beginner-friendly game engine built with .NET. It's designed to be fast, lightweight, and easy to use - unlike Godot, it doesn't suck!

## Features

- **Multi-Language Support**: Write scripts in C#, Python, Gleam, Nim, and more
- **MCP Integration**: Model Context Protocol support for AI-assisted development
- **Beginner Friendly**: Simple API and visual editor
- **Fast & Lightweight**: Optimized for old laptops and PCs
- **Cross-Platform**: Export to Windows, Linux, macOS, and Web

## Project Structure

```
CatDot/
├── src/
│   ├── CatDot.Core/          # Core engine functionality
│   ├── CatDot.Rendering/     # OpenGL/Vulkan rendering
│   ├── CatDot.ECS/           # Entity Component System
│   ├── CatDot.Scene/         # Scene management
│   ├── CatDot.Scripting/     # Scripting engine
│   ├── CatDot.Scripting.Python/  # Python support
│   ├── CatDot.Scripting.Gleam/   # Gleam support
│   ├── CatDot.Scripting.Nim/     # Nim support
│   ├── CatDot.MCP/           # Model Context Protocol
│   └── CatDot.Editor/        # Visual editor
├── tools/
│   └── CatDot.CLI/           # Command line interface
├── templates/                # Project templates
└── CatDot.sln               # Solution file
```

## Getting Started

### Prerequisites

- .NET 9.0 SDK
- Visual Studio 2022 or VS Code

### Building

```bash
dotnet build CatDot.sln
```

### Running the Editor

```bash
dotnet run --project src/CatDot.Editor
```

### Creating a New Project

```bash
dotnet run --project tools/CatDot.CLI -- create MyGame
```

## Language Support

### C# (Primary)
Full support with access to all engine APIs.

### Python
Write game logic in Python with CatDot bindings.

### Gleam
Functional programming with Gleam language support.

### Nim
Systems programming with Nim language support.

## MCP Integration

CatDot includes built-in MCP (Model Context Protocol) support for AI-assisted development:

```csharp
var mcpServer = new MCPServer();
mcpServer.RegisterTool(new MCPTool
{
    Name = "create_entity",
    Description = "Create a new entity",
    Handler = async (args) => { /* ... */ }
});
```

## License

MIT License
