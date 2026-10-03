# S3 Static Website Hosting

A static website deployed on Amazon S3 using S3 static website hosting (region: us-east-2).

## Architecture
- S3 bucket with static website hosting enabled
- `index.html` configured as the index document, served via the S3 website endpoint

## What I learned
- Configuring S3 static website hosting and the index document setting
- S3 object keys are exact and case-sensitive — `index.html` and `index.html.txt` are different objects
- Troubleshooting a `NoSuchKey` 404: my file had been saved as `index.html.txt` because
Windows hides file extensions by default; fixed by renaming and re-uploading with the exact key

## Live site
http://souhail585768187948.s3-website.us-east-2.amazonaws.com/
