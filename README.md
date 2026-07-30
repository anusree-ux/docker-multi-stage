# Go Calculator - Docker Multi-Stage Build
## About
A simple Go calculator application created to learn Docker multi-stage builds.

I first containerized the application using a single-stage Docker build. Although the application is small, the Docker image size was 1.29 GB because it included the Go compiler, build tools, source code, and other files used during the build process.
I then created a multi-stage Docker build, where the application is built in one stage and only the compiled executable is copied to a lightweight runtime image.
This reduced the final Docker image size from 1.29 GB to 16.7 MB, a reduction of approximately 98.7%.

## Docker Images

Single-stage image:
1.29 GB

Multi-stage image:
16.7 MB

Image size reduced by ~98.7%.
<img width="1241" height="211" alt="Screenshot 2026-07-30 121255" src="https://github.com/user-attachments/assets/acef7c18-e1b9-4c0b-a90d-75d7f40cd5a9" />
