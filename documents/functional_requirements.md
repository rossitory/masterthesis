# Functional Requirements Document

## Application: Therapeutic Timeline Builder

### Purpose
The Therapeutic Timeline Builder allows users to document and reflect on significant life events in a private, secure, and supportive interface. Users can add events, attach emotions, and view their timeline, providing a meaningful structure for preparing for therapy.

---

## Functional Requirements

### 1. User Management
- **User Registration**:
  - Allow new users to register with email and password.
  - Ensure passwords are hashed and stored securely.
- **Login and Authentication**:
  - Implement secure login with token-based authentication.
- **Password Management**:
  - Allow users to reset their passwords securely.
  - Implement secure email-based password reset flows with expiration limits.

---

### 2. Timeline Management
- **Timeline View**:
  - Display a horizontal timeline layout.
  - Show individual events as clickable nodes with a title and date.
  - When clicked, nodes expand to reveal additional event details in an overlay or modal.
- **Empty State for Timeline**:
  - Display a welcoming, instructional screen for users with no events.
  - Center an “Add Your First Event” button to guide new users.
 
---

### 3. Event Management
- **Add Event**:
  - Allow users to add a new event to their timeline.
  - Open an entry modal with fields for event title, description, date, and emotion tags.
  - Provide an option to upload an image or media file to visually represent the event. (Maybe)
- **Edit Event**:
  - Allow users to edit previously created events.
  - Changes should be reflected in real-time on the timeline.
- **Delete Event**:
  - Implement a soft-delete functionality (event remains accessible in a “Deleted Events” view) to prevent accidental data loss.

---

### 4. Emotion Tagging
- **Emotion Selection for Events**:
  - Provide users with a selection of predefined emotion tags (e.g., Calm, Sad, Hopeful).
  - Use a Mood Selector with icons and colors associated with each emotion.
- **Custom Emotion Tags** (Probably not):
  - Enable users to create their own custom emotions with selectable colors or icons.

---

### 5. Search and Filter (Maybe)
- **Keyword Search**:
  - Implement a search bar allowing users to search events by keyword, title, or description.
- **Emotion and Date Filters**:
  - Allow users to filter events based on selected emotions or specific date ranges.

---

### 6. Insights and Reflections (Probably not)
- **Emotion Trends**:
  - Display visual summaries of frequently used emotions or patterns over time.
- **Journal Prompts**:
  - Include a system to prompt users with reflection questions based on their recent events or most frequent emotions.

---

### 7. Security and Privacy
- **Data Encryption**:
  - Encrypt sensitive data in transit and at rest.
- **User Anonymity**:
  - Avoid personally identifiable information where possible, aside from necessary account details.
- **Privacy Settings**:
  - Allow users to control the visibility of individual entries (if the application allows sharing).
- **Automatic Logout**:
  - Automatically log users out after a period of inactivity to protect privacy.

---

### 8. Settings and Customization
- **Account Settings** (Maybe):
  - Allow users to update email, password, and profile details.
- **Dark/Light Mode** (Probably not):
  - Offer users the choice between dark and light themes.

---

### 9. Notifications and Reminders (Probably not)
- **Event Reminders**:
  - Allow users to set reminders for important events.
- **Insight Notifications**:
  - Optional push or email notifications about insights on recent activity (e.g., “You’ve added 3 calm events this month”).
- **Weekly/Monthly Reflection**:
  - Send users reminders to review their timeline periodically.

---

### 10. Help and Support
- **Tooltips**:
  - Add tooltips for all major actions, guiding users in completing fields or using features.
- **Help Center/FAQ** (Maybe):
  - Provide an in-app help section with FAQs or tips for using the timeline and other features.
- **Support Contact** (Maybe):
  - include a support contact form for feedback or assistance requests.

---

### 11. Performance and Responsiveness
- **Mobile Optimization**:
  - Ensure that all pages are fully responsive, providing a smooth experience on mobile, tablet, and desktop devices.
- **Real-Time Updates**:
  - Implement real-time updates for changes in the timeline (e.g., adding or editing events).
- **Caching for Speed** (Probably not):
  - Use caching mechanisms for frequently accessed data, especially for large timelines.

---

### 12. Backend & Data Storage Requirements
- **Database Design**:
  - Design a relational database schema for storing user data, events, emotion tags, and other related information.
- **Image Storage** (Maybe):
  - Implement a method for storing or referencing user-uploaded media securely (e.g., cloud storage).
- **Logging and Monitoring**:
  - Set up server logging and monitoring to ensure reliability and help troubleshoot issues.

---

### Optional Features (Future Roadmap)
- **AI-Powered Insights**:
  - Implement AI-based analysis of events to provide deeper insights into user patterns.
- **Event Sharing**:
  - Allow users to share certain events or timelines with therapists or trusted individuals securely.

---
