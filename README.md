<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>CloudForge CI/CD Lab</title>

  <style>
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu;
      line-height: 1.75;
      color: #1f2937;
      max-width: 960px;
      margin: auto;
      padding: 24px;
      background-color: #ffffff;
    }

    h1 {
      font-size: 2.6rem;
      border-bottom: 4px solid #2563eb;
      padding-bottom: 12px;
      margin-bottom: 1.5rem;
    }

    h2 {
      font-size: 2rem;
      margin-top: 3rem;
      border-left: 6px solid #2563eb;
      padding-left: 12px;
    }

    h3 {
      font-size: 1.4rem;
      margin-top: 1.8rem;
    }

    p {
      margin-top: 1rem;
    }

    ul {
      margin-left: 24px;
    }

    li {
      margin-bottom: 8px;
    }

    code {
      background: #0f172a;
      color: #e5e7eb;
      padding: 4px 6px;
      border-radius: 6px;
    }

    pre {
      background: #0f172a;
      color: #e5e7eb;
      padding: 16px;
      border-radius: 10px;
      overflow-x: auto;
      margin-top: 12px;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 16px;
    }

    th, td {
      border: 1px solid #e5e7eb;
      padding: 12px;
      text-align: left;
    }

    th {
      background-color: #f1f5f9;
    }

    .badge {
      display: inline-block;
      background: #2563eb;
      color: #ffffff;
      padding: 6px 12px;
      border-radius: 999px;
      font-size: 0.8rem;
      margin-right: 6px;
      margin-top: 8px;
    }

    hr {
      margin: 3rem 0;
      border: none;
      border-top: 1px solid #e5e7eb;
    }
  </style>
</head>

<body>

<h1>🚀 CloudForge CI/CD Lab</h1>

<h3>Production-Grade Full-Stack DevOps Pipeline with Node.js, Docker & Kubernetes</h3>

<div>
  <span class="badge">DevOps</span>
  <span class="badge">CI/CD</span>
  <span class="badge">Docker</span>
  <span class="badge">Kubernetes</span>
  <span class="badge">Node.js</span>
  <span class="badge">GitHub Actions</span>
</div>

<hr />

<h2>📌 Project Overview</h2>

<p>
<strong>CloudForge CI/CD Lab</strong> is a production-grade DevOps project that demonstrates
how modern engineering teams design, build, test, containerize, and deploy applications
using industry-standard DevOps practices.
</p>

<p>
The project implements a complete CI/CD pipeline using
<strong>GitHub Actions, Docker, and Kubernetes</strong>, following real-world workflows used
in cloud-native production environments.
</p>

<hr />

<h2>🎯 Project Objectives</h2>

<ul>
  <li>Build a production-ready Node.js application</li>
  <li>Implement automated testing and linting</li>
  <li>Create secure Docker images using best practices</li>
  <li>Automate CI/CD using GitHub Actions</li>
  <li>Deploy to Kubernetes (staging and production)</li>
  <li>Apply real-world DevOps branching strategies</li>
</ul>

<hr />

<h2>🧱 Technology Stack</h2>

<table>
  <tr><th>Layer</th><th>Technology</th></tr>
  <tr><td>Language</td><td>Node.js (v20 LTS)</td></tr>
  <tr><td>Version Control</td><td>Git & GitHub</td></tr>
  <tr><td>CI/CD</td><td>GitHub Actions</td></tr>
  <tr><td>Containerization</td><td>Docker</td></tr>
  <tr><td>Local Orchestration</td><td>Docker Compose</td></tr>
  <tr><td>Production Orchestration</td><td>Kubernetes</td></tr>
  <tr><td>Testing</td><td>Jest, Supertest</td></tr>
  <tr><td>Code Quality</td><td>ESLint</td></tr>
  <tr><td>Security</td><td>Trivy</td></tr>
  <tr><td>Editor</td><td>VS Code</td></tr>
</table>

<hr />

<h2>🗂️ Repository Structure</h2>

<pre>
cloudforge-ci-cd-lab/
├── .github/workflows/ci.yml
├── app.js
├── tests/app.test.js
├── k8s/
│   ├── staging/deployment.yml
│   └── production/deployment.yml
├── Dockerfile
├── docker-compose.yml
├── package.json
├── jest.config.js
├── .eslintrc.js
├── .gitignore
├── .dockerignore
├── .env.example
└── README.md
</pre>

<hr />

<h2>🔹 Step 0: Prerequisites</h2>

<ul>
  <li>Node.js v18+ or v20 LTS</li>
  <li>Git (latest version)</li>
  <li>Docker Desktop</li>
  <li>GitHub account</li>
  <li>VS Code</li>
</ul>

<pre>
node --version
npm --version
git --version
docker --version
</pre>

<hr />

<h2>🔹 Step 1: Version Control Setup</h2>

<p>
Configure Git identity and initialize the repository.
</p>

<pre>
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main

mkdir cloudforge-ci-cd-lab
cd cloudforge-ci-cd-lab
git init
</pre>

<hr />

<h2>🔹 Step 2: Application Development</h2>

<p>
A production-grade Node.js HTTP service featuring:
</p>

<ul>
  <li>Health checks for Kubernetes</li>
  <li>Prometheus-style metrics</li>
  <li>Runtime system information</li>
  <li>Graceful shutdown handling</li>
  <li>Security headers</li>
</ul>

<hr />

<h2>🔹 Step 3: Automated Testing</h2>

<p>
Automated tests ensure application correctness on every commit.
</p>

<pre>
npm test
</pre>

<hr />

<h2>🔹 Step 4: CI/CD Pipeline</h2>

<p>
The GitHub Actions pipeline performs:
</p>

<ul>
  <li>Multi-version Node.js testing</li>
  <li>Lint enforcement</li>
  <li>Dependency security audits</li>
  <li>Docker image builds and pushes</li>
  <li>Container vulnerability scanning (Trivy)</li>
</ul>

<hr />

<h2>🔹 Step 5: Docker Containerization</h2>

<pre>
docker build -t cloudforge-app .
docker run -p 3000:3000 cloudforge-app
</pre>

<p>
The Dockerfile follows best practices:
</p>

<ul>
  <li>Multi-stage builds</li>
  <li>Non-root execution</li>
  <li>Health checks</li>
  <li>Proper signal handling</li>
</ul>

<hr />

<h2>🔹 Step 6: Configuration Management</h2>

<p>
Configuration files ensure clean repositories and secure environments:
</p>

<ul>
  <li>.gitignore</li>
  <li>.dockerignore</li>
  <li>.env.example</li>
  <li>.eslintrc.js</li>
</ul>

<hr />

<h2>🔹 Step 7: Local Development with Docker Compose</h2>

<pre>
docker-compose up -d
</pre>

<hr />

<h2>🔹 Step 8: Local Validation</h2>

<pre>
curl http://localhost:3000/
curl http://localhost:3000/health
curl http://localhost:3000/info
curl http://localhost:3000/metrics
</pre>

<hr />

<h2>🔹 Step 9: GitHub Integration</h2>

<pre>
git add .
git commit -m "Initial commit: CloudForge CI/CD Lab"
git branch -M main
git push -u origin main
</pre>

<hr />

<h2>🔹 Step 10: Kubernetes Deployment</h2>

<p>
The application is deployed to Kubernetes with:
</p>

<ul>
  <li>Separate staging and production environments</li>
  <li>Liveness and readiness probes</li>
  <li>Resource requests and limits</li>
  <li>Rolling updates</li>
</ul>

<hr />

<h2>🔹 Step 11: Release & Branching Strategy</h2>

<table>
  <tr><th>Branch</th><th>Behavior</th></tr>
  <tr><td>develop</td><td>Automatic deployment to staging</td></tr>
  <tr><td>main</td><td>Automatic deployment to production</td></tr>
  <tr><td>Pull Request</td><td>Tests only (no deployment)</td></tr>
</table>

<hr />

<h2>🧪 Troubleshooting</h2>

<ul>
  <li><strong>npm test fails</strong> → Run <code>npm install</code></li>
  <li><strong>Docker build fails</strong> → Ensure Docker Desktop is running</li>
  <li><strong>CI pipeline fails</strong> → Check GitHub Actions logs</li>
  <li><strong>Port 3000 in use</strong> → Stop other Node processes</li>
  <li><strong>ESLint not found</strong> → Install dev dependencies</li>
</ul>

<hr />

<h2>🏁 Conclusion</h2>

<p>
<strong>CloudForge CI/CD Lab</strong> demonstrates a complete DevOps lifecycle from development
to production and serves as a portfolio-ready reference implementation for modern DevOps
engineering practices.
</p>

</body>
</html>

