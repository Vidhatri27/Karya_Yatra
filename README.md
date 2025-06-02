# Karya_Yatra
# Karya Yatra - Todo Application

**Journey through your to-do's**

Karya Yatra is a modern, responsive todo application that helps you organize and manage your daily tasks efficiently. Built with a clean interface and powerful features, it's designed to make task management simple and enjoyable.

## Features

### Authentication System
- **User Registration & Login**: Secure email/password authentication
- **Google OAuth Integration**: Quick login with Google accounts
- **Password Reset**: Forgot password functionality with email verification
- **Session Management**: Persistent login with JWT tokens

### Task Management
- **Add Tasks**: Create new todos with a simple interface
- **Mark Complete**: Toggle task completion status
- **Delete Tasks**: Remove unwanted tasks
- **Filter Tasks**: View all, completed, or incomplete tasks
- **Real-time Updates**: Instant synchronization with backend

### User Experience
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Modern UI**: Clean, minimalist interface with smooth animations
- **Password Visibility Toggle**: Show/hide password fields
- **Error Handling**: User-friendly error messages and feedback

### Notification System
- **Reminder Alerts**: Set custom reminders for important tasks
- **Browser Notifications**: Desktop notifications when reminders trigger

## Technologies Used

### Frontend
- **HTML5**: Semantic markup structure
- **CSS3**: Modern styling with Flexbox and animations
- **JavaScript (ES6+)**: Interactive functionality and API integration
- **Font Awesome**: Icon library for UI elements
- **Google Fonts**: Poppins and Dancing Script typography

### Backend Integration
- **RESTful API**: Communicates with Node.js/Express backend
- **JWT Authentication**: Secure token-based authentication
- **Local Storage**: Client-side data persistence

## Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Backend API server running on `http://localhost:5001`

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd karya-yatra
   ```

2. **Open the application**
   - Simply open `index.html` in your web browser
   - Or serve it using a local development server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

3. **Backend Setup**
   - Ensure your backend API is running on `http://localhost:5001`
   - The application expects the following API endpoints:
     - `POST /api/auth/login`
     - `POST /api/auth/signup`
     - `POST /api/auth/google`
     - `POST /api/auth/request-password-reset`
     - `GET /api/todos`
     - `POST /api/todos`
     - `PUT /api/todos/:id/toggle`
     - `DELETE /api/todos/:id`

## Usage

### Getting Started
1. **Create Account**: Sign up with your email or use Google OAuth
2. **Login**: Access your account with your credentials
3. **Add Tasks**: Use the input field to create new todos
4. **Manage Tasks**: 
   - Click the checkmark to mark tasks complete
   - Click the trash icon to delete tasks
   - Use filter buttons to view specific task categories

### Setting Reminders
1. Select a date and time using the reminder form
2. Click "Set Reminder" to schedule a notification
3. Grant notification permissions when prompted
4. Receive desktop notifications at the scheduled time

## File Structure

```
karya-yatra/
├── index.html          # Main application file
├── README.md          # Project documentation
└── assets/            # (Optional) Additional resources
```

## API Configuration

The application is configured to communicate with a backend API at `http://localhost:5001/api`. To modify the API endpoint, update the `API_BASE_URL` constant in the JavaScript section:

```javascript
const API_BASE_URL = 'your-api-endpoint';
```

## Browser Compatibility

- **Chrome**: 60+
- **Firefox**: 55+
- **Safari**: 12+
- **Edge**: 79+

## Features Overview

### Authentication Flow
1. Users can register with email/password or Google OAuth
2. JWT tokens are stored locally for session persistence
3. Password reset functionality via email verification
4. Secure logout with token cleanup

### Task Management Flow
1. Authenticated users can create, read, update, and delete tasks
2. Tasks are synchronized with the backend API
3. Local storage provides offline access to user data
4. Real-time filtering and status updates

## Security Features

- **JWT Token Authentication**: Secure API communication
- **Input Validation**: Client and server-side validation
- **Password Security**: Masked password inputs with toggle visibility
- **Session Management**: Automatic token cleanup on logout

## Customization

### Styling
The application uses a warm color palette with the primary color `rgb(108, 33, 52)`. To customize:

1. Update CSS custom properties
2. Modify the color scheme in the `<style>` section
3. Adjust typography by changing Google Fonts imports

### Functionality
- Add new task categories or priorities
- Implement task due dates
- Add task descriptions or notes
- Integrate with calendar applications

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

For support, feature requests, or bug reports, please create an issue in the repository or contact the development team.

---

**Karya Yatra** - Making task management a journey worth taking! 🚀
