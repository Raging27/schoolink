# Schoolink

**A role-based communication and grade-management platform connecting teachers and parents.**

Schoolink was built by a four-person team during Le Wagon's full-stack web development bootcamp. Teachers can manage student results and communicate with parents, while parents receive a focused view of grades, exam documents, and conversations.

## Product overview

| Teacher workflow | Parent workflow |
| --- | --- |
| View assigned classes and students | View linked children and results |
| Add grades and exam information | Review grades, averages, and feedback |
| Share exam documents | Access uploaded exam material |
| Start direct conversations with parents | Contact the relevant teachers |

## Engineering highlights

- Separate teacher and parent experiences using role-aware Rails routes and user types
- Authentication and account recovery with Devise
- Relational domain model covering users, sections, courses, grades, chatrooms, and messages
- Direct teacher-parent messaging with read-state tracking
- File and image handling through Active Storage and Cloudinary
- Team delivery using feature branches and pull requests

## Stack

- Ruby 3.1.2 and Rails 7.1
- PostgreSQL
- Hotwire: Turbo and Stimulus
- Devise
- Active Storage and Cloudinary
- Bootstrap 5, HTML, CSS, and JavaScript
- Heroku

## Screenshots

### Teacher dashboard

![Schoolink teacher dashboard](https://github.com/Raging27/schoolink/assets/100428479/19231ed5-e186-4abe-96ec-09a7b68301cb)

### Teacher-parent messaging

![Schoolink chat](https://github.com/Raging27/schoolink/assets/100428479/db58ebb6-3012-4a15-9f48-8c40678c9c45)

### Class averages

![Schoolink class averages](https://github.com/Raging27/schoolink/assets/100428479/74a5a16f-5a33-415d-83c7-7f7e12e652a4)

### Grade details

![Schoolink grade details](https://github.com/Raging27/schoolink/assets/100428479/f704101e-65f2-48bb-a75d-a13e2715005f)

## Run locally

### Requirements

- Ruby 3.1.2
- PostgreSQL

### Setup

```bash
git clone https://github.com/Raging27/schoolink.git
cd schoolink
bundle install
bin/rails db:create db:migrate db:seed
bin/rails server
```

Open `http://localhost:3000`.

Environment variables may be required for Cloudinary-backed media.

## Team

- Olivia Rochat
- Omar Haizoun
- Mustafa Arslan
- Ronan Kervella

Built during [Le Wagon](https://www.lewagon.com).
