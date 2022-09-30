# upload-lambda-artifact-gh-action

```yaml
      - name: Upload shared lambda layer artifact
        uses: ohpensource/upload-lambda-artifact-gh-action@main
        with:
          region: $AWS_REGION
          access-key: ${{ secrets.AWS_ACCESS_KEY_ID }}
          secret-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
          role-name: $AWS_ASSUME_ROLE_NAME
          version: "v0.0.1"
          service-name: "YOUR_SERVICE_NAME"
          function-project-name: "app-name"
          artifact-folder: "folder where the artifact is stored"
          account: "aws account id where the s3 bucket is located"
          s3-bucket: "s3 bucket name"
```
