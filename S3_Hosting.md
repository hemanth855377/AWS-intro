Hosting a Static Website on Amazon S3

Amazon S3 (Simple Storage Service) is not only used for storing files but also for hosting static websites. Static means websites built with HTML, CSS, and JavaScript (without server-side code like PHP or databases).

This feature is very useful for beginners to quickly deploy a website at low cost.

🔹 Steps to Host a Website on S3
1. Create an S3 Bucket

Go to AWS Console → S3 → Create bucket.

Bucket name must be unique (example: my-demo-website).

Select a region (like ap-south-1 for Mumbai).

Keep default settings → Click Create bucket.

2. Enable Static Website Hosting

Open your bucket → Go to Properties tab.

Scroll down to Static website hosting.

Choose Enable, select Host a static website.

Enter index.html as the homepage file.

Copy the Endpoint URL (this is your website link).

3. Upload Website Files

Go to the Objects tab inside the bucket.

Upload your files (index.html, style.css, etc.).

After upload, they will be stored in S3.

4. Set Permissions (Public Access)

By default, S3 buckets are private. To make the website accessible:

Go to Permissions → Bucket Policy.

Add this policy (replace my-demo-website with your bucket name):

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::my-demo-website/*"
    }
  ]
}


This policy allows everyone to read the website files.

5. Access the Website

Copy the S3 Endpoint URL from the bucket’s Static website hosting section.

Open it in your browser.

🎉 Your static website is live!.

