# Ansible-Role
.
├── roles
│   ├── backend
│   │   ├── docker
│   │   │   ├── Dockerfile
│   │   │   └── src
│   │   │       ├── pom.xml
│   │   │       └── src
│   │   │           └── main
│   │   │               ├── java
│   │   │               │   └── com
│   │   │               │       └── example
│   │   │               │           └── backend
│   │   │               │               └── BackendApplication.java
│   │   │               └── resources
│   │   │                   └── application.properties
│   │   └── tasks
│   │       └── main.yml
│   └── frontend
│       ├── docker
│       │   ├── Dockerfile
│       │   └── src
│       │       ├── public
│       │       │   └── index.html
│       │       └── src
│       │           └── App.js
│       └── tasks
│           └── main.yml
└── sites.yml
