♻️ THE ROCK WASTE MANAGEMENT

THE ROCK WASTE MANAGEMENT is a smart web-based platform designed to digitalize and streamline waste collection and cleaning services. The system connects customers, workers, and administrators to ensure efficient service booking, management, and tracking — reducing manual processes and improving environmental cleanliness.

🌍 Overview

The Rock Waste Management System allows:

Customers to book waste cleaning services quickly and conveniently.

Admins to manage customers, workers, and bookings from a central dashboard.

Workers to view assigned tasks and update their progress (e.g., Attending, Done).

The platform also integrates with Firebase Firestore for real-time data management and Firebase Authentication for secure user access.

🧠 Key Features
👥 Customer

Register and log in securely.

Book cleaning services (e.g., bin collection, street cleaning).

Choose preferred date, time, and location (Google Maps integrated).

View booking history and payment status.

Receive booking confirmation and status updates.

🧹 Worker

Login to access a personal dashboard showing assigned bookings.

Update task status (Attending, Done).

Send feedback or completion notes to the admin.

🧑‍💼 Admin

Manage customers, workers, and bookings.

Approve, reject, or delete bookings.

Assign workers to bookings.

Set or update service pricing.

View payment status and booking analytics.

⚙️ Tech Stack
Component	Technology Used
Frontend	ASP.NET Razor Pages / MVC
Backend	C# (.NET Framework)
Database	Firebase Firestore
Authentication	Firebase Authentication
Cloud Platform	Google Firebase
Version Control	Git & GitHub
IDE	Visual Studio 2022
🧩 System Modules

User Authentication (Admin, Worker, Customer)

Booking Management (CRUD operations)

Worker Assignment and Dashboard

Admin Dashboard with Controls

Customer Booking Page with Google Maps

Email Confirmation System (for bookings)

Payment and Pricing Management

🗄️ Firestore Database Structure
users
 ┗━ userId
     ┣━ name
     ┣━ role (admin / worker / customer)
     ┣━ email
     ┗━ status (active / disabled)

bookings
 ┗━ bookingId
     ┣━ CustomerName
     ┣━ CustomerId
     ┣━ BookingAddress
     ┣━ BookingDate
     ┣━ PreferredTime
     ┣━ ServiceType
     ┣━ AssignedWorker
     ┣━ Status (Pending, Approved, Rejected, Completed)
     ┣━ EstimatedPrice
     ┣━ FinalPrice
     ┣━ PaymentStatus
     ┗━ CreatedAt

workers
 ┗━ workerId
     ┣━ name
     ┣━ email
     ┣━ phone
     ┣━ status (approved/pending)
     ┗━ assignedBookings

🧪 How to Run Locally
🖥️ Prerequisites

Visual Studio (2022 or later)

.NET SDK installed

Firebase Project setup

Active Internet Connection

⚙️ Setup Steps

Clone the repository:

git clone https://github.com/yourusername/TheRockWasteManagement.git


Open the project in Visual Studio.

Add your Firebase credentials in appsettings.json or configuration file.

Run the project using IIS Express or dotnet run.

Access it on https://localhost:xxxx/.

🧭 Pages Overview
Page	Description
/Home	Landing page with service info
/Register	Customer/Worker registration
/Login	Login for all users
/BookCleaning	Customer service booking
/Admin/Dashboard	Admin management dashboard
/Worker/Dashboard	Worker assigned bookings
/Admin/ManageUsers	Manage customer/worker accounts
/Admin/ManageBookings	Approve/reject/set prices for bookings
🚀 Future Enhancements

Online payment integration.

Automated worker scheduling.

Push notifications via Firebase Cloud Messaging.

Reports and analytics dashboard for admins.

Mobile-friendly responsive design improvements.

🧑‍💻 Contributors
Name	Role
Mulongoni Washu	Lead Developer (System Design, Firebase Integration, Web Development)
Maredi William Semenya(Business Analyst)
Sandile Wellcome Nkosi(System Analyst)

Team Members	UI Design, Database Design, and Testing
📜 License

This project is licensed under the MIT License — you are free to use, modify, and distribute it with proper attribution.
