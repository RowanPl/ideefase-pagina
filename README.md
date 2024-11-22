# IdeeFase Template Generator

A web-based tool for generating structured feedback on student project proposals. This application helps evaluators provide consistent, criteria-based feedback for different types of development projects (Frontend, Backend, and Fullstack).

![afbeelding](https://github.com/user-attachments/assets/78e96eb8-1745-46ad-9dbd-ba017981495b)


## Features

- 🎯 Project type-specific feedback templates
- ✅ Automatic requirement validation
- 📝 Real-time template generation
- 📋 One-click copy to clipboard
- 🎨 Modern, responsive interface
- 🔄 Clear form functionality with end date preservation option

## Project Types and Requirements

### Backend & Fullstack Projects
- **User Roles**
  - Minimum: 2 roles
  - Maximum: 3 roles
- **Entities (Classes)**
  - Backend: 6-7 entities
  - Fullstack: 5-6 entities
  - Automatically includes:
    - User entity (login credentials)
    - Security entity

### Frontend Projects
- Minimum 4 functionalities
- API compliance checking
- Backend integration validation

## Installation

1. Clone the repository:
```bash
git clone https://github.com/RowanPl/Ideefase-pagina.git
```

2. Navigate to the project directory:
```bash
cd Ideefase-pagina
```

3. Open `index.html` in your web browser or serve it using a local development server.

## Usage

1. Select the project type (Frontend, Backend, or Fullstack)
2. Enter the student's name
3. Fill in the required fields based on project type:
   - Backend/Fullstack: User roles and entities
   - Frontend: Functionalities and any API/backend issues
4. Add any additional comments in the "Toelichting" field
5. Set the deadline date if needed
6. The template will generate automatically
7. Click "Copy to clipboard" to copy the generated feedback

## Project Structure

```
ideefase-template-generator/
├── index.html          # Main HTML file
├── styles.css          # Tailwind CSS styling
└── script.js          # Application logic
```

## Configuration

Key configuration options can be found in the `CONFIG` object in `script.js`:

```javascript
const CONFIG = {
    MINIMUM_FUNC: 4,
    MINIMUM_ROL: 2,
    MAXIMUM_ROL: 3,
    VARIANT_REQUIREMENTS: {
        Backend: { min: 6, max: 7 },
        Fullstack: { min: 5, max: 6 },
        Frontend: { min: 4, max: 5 }
    }
};
```

## Technologies Used

- HTML5
- JavaScript (ES6+)
- Tailwind CSS
- Font Awesome icons

## Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Development

### Building CSS

This project uses Tailwind CSS. To modify the styles:

1. Install dependencies:
```bash
npm install
```

2. Run Tailwind CLI:
```bash
npx tailwindcss -i ./styles.css -o ./dist/styles.css --watch
```

### Custom Components

The project includes several custom components:
- Toast notifications for user feedback
- Dynamic form sections
- Real-time template generation

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- Tailwind CSS for the utility-first CSS framework
- Font Awesome for the icons
- The educational institution for the project requirements specification

## Support

For support, open an issue in the GitHub repository.

---

Made with ❤️ for improving the feedback process in education
