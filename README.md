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
- **Backend**: Appwrite (Database & Authentication)
- **Deployment**: Vercel
- **Styling**: CSS3/Tailwind CSS
- **API Integration**: Movie database APIs (TMDB/OMDB)
- **Build Tool**: Vite
- **Database**: Appwrite Database for search history and trending data

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
   VITE_TMDB_API=your_tmdb_read_access_token_here
   VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
   VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
   VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
   VITE_APPWRITE_ENDPOINT=your_appwrite_endpoint_here
   ```

4. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. **Build for production**
   ```bash
   npm run build
   # or
   yarn build
   ```

6. **Run with Docker**
   You can also build and run the application containerized in production mode:
   ```bash
   # Build the docker image
   docker build -t movie-suggestion-app .

   # Run the container
   docker run -d -p 8080:80 --name movie-app movie-suggestion-app
   ```
   Access the app at `http://localhost:8080`

## 📱 Usage

1. **Browse Movies**: Explore trending, popular, or top-rated movies on the homepage
2. **Enhanced Search**:
    - Use the search bar to find specific movies or TV shows
    - Search history is stored in Appwrite for faster subsequent searches
    - Trending searches influence the trending algorithm
3. **View Details**: Click on any title to see detailed information, cast, and crew
4. **Trending Algorithm**: Movies gain trending scores based on:
    - Search frequency
    - User interactions
    - Real-time popularity data
5. **Categories**: Filter content by genres, release year, or ratings
6. **Responsive Viewing**: Access the site on any device for optimal experience

## 🎯 API Integration & Backend

This application integrates with multiple services:

### TMDB API (The Movie Database)
- Movie and TV show metadata
- High-quality poster and backdrop images
- Cast and crew information
- User ratings and reviews
- Streaming availability (where applicable)

### Appwrite Backend Services
- **Database**: Store search history and trending data
- **Collections**: Manage movie favorites and user preferences
- **Real-time Updates**: Live trending data synchronization
- **Search Optimization**: Enhanced search functionality with cached results

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `VITE_TMDB_API` | The Movie Database Read Access Token (JWT) | Yes |
| `VITE_APPWRITE_PROJECT_ID` | Appwrite project identifier | Yes |
| `VITE_APPWRITE_DATABASE_ID` | Appwrite database identifier | Yes |
| `VITE_APPWRITE_COLLECTION_ID` | Appwrite collection identifier | Yes |
| `VITE_APPWRITE_ENDPOINT` | Appwrite endpoint URL | Yes |

### TMDB API Setup

1. Visit [The Movie Database (TMDB)](https://www.themoviedb.org/settings/api)
2. Create an account and request an API key
3. Add your API key to the `.env` file

### Appwrite Backend Setup

1. **Create Appwrite Account**
    - Visit [Appwrite Console](https://cloud.appwrite.io/)
    - Create a new account or sign in

2. **Create New Project**
   ```bash
   # Create a new project in Appwrite console
   # Note down the Project ID
   ```

3. **Setup Database**
   ```bash
   # Create a new database
   # Create collections for:
   # - Search History
   # - Trending Movies
   # - User Favorites
   ```

4. **Configure Collections**
    - **Search Collection Attributes**:
        - `query` (string): Search term
        - `results` (string): JSON string of search results
        - `timestamp` (datetime): When search was performed
        - `popularity` (integer): Search frequency

    - **Trending Collection Attributes**:
        - `movieId` (string): TMDB movie ID
        - `title` (string): Movie title
        - `trendingScore` (integer): Trending calculation score
        - `lastUpdated` (datetime): Last update timestamp

5. **Set Permissions**
    - Configure read/write permissions for collections
    - Set up user authentication if needed

## 🚀 Deployment

This project is optimized for Vercel deployment with Appwrite backend:

1. **Connect to Vercel**
    - Import your repository to Vercel
    - Configure environment variables in the Vercel dashboard:
        - `VITE_TMDB_API_KEY`
        - `VITE_APPWRITE_PROJECT_ID`
        - `VITE_APPWRITE_DATABASE_ID`
        - `VITE_APPWRITE_COLLECTION_ID`
    - Deploy automatically on every push to main branch

2. **Manual Deployment**
   ```bash
   npm run build
   vercel --prod
   ```

3. **Appwrite Production Setup**
    - Ensure Appwrite project is configured for production
    - Update CORS settings to include your Vercel domain
    - Configure production database and collections

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
- [Appwrite](https://appwrite.io/) for backend-as-a-service platform
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