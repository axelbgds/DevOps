## GitLab CI/CD Pipeline

This project uses GitLab CI/CD for automated building, testing, and deployment. The pipeline is defined in the `.gitlab-ci.yml` file.

### Pipeline Stages

Our pipeline consists of the following stages:

1. Build: Builds the Docker image
2. Test: Runs tests on the built image
3. Release: Tags and pushes the image to the GitLab Container Registry
4. Deploy: Deploys the image to different environments (review, staging, production)
5. Validate: Validates the deployment

### Setting Up the Pipeline

To set up the pipeline:

1. Ensure you have a GitLab account and have created a new project.
2. Push your code to the GitLab repository, including the `.gitlab-ci.yml` file.
3. In your GitLab project, go to "Settings" > "CI/CD" > "Runners".
4. Set up a GitLab Runner for your project. You can use a shared runner provided by GitLab or set up your own runner.

### Running the Pipeline

The pipeline will automatically run when you push changes to your repository. You can view the pipeline's progress and results in the GitLab CI/CD interface:

1. In your GitLab project, go to "CI/CD" > "Pipelines".
2. You'll see a list of pipeline runs. Click on a pipeline to see its details.
3. You can view the status of each job and stage, and access logs for troubleshooting.

### Environment Variables

Make sure to set up the following environment variables in your GitLab project (Settings > CI/CD > Variables):

- `CI_REGISTRY`: Your GitLab Container Registry URL
- `CI_REGISTRY_USER`: Your GitLab username
- `CI_REGISTRY_PASSWORD`: Your GitLab personal access token with registry access

### Docker Compose for Local Development

For local development and testing, you can use the provided `docker-compose.yml` file to set up a local GitLab runner:

```bash
docker-compose up -d