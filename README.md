# Commonplace — Good Things, Shared

> A calm, community-inspired social feed for sharing small discoveries, thoughtful notes, and everyday ideas.

Commonplace is a responsive front-end web app concept built with **HTML, CSS, and vanilla JavaScript**. Its editorial-inspired interface is designed to make online sharing feel more personal and less noisy.

## Preview

Open `index.html` in a modern browser to explore the interface locally.

> **Project status:** Front-end prototype. Posts and interactions are stored in the browser's `localStorage`; there is no server, account system, or cross-device synchronization in this version.

## Features

- **Responsive layout** for desktop, tablet, and mobile screens
- **Social feed** with sample community posts
- **Create a note** with a 500-character limit
- **Image attachments** with a local preview
- **Like and save** posts
- **Replies/comments** on posts
- **Topic-based discovery** for themes such as Design, Writing, and Slow Living
- **Search** posts by author, text, or topic
- **Feed filters** for For You, Following, Latest, and Saved
- **Follow controls** in the suggested-people panel
- **Toast notifications** for user feedback
- **Accessible UI details**, including button labels, semantic landmarks, and visible keyboard focus styles
- **Reduced-motion support** for visitors who prefer less animation

## Tech Stack

| Technology | Purpose |
| --- | --- |
| HTML5 | Semantic page structure and dialogs |
| CSS3 | Layout, responsive styling, animation, and visual design |
| Vanilla JavaScript | Feed rendering and client-side interactions |
| Browser `localStorage` | Persistence of posts and interaction state |
| Google Fonts | DM Sans and Fraunces typography |
| Unsplash image URLs | Demo avatars and editorial imagery |

No framework, package manager, build step, or external API key is required to run the prototype.

## Getting Started

### Option 1: Open directly

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Start creating notes and trying the feed interactions.

### Option 2: Run a local development server

If you have Python installed, open a terminal in the project directory and run:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

You can also use the **Live Server** extension in Visual Studio Code.

## Project Structure

```text
commonplace/
├── index.html   # Main page and UI structure
├── styles.css   # Design system, layout, and responsive rules
├── app.js       # Feed state, rendering, and interactions
├── README.md    # Project documentation
├── LICENSE      # Project license
└── .gitignore   # Files excluded from version control
```

## How It Works

1. `index.html` defines the application shell, navigation, feed, side panels, composer dialog, and notification area.
2. `styles.css` provides the color palette, typography, responsive breakpoints, card styling, and interaction states.
3. `app.js` renders posts from a local data model and attaches event listeners for composing, searching, filtering, liking, saving, and replying.
4. The browser stores post data under the `commonplace-posts-v1` local-storage key.

### Data and Privacy Notes

- The prototype does not include a backend or authentication.
- Local posts are stored only in the current browser profile and are not synced to other users or devices.
- Clearing browser site data may remove saved prototype content.
- Images selected for a post are stored as browser-side data; large images can use significant local storage.
- Demo imagery and Google Fonts are loaded from third-party hosts, so those assets require an internet connection.

## Current Limitations

The following interface elements are illustrative or not yet connected to a real service:

- User registration, login, and profile management
- Real-time messaging and notifications
- A production follow graph and personalized feed
- Server-side storage, moderation, and content reporting
- Link previews and external content ingestion
- Production deployment, monitoring, and automated tests

The “Following,” messaging, notification, and profile-related UI should be treated as prototype behavior rather than production functionality.

## Roadmap

- [ ] Add a backend API and persistent database
- [ ] Implement secure authentication and user profiles
- [ ] Connect follow relationships and feed personalization
- [ ] Add real messaging and notification delivery
- [ ] Improve image upload validation and storage
- [ ] Add moderation, reporting, and abuse prevention
- [ ] Add unit and browser-based integration tests
- [ ] Add CI checks and deployment documentation
- [ ] Add metadata, social sharing previews, and a production favicon

## Contributing

Contributions, suggestions, and issue reports are welcome.

1. Fork the repository.
2. Create a branch: `git checkout -b feat/your-change`
3. Make a focused change and test it in a browser.
4. Commit with a clear message: `git commit -m "Add your change"`
5. Push the branch and open a pull request.

For substantial changes, open an issue first to discuss the proposal.

## License

This project is distributed under the MIT License. See [`LICENSE`](LICENSE) for details.

## Acknowledgements

- [Google Fonts](https://fonts.google.com/) for DM Sans and Fraunces
- [Unsplash](https://unsplash.com/) for demo imagery

---

Built as a front-end project exploring thoughtful, community-oriented social experiences.
