# 📝 Notes App

A simple and elegant note-taking application built with React and Tailwind CSS. Create, view, and delete notes with a beautiful sticky note interface.

## ✨ Features

- **Add Notes** - Create notes with a heading and detailed description
- **Delete Notes** - Remove notes with a single click
- **Beautiful UI** - Sticky note design with dark theme
- **Responsive Design** - Works seamlessly on desktop and mobile devices
- **Real-time Updates** - See your notes instantly as you add or delete them
- **Tailwind CSS** - Modern styling with utility-first CSS framework

## 🛠️ Tech Stack

- **Frontend Framework:** React 19
- **Build Tool:** Vite
- **Styling:** Tailwind CSS 4.3
- **Package Manager:** npm

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v16 or higher)
- npm (comes with Node.js)

## 🚀 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/notes-app.git
   cd notes-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```
   The app will automatically open in your default browser at `http://localhost:5173`

## 📖 Usage

1. **Add a Note:**
   - Enter a heading in the "Enter Notes Heading" input
   - Write details in the "Write Details here" textarea
   - Click the "Add Note" button
   - Your note appears as a sticky note on the right side

2. **Delete a Note:**
   - Click the red "Delete" button on any sticky note
   - The note is immediately removed

## 📁 Project Structure

```
Notes_App/
├── src/
│   ├── App.jsx          # Main component with all logic
│   ├── index.css        # Global styles with Tailwind import
│   └── main.jsx         # React entry point
├── index.html           # HTML template
├── vite.config.js       # Vite configuration
├── package.json         # Project dependencies
└── README.md           # This file
```

## 🔧 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server (opens in browser) |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint to check code quality |

## 💡 How It Works

### State Management
The app uses React's `useState` hook to manage:
- `title` - Current note heading input
- `details` - Current note description input
- `task` - Array of all created notes

### Key Functions
- **`submitHandler`** - Adds a new note to the task array
- **`deleteNote`** - Removes a note by its index

### Data Flow
```
User Input → State Update → Component Re-render → Display Notes
```

## 🎨 Customization

### Change Colors
Edit the Tailwind classes in `src/App.jsx`:
- `bg-black` - Background color
- `bg-red-500` - Delete button color

### Modify Sticky Note Image
Replace the background image URL in the note card:
```jsx
bg-[url('YOUR_NEW_IMAGE_URL')]
```

## 📦 Build for Production

```bash
npm run build
```

This creates an optimized production build in the `dist/` folder.

## 🐛 Troubleshooting

**Notes not appearing?**
- Check browser console for errors
- Ensure `npm run dev` is running
- Clear browser cache and refresh

**Styles not loading?**
- Verify Tailwind CSS is imported in `src/index.css`
- Restart the dev server: `npm run dev`

## 👨‍💻 Author

Created as a learning project for React fundamentals.

---

**Happy Note Taking! **
