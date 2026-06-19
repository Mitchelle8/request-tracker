# PhotoMed Request Tracker

A simple and responsive web-based request tracking application built using HTML, Tailwind CSS, and JavaScript. The application allows users to submit requests, feedback, issues, and ideas while providing tools to manage, filter, and track their status.

This project was developed as part of the PhotoMed Software Engineering Attachment Assessment.

---

## Live Demo

🔗 [https://request-tracker.mchlladhis.workers.dev](https://request-tracker.mchlladhis.workers.dev)

---

## GitHub Repository

🔗 [https://github.com/Mitchelle8/request-tracker](https://github.com/Mitchelle8/request-tracker)

---

## Features

### Request Submission
Users can submit requests by providing:
- Full Name
- Email Address
- Product / Service
- Request Type
- Priority Level
- Detailed Message

### Request Management
Each submitted request is automatically assigned a status of **New** and can later be updated to:
- New
- In Review
- Resolved
- Rejected

### Filtering
Users can filter requests by:
- Status
- Priority

### Dashboard Statistics
The system automatically displays:
- Total Requests
- New Requests
- Requests In Review
- Resolved Requests

### Data Persistence
Requests are stored using browser localStorage, ensuring data remains available after refreshing the page.

### CSV Export
Users can export all submitted requests into a CSV file for reporting or further analysis.

### Responsive User Interface
The application is fully responsive and works across desktop, tablet, and mobile devices.

### User Experience Enhancements
- Toast notification after successful submission
- Empty-state display when no requests exist
- Modern card-based request layout
- Responsive dashboard design

---

## Technologies Used

## Tech Stack

### Frontend
- HTML5
- Tailwind CSS
- JavaScript (ES6)

### Storage
- LocalStorage
  
### Deployment
- Cloudflare Pages 

---

## Project Structure

```text
PhotoMed-Request-Tracker/
│
├── index.html
└── README.md
```
---

## How to Run Locally

### Option 1: Open Directly

1. Clone the repository:
```bash
git clone [https://github.com/Mitchelle8/request-tracker.git](https://github.com/Mitchelle8/request-tracker.git)
```
Navigate to the project folder.

```Bash
cd request-tracker
```
Open index.html in your preferred web browser.

No additional installation or setup is required.

# How the Application Works

-  User fills out the request form.

- Request data is validated.

- Request is saved to localStorage.

- Request immediately appears in the request list.

- Status can be updated using the status dropdown.

- Requests can be filtered by status or priority.

- Dashboard statistics update automatically.

- Data remains available after page refresh.

- Requests can be exported as a CSV file.

---

## Assessment Requirements Completed

### Core Features
- [x] Submit requests via form interface
- [x] Capture Name, Email, Product, Type, Priority, and Message
- [x] Display requests dynamically on a dashboard
- [x] Manage request statuses (New, In Review, Resolved, Rejected)
- [x] Filter requests by Status and Priority
- [x] Persist data using browser `localStorage`
- [x] Fully responsive mobile-friendly interface

### Bonus Features
- [x] Live metrics dashboard counter
- [x] Toast notification on successful form submission
- [x] Client-side CSV data export engine
- [x] Clean empty-state display when no data exists

---

## Challenges Faced & Solutions

- **The Challenge:** Keeping the UI layout, dashboard metrics, and active filters perfectly synchronized with `localStorage` whenever a card's status was changed in real time.
- **The Solution:** Created a centralized rendering pipeline function. Whenever data changes, it updates `localStorage` first, then runs the data through the active filters and updates the entire dashboard view and stats simultaneously.

---

## Future Improvements

1. **Database Integration:** Move from `localStorage` to a persistent database like Cloudflare D1.
2. **Authentication:** Add a secure admin login portal to protect the request management actions.
3. **Global Search:** Add a real-time text filter bar to search records by name or email strings instantly.

---

## AI Usage Disclosure

AI tools were used to assist with debugging, optimizing Tailwind utility classes, and structuring code logic. All suggestions were fully reviewed, tested, and thoroughly understood before integration into the final application.

---

## Author

**Mitchelle Omondi**  
Software Engineering Attachment Assessment Submission (2026)  

---

## License

This project was developed strictly for assessment performance evaluations under PhotoMed recruitment criteria.
