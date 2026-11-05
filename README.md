# Library Seat & Resource Booking System

**LPU Project by S.S. Arunesh · Reg. No. 12602508**

A web app for reserving library seats, reading rooms and resources. Students pick a location and time slot on a visual seat map; bookings are recorded and seats are released automatically when the slot ends or when a student doesn't check in within 15 minutes.

Built with plain **HTML, CSS and JavaScript**. There is no framework, build step or backend, and `localStorage` stores the data. The design is strictly monochrome (black, white and greys).

## Features

| Module | What it does |
|---|---|
| Student login | Registration with validation (8-digit reg. no., unique), login, role-based access |
| Visual seat map | 60 seats across Ground Floor – Silent Zone, First Floor – Group Study and Computer Lab, showing available / booked / mine / maintenance |
| Resource availability | Reading rooms, discussion rooms and equipment in a resource × time-slot grid |
| Slot booking | Seven 2-hour slots (08:00–22:00), up to 7 days ahead, with double-booking prevention |
| Booking history | Filters, search, check-in / cancel / release, printable view |
| Automatic seat release | No-show after 15 minutes without check-in; auto-complete when the slot ends |
| Notifications | Notification bell with unread count, toasts and a full notifications page |
| Admin dashboard | Live stats, live seat map with maintenance control, bookings, resources, users and settings |

## Demo logins

| Role | Login | Password |
|---|---|---|
| Student | `12602508` | `student123` |
| Admin | `admin` | `admin123` |

## Run locally

Open `index.html` in a browser, or serve the folder:

```
python -m http.server 8080
```

Then visit `http://localhost:8080`.

## Folder structure

```
index.html  login.html  register.html  notifications.html
student/    dashboard, seat map, resources, history
admin/      admin dashboard
css/        styles
js/         app logic and page scripts
```

Data is stored in each visitor's own browser, so bookings are not shared between devices.
