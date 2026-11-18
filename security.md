# UML Class Diagram Generator

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0F0C29,100:302B63&height=220&section=header&text=Uml%20Class%20Diagram%20Generator&fontSize=55&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Turn%20Your%20Code%20Into%20Beautiful%20Visual%20Architecture&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-3.1.0-302B63?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-98.1K-0F0C29?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-FFD700?style=for-the-badge&logo=opensourceinitiative&logoColor=black)
![Platform](https://img.shields.io/badge/platform-web%20%7C%20cli%20%7C%20vscode-00C9FF?style=for-the-badge&logo=visualstudiocode&logoColor=white)

</div>

---

## 🏛️ Architecture Made Visible

Every great software project starts with a solid architecture. But as the codebase grows, the mental model of the system becomes clouded. New developers struggle to understand how classes relate to each other. Legacy code becomes a "big ball of mud."

**UML Class Diagram Generator** is a powerful, open-source tool that automatically generates Unified Modeling Language (UML) class diagrams from your source code. It parses your files, extracts the classes, interfaces, methods, and relationships, and renders a stunning, interactive diagram.

This is not just a static image generator. It is a living documentation tool. You can embed it in your CI/CD pipeline to generate diagrams on every commit. It supports Java, Python, TypeScript, C#, and Go. It includes a sleek web interface, a command-line interface for automation, and a VS Code extension for real-time previews. It is the ultimate tool for software architects and tech leads.

---

## 🗺️ The Three Layers Of The Generator

We have designed the tool to fit into every stage of your development workflow.

| Layer | Description | Technology |
| :--- | :--- | :--- |
| **Parser** | Extracts classes, methods, and relationships from source code | Tree-sitter, AST |
| **Renderer** | Converts the parsed data into a visual diagram | Mermaid.js, D3.js |
| **Exporter** | Saves the diagram as SVG, PNG, or PlantUML text | Puppeteer, SVG |

<img width="1280" height="720" alt="online-class-diagram-2" src="https://github.com/user-attachments/assets/6bb2f83f-6283-48ce-a46c-5ed54670c8be" />

---

## ✨ Core Features & Capabilities

| Feature | Description |
| :--- | :--- |
| **Multi-Language Support** | Java, Python, TypeScript, C#, Go, and more |
| **Interactive Diagrams** | Zoom, pan, and click on classes to see details |
| **Relationship Detection** | Automatically detects inheritance, composition, and aggregation |
| **Dark Mode UI** | A stunning, eye-friendly interface for late-night architecture reviews |
| **CI/CD Integration** | Generate diagrams automatically on every pull request |
| **Export Options** | Save as SVG, PNG, PDF, or PlantUML text |

---

<div align="center">

### 🔗 Ready to visualize your code?

[![Get Tool](https://img.shields.io/badge/🏛️_GET_TOOL-0F0C29?style=for-the-badge&logoColor=white)](https://share.google/XiwQglrjy8cmSwjM4)

</div>

---

## ⚙️ Quick Setup

You can install the CLI via npm or use the VS Code extension directly.

```bash
# Step 1: Install the CLI globally
npm install -g uml-generator

# Step 2: Run the generator on your project
uml-gen --input ./src --output ./diagrams

# Step 3: Open the generated SVG in your browser
open ./diagrams/class-diagram.svg
```

Once the command finishes, you will find a beautifully rendered UML diagram in the `diagrams/` folder. The diagram uses color coding to distinguish between interfaces, abstract classes, and concrete classes.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-302B63?style=for-the-badge&logoColor=white)](https://share.google/XiwQglrjy8cmSwjM4)

</div>

---

## 🧠 Under The Hood: The AST Parser

How does the tool understand your code? It doesn't just use regular expressions. It uses a technique called **Abstract Syntax Tree (AST) Parsing**.

When you feed a Python file to the tool, it uses the `tree-sitter` library to parse the code. `tree-sitter` is a highly optimized parser that can handle incomplete or syntactically incorrect code. It generates a tree structure representing the code.

The tool walks through this tree. When it finds a `class_definition` node, it creates a new Class object. When it finds a `function_definition` inside a class, it adds it as a method. When it finds an `argument_list` or an `extends_clause`, it adds a relationship. The result is a pure, structured representation of your codebase.

---

## 🛠️ Tech Stack

<div align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Tree-sitter](https://img.shields.io/badge/Tree--sitter-00C9FF?style=flat-square&logo=tree&logoColor=black)
![Mermaid](https://img.shields.io/badge/Mermaid-FF3670?style=flat-square&logo=mermaid&logoColor=white)
![D3.js](https://img.shields.io/badge/D3.js-F9A03C?style=flat-square&logo=d3dotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

## 🤝 Community & Contributing

We believe that good architecture should be visible to everyone. If you have added support for a new language, improved the layout algorithm, or found a bug in the parser, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-language`).
3. **Commit** your changes (`git commit -m 'Add new language'`).
4. **Push** to the branch (`git push origin feature/new-language`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your diagrams, ask for help with parser configuration, and discuss the latest trends in software architecture.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@uml-generator.dev.

---

<div align="center">

### ⭐ If this tool clarifies your codebase, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-FFD700?style=for-the-badge&logo=github&logoColor=black)](https://github.com/your-username/uml-class-diagram-generator)

---

### 🚀 Start visualizing today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-00C9FF?style=for-the-badge&logoColor=white)](https://share.google/XiwQglrjy8cmSwjM4)

<sub>Crafted with precision and ❤️ by the UML Class Diagram Generator community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:302B63,100:0F0C29&height=120&section=footer)

</div>
