# Book Club Hub

A collaborative web application for managing book club activities, built with vanilla JavaScript and Firebase.

## 🌐 Live Site

**URL:** https://maryoc.github.io/book-club/

## 📖 Overview

Book Club Hub is a real-time collaborative platform where book club members can:
- Suggest and vote on books to read
- Propose and vote on meeting locations
- Share availability and schedule meetings
- Review and rate books they've read

All data syncs in real-time across all users using Firebase Realtime Database.

## ✨ Features

### 1. Book Suggestions
- Add book suggestions with title, author, and your name
- Vote on books you'd like to read
- Automatic sorting by number of votes
- Delete suggestions when needed

### 2. Location Ideas
- Suggest meeting locations with details and address
- Vote on preferred locations
- Automatic sorting by popularity
- Delete locations when needed

### 3. Calendar & Availability
- Interactive monthly calendar view
- Mark dates when you're available
- Set next meeting date with one tap
- Select meeting time (with AM/PM formatting)
- Choose book and location from suggestions
- See how many members are available each day
- Mobile-optimized with dedicated "Set as Next Meeting" button
- Global banner shows upcoming meeting details across all tabs

### 4. Past Book Reviews
- Review books with 5-star rating system
- Add detailed notes about each book
- Pull books directly from suggestions or enter manually
- Edit existing reviews
- Delete reviews when needed

## 🛠️ Technologies Used

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Database:** Firebase Realtime Database
- **Hosting:** GitHub Pages
- **Design:** Apple-inspired design system with clean, simple UI
- **Responsive:** Mobile-first design with optimized layouts for all screen sizes

## 🎨 Design Features

- Clean, minimal Apple-inspired aesthetic
- SF Pro font family
- Responsive design for mobile and desktop
- Smooth animations and transitions
- Touch-optimized interactions
- Haptic feedback on mobile devices (when supported)

## 📱 Mobile Support

The app is fully optimized for mobile devices:
- Responsive layout adapts to screen size
- Touch-friendly tap targets
- Simplified navigation on small screens
- Calendar fits properly on mobile without overflow
- Dedicated button for setting meetings (no complex gestures required)

## 🔥 Firebase Configuration

The app uses Firebase Realtime Database for real-time collaboration:

- **Project Name:** book-club-hub-35666
- **Database URL:** https://book-club-hub-35666-default-rtdb.firebaseio.com
- **Authentication:** Currently in test mode for easy access

### Data Structure

```
book-club-hub/
├── books/              # Array of book suggestions
├── locations/          # Array of location suggestions
├── availability/       # Object mapping dates to availability counts
├── nextMeeting/        # String: next meeting date
├── meetingLocation/    # String: selected location ID
├── meetingBook/        # String: selected book ID
├── meetingTime/        # String: meeting time in HH:mm format
└── reviews/            # Array of book reviews
```

## 🚀 Deployment

This app is deployed using GitHub Pages:

1. **Repository:** https://github.com/maryoc/book-club
2. **Branch:** main
3. **Path:** / (root)
4. **Custom Domain:** None (using default GitHub Pages URL)

### Deploy Updates

To deploy changes:

1. Make changes to `index.html`
2. Commit changes to the repository
3. Push to the `main` branch
4. GitHub Pages automatically rebuilds (takes 1-2 minutes)

## 📂 Repository Information

- **Repository Name:** book-club
- **Owner:** maryoc
- **Files:**
  - `index.html` - Single-page application (all HTML, CSS, and JavaScript)
  - `README.md` - This documentation

## 🔒 Security Considerations

**Current Status:** Firebase is in test mode, allowing read/write access to anyone with the URL.

**For Production Use:** Consider adding Firebase security rules to:
- Require authentication
- Limit write access to authenticated users
- Validate data structure
- Prevent malicious data

### Recommended Security Rules

```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

For a more secure setup, consider implementing Firebase Authentication.

## 🎯 Future Enhancement Ideas

- User authentication (Firebase Auth)
- Member profiles with avatars
- Discussion threads for each book
- Reading progress tracking
- Email notifications for upcoming meetings
- Export meeting history
- Photo uploads for book covers
- Integration with book APIs (Google Books, Goodreads)
- Dark mode toggle
- Attendance tracking
- Meeting notes and minutes

## 💻 Local Development

To run locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/maryoc/book-club.git
   ```

2. Open `index.html` in a web browser

3. Changes will sync with the live Firebase database

**Note:** Since Firebase is shared, local testing will affect production data. Consider creating a separate Firebase project for development.

## 🤝 Contributing

This is a personal book club project. If you'd like to use it for your own book club:

1. Fork this repository
2. Create your own Firebase project
3. Replace the Firebase configuration in `index.html`
4. Deploy to your own GitHub Pages

## 📧 Contact

**Repository Owner:** maryoc
**Project:** Book Club Hub

## 📄 License

This project is for personal use. Feel free to fork and customize for your own book club!

---

Built with ❤️ using Firebase and GitHub Pages
