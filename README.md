# Color Generator 🎨

This project is a React application that generates color shades and tints from a user-provided color code (HEX or color name). The generated color tones are visually displayed, and users can copy them to the clipboard.

## 🗃️ Table of Contents

- About the Project
- Technologies Used
- Installation
- How It Works
- Code Structure
- Example Scenarios
- Refresh Your Knowledge
- Contributing

## 🌟 About the Project

This project automatically generates color shades from a given color code (HEX or color name). Users can visually see the generated color shades and copy them to the clipboard. The project is built using React and the `values.js` library.

## 🛠 Technologies Used

- **React**: Used for building the user interface.
- **values.js**: A library used to generate color shades.
- **React Toastify**: Used to display notifications to users.
- **CSS**: Used for styling.

## 🚀 Installation

To run the project locally, follow these steps:

### Clone the repository:
```bash
git clone https://github.com/Ulku-dur/color-generator
```

### Navigate to the project directory:
```bash
cd https://github.com/Ulku-dur/color-generator
```

### Install dependencies:
```bash
npm install
```

### Start the project:
```bash
npm run dev
```

### Open in browser:
The project will run on `http://localhost:5173`.

## 🎯 How It Works

### Enter a Color:
- Input a HEX code (e.g., `#f15025`) or a color name (e.g., `red`).
- Alternatively, use the color picker to select a color.

### Generate Color Shades:
- Click the **"Generate"** button.
- The application automatically creates and displays color shades based on the input.

### Copy Colors:
- Click on any color shade to copy its HEX code to the clipboard.
- A notification appears upon successful copying.

## 🧩 Code Structure

### 1. `App.js`

#### **States:**
- `color`: Stores the user-inputted color.
- `list`: Stores the generated color shades.

#### **Functions:**
- `handleSubmit`: Generates color shades when the form is submitted.

#### **Components:**
- `ColorsList`: Displays the generated color shades.

### 2. `ColorsList.js`

#### **Props:**
- `colors`: Array of generated color shades.

#### **Structure:**
- Renders the `SingleColor` component for each color shade.

### 3. `SingleColor.js`

#### **Props:**
- `color`: Contains HEX and weight details.

#### **Functions:**
- `saveToClipboard`: Copies the color to the clipboard.

## 📚 Example Scenarios

### **Scenario 1: Entering a HEX Code**
1. Enter `#f15025` in the input field.
2. Click the **"Generate"** button.
3. Shades of orange are displayed.

### **Scenario 2: Using the Color Picker**
1. Open the color picker and select a color.
2. Click the **"Generate"** button.
3. Shades of the selected color are displayed.

## 🔄 Refresh Your Knowledge

When revisiting this project, review the following concepts:

### **React State Management:**
- How to use the `useState` hook?
- How to update states?

### **Form Handling:**
- How is form data processed upon submission?
- Why use `e.preventDefault()`?

### **Generating Color Shades:**
- How does the `values.js` library work?
- What does the `all(10)` method do?

### **Copying to Clipboard:**
- How to use `navigator.clipboard` API?
- How to handle errors effectively?

## 🤝 Contributing

If you'd like to contribute, follow these steps:

1. **Fork** the repository.
2. **Create a new branch:**
   ```bash
   git checkout -b new-feature
   ```
3. **Make your changes and commit:**
   ```bash
   git commit -m "Added new feature"
   ```
4. **Push your branch:**
   ```bash
   git push origin new-feature
   ```
5. **Create a pull request.**

