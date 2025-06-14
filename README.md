# 📸 Instagram Clone - SQL Backend

This project is an **Instagram Clone (Backend Only)** designed to replicate the core functionalities of the Instagram platform using **SQL**. It includes a complete relational database schema that models users, posts, comments, likes, followers, reports, and stories.

## 📂 Project Structure
📁 Instagram-Clone-SQL/
📄 INSTAGRAM_CLONE.sql # Full SQL script with schema definition
📄 README.md # Project overview and documentation

## 🧱 Features Modeled

This database schema captures essential features commonly found in social media platforms like Instagram:

### 👤 Users
- User registration with details: `username`, `email`, `password`, `bio`, `gender`, `profile image`
- Timestamps for account creation and updates

### 📸 Posts
- Users can create posts with:
  - Captions
  - Media (image/video)
  - Timestamps

### 💬 Comments
- Users can comment on any post
- Comment includes text, timestamp, and is linked to both user and post

### ❤️ Likes
- Users can like posts
- Unique constraint to prevent multiple likes on the same post

### 🔁 Followers
- User can follow/unfollow others
- Follower-Following relationships tracked

### 🧾 Reports
- Users can report inappropriate content or accounts
- Includes `report_reason`, target (post/user), and `timestamp`

### 🎯 Stories
- Temporary content shared by users
- Auto-expiration logic modeled via `created_at` timestamp

---

## 🧰 Technologies Used

- ✅ **SQL** (MySQL / MariaDB compatible)
- 🔄 **Relational Database Design**
- 🔗 **Foreign Keys with Cascading Updates/Deletes**
- 🔢 **Auto-Incremented IDs**
- 📅 **DateTime Fields for Timestamps**
- 📚 **Enum Types** for fields like gender or report reason

## 📌 Setup Instructions

1. **Clone the repository** or download the SQL script.
2. Open any MySQL-compatible client (like MySQL Workbench, phpMyAdmin, or CLI).
3. Run the `INSTAGRAM_CLONE.sql` file to create all tables and constraints.

```bash
mysql -u your_username -p your_database < INSTAGRAM_CLONE.sql

📬 Contact
For any questions, collaboration, or suggestions:
📧 varshareddy724@gmail.com
🔗 https://www.linkedin.com/in/varsha-reddy-64a915257/



