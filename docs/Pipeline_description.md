# Pipeline description

The CircleCI pipeline automates the build and deployment process for this project with separate frontend and backend components.

1. Build Job:
    - Sets up the Node.js environment (cimg/node:18.20.5)
    - Installs dependencies and builds both the frontend and backend:
        - Installs Node.js and checks out the code.
        - Installs frontend and backend dependencies using custom npm scripts.
        - Lints and builds the frontend and backend.

At this step, the pipeline waits for manual approval and continues with the deploy job only after that.

2. Deploy Job:
    - Runs in a basic container (cimg/base:stable)
    - Sets up the Node.js environment (cimg/node:18.20.5)
    - Sets up AWS, and Elastic Beanstalk
    - Deploys the built applications to the respective environments using npm scripts
