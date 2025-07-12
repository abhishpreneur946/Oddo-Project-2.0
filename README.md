# StackIt - A Minimal Q&A Forum Platform

StackIt is a modern, minimal question-and-answer platform designed for collaborative learning and structured knowledge sharing. Built with React, Node.js, and MongoDB, it provides a clean and intuitive interface for asking questions, providing answers, and engaging with the community.

## 🚀 Features

### Core Features
- **Ask Questions**: Create detailed questions with rich text formatting
- **Rich Text Editor**: Support for bold, italic, lists, links, images, and more
- **Answer Questions**: Provide comprehensive answers with the same rich editor
- **Voting System**: Upvote and downvote questions and answers
- **Accept Answers**: Mark the best answer for your questions
- **Tagging System**: Organize content with relevant tags
- **Real-time Notifications**: Get notified about answers, comments, and mentions
- **Search Functionality**: Find questions quickly with powerful search

### User Management
- **User Registration & Login**: Secure authentication system
- **User Profiles**: Customizable profiles with bio, avatar, and stats
- **Role-based Access**: Guest, User, and Admin roles
- **Reputation System**: Build reputation through quality contributions

### Community Features
- **Real-time Updates**: Live notifications and updates
- **Comment System**: Add comments to answers
- **Mention System**: Mention users with @username
- **View Tracking**: Track question views and engagement
- **Popular Tags**: Discover trending topics

## 🛠️ Tech Stack

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **Socket.IO** - Real-time communication
- **JWT** - Authentication
- **bcryptjs** - Password hashing
- **Multer** - File uploads

### Frontend
- **React** - UI library
- **React Router** - Navigation
- **Tailwind CSS** - Styling
- **Framer Motion** - Animations
- **React Quill** - Rich text editor
- **Axios** - HTTP client
- **Socket.IO Client** - Real-time updates
- **React Hot Toast** - Notifications

## 📦 Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud)
- npm or yarn

### Backend Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd stackit-qa-forum
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Configuration**
   Create a `.env` file in the root directory:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/stackit
   JWT_SECRET=your-secret-key-here
   CLIENT_URL=http://localhost:3000
   ```

4. **Start the server**
   ```bash
   npm run server
   ```

### Frontend Setup

1. **Navigate to client directory**
   ```bash
   cd client
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

### Full Stack Development

To run both backend and frontend simultaneously:
```bash
# From the root directory
npm run dev
```

## 🗄️ Database Setup

The application uses MongoDB with the following collections:
- **Users**: User accounts and profiles
- **Questions**: Questions with metadata
- **Answers**: Answers to questions
- **Notifications**: Real-time notifications

## 🔧 Configuration

### Environment Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `PORT` | Server port | 5000 |
| `MONGODB_URI` | MongoDB connection string | mongodb://localhost:27017/stackit |
| `JWT_SECRET` | JWT signing secret | your-secret-key-here |
| `CLIENT_URL` | Frontend URL | http://localhost:3000 |

### API Endpoints

#### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get current user
- `PUT /api/auth/profile` - Update profile

#### Questions
- `GET /api/questions` - Get all questions
- `POST /api/questions` - Create question
- `GET /api/questions/:id` - Get single question
- `PUT /api/questions/:id` - Update question
- `DELETE /api/questions/:id` - Delete question
- `POST /api/questions/:id/vote` - Vote on question

#### Answers
- `GET /api/answers/question/:questionId` - Get answers for question
- `POST /api/answers` - Create answer
- `PUT /api/answers/:id` - Update answer
- `DELETE /api/answers/:id` - Delete answer
- `POST /api/answers/:id/vote` - Vote on answer

#### Notifications
- `GET /api/notifications` - Get user notifications
- `PUT /api/notifications/:id/read` - Mark as read
- `PUT /api/notifications/read-all` - Mark all as read

## 🎨 Features in Detail

### Rich Text Editor
The platform includes a comprehensive rich text editor with:
- **Text Formatting**: Bold, italic, strikethrough
- **Lists**: Numbered and bullet points
- **Links**: Insert and manage hyperlinks
- **Images**: Upload and embed images
- **Code Blocks**: Syntax highlighting for code
- **Alignment**: Left, center, right text alignment

### Notification System
Real-time notifications for:
- New answers to your questions
- Comments on your answers
- Mentions using @username
- Votes on your content
- Accepted answers

### Voting System
- Upvote/downvote questions and answers
- Prevent duplicate votes
- Track vote counts
- Build user reputation

### Search & Discovery
- Full-text search across questions
- Tag-based filtering
- Sort by newest, votes, views
- Popular tags discovery

## 🚀 Deployment

### Backend Deployment
1. Set up environment variables
2. Configure MongoDB connection
3. Deploy to your preferred platform (Heroku, Vercel, etc.)

### Frontend Deployment
1. Build the application: `npm run build`
2. Deploy the `build` folder to your hosting service

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📝 License

This project is licensed under the MIT License.

## 🆘 Support

For support and questions:
- Create an issue in the repository
- Check the documentation
- Review the API endpoints

## 🎯 Roadmap

- [ ] Advanced search filters
- [ ] Question bounties
- [ ] User badges and achievements
- [ ] Mobile app
- [ ] API rate limiting
- [ ] Content moderation tools
- [ ] Analytics dashboard
- [ ] Email notifications
- [ ] Dark mode theme
- [ ] Internationalization

---

**StackIt** - Making knowledge sharing simple and effective. 