# Project Management System

## Project Management System is an application designed to assist in managing projects, the employees involved in those projects, as well as keeping track of working hours and user attendance within the system.

https://github.com/AdnanPobrklic/project-managment/assets/109630160/1ab74496-b3cc-451e-85fb-a409155e1c00

## Key Features

- **Various Roles:**
    - Administrator: Real-time system activity overview.
    - Managers: Creation and management of projects, teams, and tasks, as well as monitoring working hours and attendance.
    - Workers: Execution of assigned tasks, input of working hours.

- **Project Management:**
    - Addition and tracking of projects.
    - Formation of teams with defined leaders and members.

- **Tasks and Workers:**
    - Addition of tasks to projects with assignment to specific workers.
    - Input and tracking of completed tasks.

- **Attendance and Status:**
    - Monitoring attendance of all online and offline users and the time they were present.
    - Tracking user status.

- **Real-time Communication:**
    - Real-time notifications.
    - Ability to use chat for communication between users.

- **Sending Notifications:**
    - Sending notifications via email for important information and updates.

- **Report Generation:**
    - Generating PDF reports with data on working hours and attendance by users and projects.
    - Ability to download and send them via email.

## Project Architecture

```
└── 📁
    └── .gitignore
    └── License.md
    └── README.md
    └── 📁controllers
        └── chatControllers.js
        └── korisnikControllers.js
        └── prijavaControllers.js
        └── projectControllers.js
        └── radnaPovrsinaControllers.js
    └── 📁models
        └── Aktivnost.js
        └── Attendance.js
        └── Chat.js
        └── Korisnik.js
        └── Obavjesti.js
        └── Projekat.js
        └── Sessions.js
    └── package-lock.json
    └── package.json
    └── 📁public
        └── 📁css
            └── 404.css
            └── aktivnosti.css
            └── chat.css
            └── dodaj-projekat.css
            └── dodaj-radnika.css
            └── header.css
            └── pocetna.css
            └── prijava.css
            └── projekat-detalji.css
            └── radna-povrsina.css
            └── style.css
            └── table-page.css
            └── unos-zadatka.css
            └── uredi-page.css
            └── zadatak-detalji.css
        └── 📁img
            └── 404shortcuticon.png
            └── add-task.png
            └── attendance.png
            └── blueprint.png
            └── broom.png
            └── clipboard.png
            └── contact-list.png
            └── error-404.png
            └── new-chat.png
            └── notification-p-icon.png
            └── notification.png
            └── paper-plane.png
            └── prijava-bg.svg
            └── prijavashortcuticon.png
            └── radna-povrsinashortcuticon.png
            └── system-activity.png
            └── user.png
        └── 📁js
            └── aktivnosti.js
            └── chat-frontend.js
            └── dodaj-projekat.js
            └── dodaj-radnika.js
            └── dodaj-zadatak.js
            └── header.js
            └── korisnik-uredi.js
            └── prijava.js
            └── projekat-detalji.js
            └── projekat-uredi.js
            └── script.js
            └── table-page.js
            └── unos-zadatka.js
    └── 📁routes
        └── chatRoutes.js
        └── korisnikRoutes.js
        └── prijavaRoutes.js
        └── projectRoutes.js
        └── radnaPovrsinaRoutes.js
    └── server.js
    └── 📁service
        └── 📁fonts
            └── Roboto-Bold.ttf
            └── Roboto-Medium.ttf
        └── mail-transporter.js
        └── pdf-service.js
    └── 📁sockets
        └── socketManager.js
    └── 📁views
        └── 404.ejs
        └── aktivnosti.ejs
        └── chat.ejs
        └── dodaj-korisnika.ejs
        └── dodaj-projekat.ejs
        └── dodaj-zadatak.ejs
        └── korisnik-uredi.ejs
        └── moji-zadaci.ejs
        └── 📁partials
            └── chat-user-list.ejs
            └── head.ejs
            └── header.ejs
            └── radna-povrsina-links.ejs
        └── pocetna.ejs
        └── prijava.ejs
        └── prisustvoRadnika.ejs
        └── projekat-detalji.ejs
        └── projekat-uredi.ejs
        └── projekatRV.ejs
        └── radnikRV.ejs
        └── svi-korisnici.ejs
        └── svi-projekti.ejs
        └── unos-zadatka.ejs
        └── zadatak-detalji.ejs
```
## Installation

1. Install necessary modules: `npm install`

## Configuration

- Adjust the `.env` file to contain

    1. DBURI=mongoose_uri (if not provided, localhost will be used)
    2. PORT=number (if not provided, 3000 will be used)
    3. SESSION_SECRET=secret
    4. EMAIL=email
    5. EMAIL_PW=email_password

## Running

1. Start the application: `npm start`
2. The application will be available at http://localhost:3000/

## Resources

The following resources were used for this application:

- **Icons**
    1. [Font Awesome](https://fontawesome.com/)
    2. [Flaticon](https://www.flaticon.com/)

- **Background image**
    1. [Haikei](https://app.haikei.app/)
