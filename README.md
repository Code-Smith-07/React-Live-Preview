# ⚛️ React Live Preview

<div align="center">

![React Live Preview](https://img.shields.io/badge/React-Live%20Preview-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![License MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)
![License Apache](https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=for-the-badge)
![Made with Love](https://img.shields.io/badge/Made%20with-❤️-red.svg?style=for-the-badge)

**A stunning, glassmorphic React code editor with instant live preview**

[Demo](#-demo) • [Features](#-features) • [Getting Started](#-getting-started) • [Usage](#-usage) • [Contributing](#-contributing)

</div>

---

## 🎨 About

React Live Preview is a beautiful, modern in-browser code editor that lets you write React code and see the results instantly. Built with a stunning glassmorphic UI, powered by CodeMirror 5, and featuring live JSX compilation with Babel - all in a single HTML file.

Perfect for:
- 🎓 Learning React concepts
- 🚀 Quick prototyping and experimentation
- 📝 Creating live coding demos
- 🎨 Testing React components on the fly
- 🔧 No build tools or setup required!

## ✨ Features

### 🎯 Core Features
- **⚡ Instant Live Preview** - See your React code execute in real-time
- **🎨 Glassmorphic UI** - Beautiful, modern design with blur effects
- **💻 Syntax Highlighting** - Powered by CodeMirror with Dracula theme
- **📱 Responsive Design** - Works seamlessly on desktop and mobile
- **🔄 Auto-Compilation** - Babel transforms JSX on the fly
- **🌙 Dark Mode** - Eye-friendly dark interface

### 🛠️ Editor Features
- Line numbers and syntax highlighting
- Auto-closing brackets
- JSX/ES6+ support
- Clean, distraction-free interface
- Mac-like window controls
- Status indicators

### 🎭 UI Features
- Stunning animated background
- Glassmorphism effects throughout
- Smooth transitions and animations
- Professional typography (Inter + JetBrains Mono)
- Visual feedback for active state

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection (for CDN resources)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Code-Smith-07/React-Live-Preview.git
   ```

2. **Navigate to the project**
   ```bash
   cd React-Live-Preview
   ```

3. **Open in browser**
   ```bash
   # Simply open index.html in your browser
   open index.html  # macOS
   start index.html # Windows
   xdg-open index.html # Linux
   ```

That's it! No npm install, no build process, no configuration files. Just pure simplicity. 🎉

## 💡 Usage

### Basic Example

The editor comes with a starter template. Try this code:

```jsx
function App() {
  const [count, setCount] = React.useState(0);
  
  return (
    <div style={{ textAlign: 'center', padding: '50px' }}>
      <h1>Hello React! 🎉</h1>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}

ReactDOM.render(<App />, document.getElementById('root'));
```

### Advanced Features

Try more complex React features:

```jsx
function TodoApp() {
  const [todos, setTodos] = React.useState([]);
  const [input, setInput] = React.useState('');
  
  const addTodo = () => {
    if (input.trim()) {
      setTodos([...todos, { id: Date.now(), text: input }]);
      setInput('');
    }
  };
  
  return (
    <div style={{ maxWidth: '400px', margin: '0 auto', padding: '20px' }}>
      <h2>Todo List</h2>
      <input 
        value={input}
        onChange={(e) => setInput(e.target.value)}
        onKeyPress={(e) => e.key === 'Enter' && addTodo()}
        placeholder="Add a todo..."
        style={{ width: '100%', padding: '10px', marginBottom: '10px' }}
      />
      <button onClick={addTodo} style={{ padding: '10px 20px' }}>
        Add Todo
      </button>
      <ul style={{ listStyle: 'none', padding: 0 }}>
        {todos.map(todo => (
          <li key={todo.id} style={{ padding: '10px', background: '#f0f0f0', margin: '5px 0', borderRadius: '5px', color: '#000' }}>
            {todo.text}
          </li>
        ))}
      </ul>
    </div>
  );
}

ReactDOM.render(<TodoApp />, document.getElementById('root'));
```

## 🏗️ Built With

- **[React 18](https://react.dev/)** - JavaScript library for building user interfaces
- **[CodeMirror 5](https://codemirror.net/5/)** - Versatile text editor implemented in JavaScript
- **[Babel Standalone](https://babeljs.io/docs/babel-standalone)** - Browser-based JavaScript compiler
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework
- **[Google Fonts](https://fonts.google.com/)** - Inter & JetBrains Mono typography

## 🎯 Roadmap

- [ ] Multiple file support
- [ ] Theme customization
- [ ] Export/Import code snippets
- [ ] Dark/Light mode toggle
- [ ] Code sharing functionality
- [ ] TypeScript support
- [ ] Console output panel
- [ ] Error boundary display
- [ ] Auto-save to localStorage
- [ ] Keyboard shortcuts panel

## 🤝 Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## 📄 License

This project is dual-licensed under:

- **MIT License** - See [LICENSE-MIT](LICENSE-MIT) for details
- **Apache License 2.0** - See [LICENSE-APACHE](LICENSE-APACHE) for details

You may choose either license to govern your use of this project.

## 👨‍💻 Author

**Code-Smith-07**
- GitHub: [@Code-Smith-07](https://github.com/Code-Smith-07)

## 🌟 Show Your Support

If you found this project helpful, please give it a ⭐️! It helps others discover it too.

## 📝 Acknowledgments

- Inspired by CodePen, JSFiddle, and other online code editors
- Thanks to the React and CodeMirror communities
- Special thanks to all contributors

## 📧 Contact

Have questions or suggestions? Feel free to:
- Open an issue
- Start a discussion
- Reach out on GitHub

---

<div align="center">

**Made with ❤️ by Code-Smith-07**

If you like this project, consider buying me a coffee! ☕

</div>
