<img width="3188" height="1202" alt="frame (3)" src="https://github.com/user-attachments/assets/517ad8e9-ad22-457d-9538-a9e62d137cd7" />


# CUPIDN'T - How universe put together 2 peeps


## Basic Details:A tongue-in-cheek dating website where mischievous Cupid delights in matching you with your worst possible match. The more incompatible you are, the closer Cupid puts you to your “perfect” mismatch.
### Team Name: [Phi]


### Team Members
- Team Lead: [Sruthi S Menon] - [LBSITW]
- Member 2: [Vaishnavi Rajesh] - [LBSITW]

### Project Description
[2-3 lines about what your project does] : Cupidn't is a playful, satirical web app where mischievous Cupid deliberately matches users with their most incompatible partners based on an entertaining personality quiz. The worse the compatibility, the closer they put you physically, with snarky commentary and humorous “commitment” roasts adding to the fun.
It’s a lighthearted parody of dating apps, designed purely for laughs and interactive amusement.


### The Problem (that doesn't exist)
[What ridiculous problem are you solving?]: Cupidn't embraces this mischievous perspective by deliberately creating hilariously incompatible matches that highlight the fun and frustration of human relationships. Rather than solving the problem of finding “the one,” it satirizes it — showing that sometimes, love (or the lack thereof) is a comedy of errors. This project playfully exposes the quirks of matchmaking and pokes fun at the idea that romance can be algorithmically perfected.

### The Solution (that nobody asked for)
[How are you solving it? Keep it fun!] :  Cupidn't embraces this mischievous perspective by deliberately creating hilariously incompatible matches that highlight the fun and frustration of human relationships. Rather than solving the problem of finding “the one,” it satirizes it — showing that sometimes, love (or the lack thereof) is a comedy of errors. This project playfully exposes the quirks of matchmaking and pokes fun at the idea that romance can be algorithmically perfected.

## Technical Details
### Technologies/Components Used
For Software:
- [Languages used] : HTML5: The structure and main markup of the app are written in standard HTML.

CSS3: All styling and visual themes are done in plain CSS, including custom fonts and responsive layouts.

JavaScript (Vanilla): All interactivity, quiz logic, data handling, profile generation, and page transitions are managed with plain (vanilla) JavaScript.



### Implementation
For Software: Architecture & Structure
Type: Single Page Application (SPA)

Languages: HTML, CSS, and vanilla JavaScript (no frameworks)

Design: 100% Frontend; all logic and state are handled in the browser (no backend/server)

User Flow
Welcome Page:

Asks for user’s name and gender with a playful prompt.

Validates inputs before letting the user proceed.

Compatibility Test:

Contains 9 multiple-choice questions (radio buttons).

Progress bar updates as each question is answered.

Each option represents a personality trait or lifestyle preference (e.g., introvert/extrovert, vegan/non-vegan).

Results Page (Cupidn’t’s Mismatches):

Shows a deliberately "bad" match: user is paired with a fake profile based on opposite answers.

Compatibility Score: Randomly generated, always low (e.g., 8–30%).

Distance Logic: Lower compatibility = closer distance ("next door neighbors"), better compatibility = far ("other side of the planet").

Profile Cards:

User and fake match profile cards, each with avatar, name, age, trait, and a commitment badge (💍) if applicable.

Commentary & Roasts:

Commentary string is generated with satirical, context-aware text reflecting the incompatibility.

If the user is “committed” and replays, displays a “Cupid’s warning” roast.

Buttons:

"Match Them" (shows a snarky match confirmation)

"Beg Cupid to Undo" (shows random roast/rejection messages from Cupid)

"Cry Silently" (shows random self-pity popups)

All buttons are handled via JS popups/alerts for snarky responses.

Persistence (within session):

User state and match history are stored in in-memory JS objects.

Previous users/matches and repeated “commitment” attempts are recorded for heckling.

Data Generation
Fake Matches:

Profile data (name, avatar, age, trait, bio, commitment status) for matches is drawn from hardcoded arrays, chosen based on user’s gender (“opposite” or “random”).

User “Traits”:

On quiz submission, a “user trait” string is generated from their answers for display.

Commentary:

Commentary bubbles are assembled from templates, sometimes referencing user answers or contrasting traits for comedic effect.

Visual/UI
Fonts:

Uses Comic Neue and Kalam (from Google Fonts) for a playful, hand-drawn vibe.

Color/Theme:

Bright, valentine-gone-wrong palette (pinks, oranges, yellows).

Profile Cards & Modals:

Results display in side-by-side cards, with hover and highlight effects.

Clickable profile modals (for details) use the same theme and show big avatars and bios.

Responsive Layout:

Flexbox used for layout; media queries ensure usability on mobile devices.

No Third-Party Dependencies
No React/Vue/Angular, no build tooling, no package managers.

Uses only ES6 vanilla JS; modularized via local functions.

Running
How to run: Just open the .html file in any modern browser. No server required.

In summary:
Cupidn't is a satirical, SPA-style website built with only HTML, CSS, and JavaScript, featuring custom UI, comical matching, and mischievous Cupid commentary—all in a single self-contained frontend file.

Related
What are the core architectural components of the implementation
How does the app handle user data and privacy considerations
What specific coding patterns or principles are applied in the implementation
How are features like location-based stories integrated into the code
What testing methods or frameworks are used to ensure quality
How does the app handle user data and privacy considerations
How does the app handle user data and privacy considerations
Here’s how the Cupidn’t app handles user data and privacy considerations based on the provided implementation:

User Data Handling
No Accounts or Logins:
Users never create accounts, log in, or provide passwords. Only a first name and selected gender are collected at the start, purely for in-page personalization and satire.

All Data Stays Local:
All user data and quiz answers are stored entirely in-browser, in JavaScript memory (variables/objects). Nothing is transmitted to a server, database, or any external location.

Session-Only Memory:
User information (name, gender, quiz answers, previous “matches,” if they’re a repeat user, etc.) exists only for as long as the page is open.

If the user closes or reloads the page, their data is lost—there’s no persistent storage.

Optional: You can extend the app to use localStorage for persistence, but by default, it doesn’t.

No Tracking or Analytics:
No cookies, tracking scripts, analytics, or third-party libraries are used.
The only remote asset is loading Comic Neue & Kalam fonts from Google Fonts for styling.

Privacy Considerations
Minimal Data Collected:

Only a non-identifying first name and a gender selection are required.

No email, age (user’s age is randomly generated for jokes), address, or sensitive information is ever requested or kept.

No Data Sharing, Selling, or External Access:
All logic, generation, and storage are entirely client-side and ephemeral.
Users’ answers and results never leave their browser.

Intended for Fun, Not Real Romance:
The app is made clear (in README/FAQs) as a satire and demo—no real-life matches, no communication between users, and no real profiles.

Example Statement (for README or Footer)
"Cupidn’t is a fully client-side app; your answers never leave your device, and no personal information is stored, shared, or tracked. All matches and profiles are fictional and generated in your own browser session for entertainment only."

Summary:
Cupidn’t is designed with privacy by default: no persistent data, no network requests, no cookies or analytics, and only in-memory, session-scoped usage of minimal, non-sensitive input. If you wish, you can include an explicit privacy statement in the app or README to reassure users of this stance.

Related
What privacy policies does this app mention regarding data collection and sharing
How does the app ensure the security of user data during transmission and storage
Are there any documented data breaches or security vulnerabilities associated with the app
What types of personal information are explicitly collected or optionally provided by users
How transparent is the app about its data handling practices and compliance with privacy laws



### Project Documentation
For Software: 
Cupidn't is a fun and interactive single-page web application that imagines Cupid as a mischievous trickster who deliberately pairs people with their most incompatible partners. Rather than perfect matches, Cupid decides to have some fun by matching opposites and placing the least compatible people physically close to each other — encouraging delightful awkwardness and chaos.

The project is a parody of modern dating apps, subverting traditional notions of compatibility with snarky commentary, quirky profiles, and playful roasts from a gleefully evil Cupid.

Key Features
Mischievous Cupid Theme: The entire app embodies a cheeky, sarcastic Cupid who relishes creating awkward and incompatible matches.

User Input & Personalization: Users enter their name and gender for a personalized touch.

Compatibility Quiz: 9 humorous personality and lifestyle questions (introvert/extrovert, commitment/situationship, vegan/non-vegan, etc.) with a progress bar.

Smart Matching Logic: Matches are chosen oppositely with low compatibility scores (5–30%), with distances representing how close or far the pair live.

Results Display:

Bold header “Cupidn't’s Mismatches” plus an annoyed Cupid emoji.

Fake compatibility score and cheeky distance text.

Side-by-side user + fake match cards with avatars, ages, traits, and commitment badges.

Snarky and dynamically generated commentary bubble.

User Interaction Buttons:

Match Them: Confirms the dreaded pairing with a funny alert.

Beg Cupid to Undo: Enables hilarious “no take-backs” roast messages.

Cry Silently: Offers empathetic but humorous cries.

Returning User Roasts: Tracks repeat committed users and gives special roasting warnings.

Data Handling: All data lives on the client side, session-only, with no external communication.

Responsive and Accessible Design: Works well on desktop and mobile, uses playful fonts and bright color scheme.

User Flow
Welcome Page:
User inputs their name and gender.

Compatibility Quiz:
A series of 9 amusing questions about personality and preferences.

Compatibility Calculation:

Based on quiz answers, an incompatible “opposite” match is generated.

Compatibility score is intentionally low.

Distance between matched users is determined inversely to compatibility.

Personalized, snarky commentary is created.

Matching Result Page:

Displays scores, distances, user & match cards, and witty commentary.

Offers interactive buttons for “Match Them,” “Beg Cupid to Undo,” and “Cry Silently.”

Tracks returning users for extra roasts when they choose “commitment” repeatedly.

Technologies Used
Languages:

HTML5 for structure and markup

CSS3 for styling, including Google Fonts for Comic Neue & Kalam (handwritten comic style)

Vanilla JavaScript (ES6) for all application logic and interactivity

Libraries/Frameworks: None external

Tools: Pure frontend, single HTML file, no build tools or backend required

Privacy & Data Handling
No personal data storage: Only name and gender are collected locally for personalization.

Client-side only: All user input, fake matches, and logic happen inside the browser; no data is sent or saved externally.

Session-limited data: No local storage or cookies are used, so data is lost on page reload or close.

No tracking or analytics: The app respects user privacy fully.

How to Run
Save the complete HTML file (e.g., cupidnt.html) locally.

Open it in any modern web browser (Chrome, Firefox, Edge, Safari).

Follow on-screen instructions to enter your name, gender, and take the fun quiz.

View your mischievous match and enjoy the snark!

Customization & Extensibility
Quiz Questions: Easily editable in the HTML form.

Match Profiles & Comments: Stored in JavaScript arrays; can add or change entries for more fun.

User Interface: Colors, fonts, and layout can be customized in the CSS block.

Data Persistence: Can be enhanced by adding localStorage or external storage for persistent user tracking.

Additional Features: Possibility to add share buttons, more detailed profile popups, or extra matchmaking “sweetness”/“sourness” scales.

# Screenshots (Add at least 3)
![Screenshot1](Add screenshot 1 here with proper name)
*Add caption explaining what this shows*

![Screenshot2](Add screenshot 2 here with proper name)
*Add caption explaining what this shows*

![Screenshot3](Add screenshot 3 here with proper name)
*Add caption explaining what this shows*

# Diagrams
![Workflow](Add your workflow/architecture diagram here)
*Add caption explaining your workflow*

For Hardware:

# Schematic & Circuit
![Circuit](Add your circuit diagram here)
*Add caption explaining connections*

![Schematic](Add your schematic diagram here)
*Add caption explaining the schematic*

# Build Photos
![Components](Add photo of your components here)
*List out all components shown*

![Build](Add photos of build process here)
*Explain the build steps*

![Final](Add photo of final product here)
*Explain the final build*

### Project Demo
# Video
[Add your demo video link here]
*Explain what the video demonstrates*

# Additional Demos
[Add any extra demo materials/links]

## Team Contributions
- [Name 1]: [Specific contributions]
- [Name 2]: [Specific contributions]
- [Name 3]: [Specific contributions]

---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProjects--25-25?link=https%3A%2F%2Fwww.tinkerhub.org%2Fevents%2FQ2Q1TQKX6Q%2FUseless%2520Projects)



