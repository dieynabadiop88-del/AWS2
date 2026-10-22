# Dieynaba Diop — IT Portfolio

A personal Bootstrap 5 portfolio website for an AWS Amplify hosting assignment.

## Deploy
1. Upload all files and folders to the root of a GitHub repository.
2. In AWS Amplify, choose **Deploy an app** > **GitHub** and authorize access.
3. Select the repository and branch, and deploy.
4. If Amplify requests build settings for this static HTML site, use:

```yaml
version: 1
frontend:
  phases:
    build:
      commands: []
  artifacts:
    baseDirectory: /
    files:
      - '**/*'
  cache:
    paths: []
```

Bootstrap is loaded from a CDN, so the deployed site needs internet access. Replace the illustration in `images/technology.svg` if you prefer a personal photo, and update the HTML image path.
