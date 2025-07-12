# StackIt - Odoo Hackathon Project

🌐 Live Demo https://theycotes.com/Stackit/project%202/index.php

/StackIt
│
├── api/
│   ├── accept_answer.php            # Marks an answer as accepted
│   ├── get_question_from_answer.php # Fetch question from answer
│   ├── notifications.php            # Notification handler (fetch/send)
│   ├── vote.php                     # Upvote/downvote handler
│
├── assets/
│   ├── css/
│   │   └── style.css                # All page styling
│   ├── js/
│   │   └── main.js                  # Voting, notifications, AJAX
│
├── config/
│   └── database.php                 # DB connection settings
│
├── includes/
│   ├── auth.php                     # Session & auth checker
│   └── functions.php                # Reusable utility functions
│
├── sqlquery/
│   └── 20250712090052_rustic_snow.sql # Sample backup or seed query
│
├── uploads/
│   └── [uploaded images]           # User-uploaded images (from rich text)
│
├── admin.php                        # Admin control panel
├── admin2.php                       # Secondary admin functions
├── ask.php                          # Page to ask a new question
├── index.php                        # Homepage with all questions
├── login.php                        # User login form
├── logout.php                       # Logout and session destroy
├── profile.php                      # User profile and activity
├── question.php                     # View a single question and its answers
├── register.php                     # User registration form
├── upload_image.php                 # Handles image uploads via editor
├── u564191134_stackk.sql            # MySQL dump of the full database
├── project 2 (1).zip                # Optional: zipped version of project
├── README.md                        # This documentation file


## 🧑‍💻 Tech Stack

This project uses a simple but effective stack of core web technologies:

- **Language**: PHP (Core PHP)
- **Database**: MySQL
- **Frontend**: HTML, CSS, JavaScript
- **Rich Text Editor**: TinyMCE or CKEditor (for Q/A formatting)
- **Authentication**: PHP Sessions
- **Notifications**: AJAX-based polling system

---

## ✨ Key Features

- 📝 **Ask Questions** – Title, rich-text description, and multiple tags
- 🧾 **Answer Questions** – Users can post rich-formatted answers
- 👍 **Voting** – Upvote or downvote helpful/unhelpful answers
- ✅ **Accept Answers** – Mark the best answer for your question
- 🏷️ **Tagging System** – Assign multiple tags to categorize questions

### 🔔 Notification System
Users receive real-time updates when:
- Someone answers their question
- Someone comments on their answer
- Someone mentions them using `@username`

---

## 🔐 Authentication Flow

Authentication is handled using PHP sessions and protected access logic:

- `register.php` – User signup form
- `login.php` – Starts user session and stores ID
- `logout.php` – Destroys session and logs user out
- `includes/auth.php` – Middleware to protect pages from unauthorized access
- `admin.php`, `admin2.php` – Admin-only access for moderation tasks

---
