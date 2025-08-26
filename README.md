# Todo Application

A modern, feature-rich todo application built with Ruby on Rails. This application provides a clean and intuitive interface for managing tasks and staying organized.

## Features

- ✨ Create, edit, and delete todos
- 📝 Mark todos as complete/incomplete
- 🏷️ Organize todos with categories
- 📅 Set due dates for todos
- 🔍 Search and filter todos
- 📱 Responsive design for mobile devices
- ⚡ Fast and efficient performance

## Technology Stack

- **Backend**: Ruby on Rails 7
- **Database**: SQLite3 (development), PostgreSQL (production)
- **Frontend**: HTML, CSS, JavaScript
- **Asset Pipeline**: Sprockets
- **Testing**: Minitest
- **Deployment**: Docker support included

## Prerequisites

Before you begin, ensure you have the following installed:

- Ruby 3.0 or higher
- Rails 7.0 or higher
- SQLite3 (for development)
- Node.js (for asset compilation)
- Yarn or npm

## Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd todo
   ```

2. **Install Ruby dependencies**
   ```bash
   bundle install
   ```

3. **Install JavaScript dependencies**
   ```bash
   yarn install
   # or
   npm install
   ```

4. **Set up the database**
   ```bash
   rails db:create
   rails db:migrate
   rails db:seed
   ```

5. **Start the server**
   ```bash
   rails server
   ```

6. **Visit the application**
   Open your browser and navigate to `http://localhost:3000`

## Usage

### Basic Todo Management

1. **Create a new todo**: Click the "Add Todo" button and enter your task details
2. **Edit a todo**: Click the edit icon next to any todo to modify it
3. **Mark as complete**: Check the checkbox to mark a todo as done
4. **Delete a todo**: Click the delete icon to remove a todo

### Advanced Features

- **Filter todos**: Use the filter options to view todos by status
- **Search todos**: Use the search bar to find specific todos
- **Sort todos**: Click column headers to sort todos by different criteria

## Database Setup

The application uses SQLite3 for development. To set up the database:

```bash
# Create the database
rails db:create

# Run migrations
rails db:migrate

# Seed with sample data (optional)
rails db:seed

# Reset database (if needed)
rails db:reset
```

## Testing

Run the test suite to ensure everything is working correctly:

```bash
# Run all tests
rails test

# Run specific test files
rails test test/models/
rails test test/controllers/
rails test test/system/

# Run tests with coverage
COVERAGE=true rails test
```

## Development

### Development Workflow

1. **Start the development server**
   ```bash
   rails server
   ```

2. **Run tests before committing**
   ```bash
   rails test
   ```

3. **Check code style**
   ```bash
   bin/rubocop
   ```

4. **Update dependencies**
   ```bash
   bundle update
   yarn upgrade
   ```

### Code Quality

- Follow Ruby style guidelines
- Write tests for new features
- Use meaningful commit messages
- Keep the codebase clean and well-documented

### Debugging

- Use `rails console` for interactive debugging
- Check logs in `log/development.log`
- Use `debugger` statements for breakpoint debugging

## Deployment

### Docker Deployment

The application includes Docker support:

```bash
# Build the Docker image
docker build -t todo-app .

# Run the container
docker run -p 3000:3000 todo-app
```

### Production Deployment

For production deployment:

1. Set up environment variables
2. Configure your database (PostgreSQL recommended)
3. Set up asset compilation
4. Configure your web server (Nginx/Apache)
5. Set up SSL certificates

## API Documentation

The application provides a RESTful API for todo management:

- `GET /api/todos` - List all todos
- `POST /api/todos` - Create a new todo
- `GET /api/todos/:id` - Get a specific todo
- `PUT /api/todos/:id` - Update a todo
- `DELETE /api/todos/:id` - Delete a todo

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Contribution Guidelines

- Write clear, descriptive commit messages
- Include tests for new functionality
- Follow the existing code style
- Update documentation as needed
- Ensure all tests pass before submitting

## Troubleshooting

### Common Issues

**Database connection errors**
```bash
rails db:create
rails db:migrate
```

**Asset compilation issues**
```bash
rails assets:precompile
rails assets:clean
```

**Permission errors**
```bash
chmod +x bin/rails
chmod +x bin/setup
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/your-repo/todo/issues) page
2. Create a new issue with detailed information
3. Contact the maintainers

## Acknowledgments

- Built with [Ruby on Rails](https://rubyonrails.org/)
- Icons provided by [Heroicons](https://heroicons.com/)
- Styling inspired by modern design principles

---

**Happy coding! 🚀**
