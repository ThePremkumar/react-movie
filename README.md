# FilmChoice 🎬

**🚀 Live Site**: [filmchoice.vercel.app](https://filmchoice.vercel.app/)

A modern web application for discovering and exploring movies and TV shows. Built with React and deployed on Vercel for optimal performance and user experience.

## 🌟 Features

- **Movie & TV Show Discovery**: Browse through a vast collection of movies and television series
- **Search Functionality**: Find your favorite titles quickly with intelligent search
- **Detailed Information**: Get comprehensive details about movies including cast, crew, ratings, and synopsis
- **Responsive Design**: Seamless experience across desktop, tablet, and mobile devices
- **Real-time Data**: Up-to-date information powered by movie databases
- **User-Friendly Interface**: Clean, intuitive design for effortless navigation

## 🚀 Technologies Used

- **Frontend**: React.js
- **Deployment**: Vercel
- **Styling**: CSS3/Tailwind CSS
- **API Integration**: Movie database APIs (TMDB/OMDB)
- **Build Tool**: Create React App or similar bundler

## 🏗️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/ThePremkumar/react-movie.git
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Environment Variables**
   Create a `.env` file in the root directory and add your API keys:
   ```env
    VITE_TMDB_API_KEY=
    VITE_APPWRITE_PROJECT_ID=
    VITE_APPWRITE_DATABASE_ID=
    VITE_APPWRITE_COLLECTION_ID=
   ```

4. **Start the development server**
   ```bash
   npm start
   # or
   yarn start
   ```

5. **Build for production**
   ```bash
   npm run build
   # or
   yarn build
   ```

## 📱 Usage

1. **Browse Movies**: Explore trending, popular, or top-rated movies on the homepage
2. **Search**: Use the search bar to find specific movies or TV shows
3. **View Details**: Click on any title to see detailed information, cast, and crew
4. **Categories**: Filter content by genres, release year, or ratings
5. **Responsive Viewing**: Access the site on any device for optimal experience

## 🎯 API Integration

This application integrates with movie databases to provide:
- Movie and TV show metadata
- High-quality poster and backdrop images
- Cast and crew information
- User ratings and reviews
- Streaming availability (where applicable)

## 🔧 Configuration

### Environment Variables

| Variable                | Description | Required |
|-------------------------|-------------|----------|
| `VITE_APP_TMDB_API_KEY` | The Movie Database API key | Yes |
| `VITE_APP_API_BASE_URL` | Base URL for API requests | Yes |

### API Setup

1. Visit [The Movie Database (TMDB)](https://www.themoviedb.org/settings/api)
2. Create an account and request an API key
3. Add your API key to the `.env` file

## 🚀 Deployment

This project is optimized for Vercel deployment:

1. **Connect to Vercel**
    - Import your repository to Vercel
    - Configure environment variables in the Vercel dashboard
    - Deploy automatically on every push to main branch

2. **Manual Deployment**
   ```bash
   npm run build
   vercel --prod
   ```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [The Movie Database (TMDB)](https://www.themoviedb.org/) for providing the movie data API
- [Vercel](https://vercel.com/) for hosting and deployment platform
- React community for the amazing framework and ecosystem

## 📞 Support

If you have any questions or run into issues, please:
- Open an issue on GitHub
- Check the documentation
- Contact the maintainers

---

⭐ If you found this project helpful, please give it a star on GitHub!

**Live Site**: [filmchoice.vercel.app](https://filmchoice.vercel.app/)