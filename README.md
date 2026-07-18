# DevOps Intern Final Assessment

![CI](https://github.com/RiyaDominic/devops-intern-final/actions/workflows/ci.yml/badge.svg)

## Name
**Riya Dominic**

## Date
**18 July 2026**

---

# Project Description

This project demonstrates a complete DevOps workflow using open-source tools and cloud-native practices. It includes version control with Git and GitHub, Linux shell scripting, Docker containerization, GitHub Actions for CI/CD, Nomad job deployment configuration, and Grafana Loki logging setup.

---

# Technologies Used

- Git
- GitHub
- Linux Shell
- Docker
- GitHub Actions
- Nomad
- Grafana Loki
- Python 3

---

# Project Structure

```text
devops-intern-final/
│
├── hello.py
├── Dockerfile
├── README.md
│
├── scripts/
│   └── sysinfo.sh
│
├── monitoring/
│   └── loki_setup.txt
│
├── nomad/
│   └── hello.nomad
│
├── screenshots/
│
└── .github/
    └── workflows/
        └── ci.yml
```

---

# Step 1 – Git & GitHub

- Created a public GitHub repository.
- Added README.md.
- Added a simple Python application (`hello.py`).

Run:

```bash
python hello.py
```

Output:

```text
Hello, DevOps!
```

---

# Step 2 – Linux Shell Script

Location:

```text
scripts/sysinfo.sh
```

The script displays:

- Current user
- Current date
- Disk usage

Run:

```bash
chmod +x scripts/sysinfo.sh
./scripts/sysinfo.sh
```

---

# Step 3 – Docker

Build the Docker image:

```bash
docker build -t hello-devops .
```

Run the container:

```bash
docker run --rm hello-devops
```

Output:

```text
Hello, DevOps!
```

---

# Step 4 – GitHub Actions (CI/CD)

Workflow file:

```text
.github/workflows/ci.yml
```

The workflow automatically:

- Checks out the repository
- Installs Python
- Runs `hello.py`

It executes automatically on every push to the `main` branch.

---

# Step 5 – Nomad Deployment

Nomad configuration:

```text
nomad/hello.nomad
```

Example command:

```bash
nomad job run nomad/hello.nomad
```

---

# Step 6 – Grafana Loki

Loki setup documentation:

```text
monitoring/loki_setup.txt
```

Start Loki:

```bash
docker run -d --name loki -p 3100:3100 grafana/loki:3.0.0
```

Verify:

```text
http://localhost:3100/ready
```

Expected response:

```text
ready
```

View logs:

```bash
docker logs loki
```

---

---

# Repository

GitHub Repository:

**https://github.com/RiyaDominic/devops-intern-final**

---

## Author

**Riya Dominic**

