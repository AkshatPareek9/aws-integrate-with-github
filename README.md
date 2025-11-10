# Project: AWS Integration with GitHub

This project demonstrates how to integrate a GitHub repository with AWS services (S3) using GitHub Actions for automated deployment.

<img width="378" height="103" alt="image" src="https://github.com/user-attachments/assets/faa6b737-143e-4c32-abac-b3b6bc866606" />

## Steps to Set Up

1. **Create an S3 bucket on AWS**

   * Ensure proper permissions and make it public (if hosting a static website).

2. **Clone the Git repository**

   ```bash
   git clone <your-repo-url>
   cd <repo-name>
   ```

3. **Update GitHub Actions workflow**

   * Edit `.github/workflows/main.yml` to include steps for AWS deployment.

4. **Commit the changes**

   ```bash
   git add .github/workflows/main.yml
   git commit -m "Add AWS S3 deployment workflow"
   git push origin main
   ```

5. **Verify S3 bucket**

   * Check if the files are uploaded correctly.
   * Confirm that the bucket permissions allow access if hosting a website.

6. **Check website** (if hosting static site)

   * Open the S3 bucket URL in a browser.
   * Ensure the website loads correctly.
