
## Ideation

GitHub Project Management: https://github.com/orgs/sagufoundation/projects/5

ChatGPT: https://chatgpt.com/share/6968f9ce-9158-800e-b7bd-3e137bcb40ea

Demo GitHub Pages: https://sagufoundation.github.io/connect-online-registration-prototype/

users
```bash
    users
    ├── id (bigint, PK)
    ├── full_name (string)
    ├── gender (enum: male, female, other)
    ├── phone (string, nullable)
    ├── email (string, unique)
    ├── password (string)
    ├── is_active (boolean, default true)
    ├── email_verified_at (timestamp, nullable)
    ├── remember_token (string, nullable)
    ├── created_at
    └── updated_at

```

roles
```bash
    roles
    ├── id
    ├── name (admin, instructor, student)
    ├── guard_name (web)
    ├── created_at
    └── updated_at

```

permission
```bash
    permissions
    ├── id
    ├── name (create-course, edit-course, etc)
    ├── guard_name
    ├── created_at
    └── updated_at

```

programs
```bash
    programs
    ├── id
    ├── program_name
    ├── description
    ├── is_active (boolean)
    ├── created_at
    └── updated_at

```

courses
```bash
    courses
    ├── id
    ├── program_id (FK)
    ├── course_name
    ├── description
    ├── is_active (boolean)
    ├── created_at
    └── updated_at

```