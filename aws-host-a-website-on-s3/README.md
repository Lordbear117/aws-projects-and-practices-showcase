# Host a Website on Amazon S3

This guide provides step-by-step instructions to host a static website using Amazon S3.

## Prerequisites

- An AWS account
- Basic knowledge of AWS S3

## Steps to Host a Website

### 1. Create an S3 Bucket

- Log in to your AWS Management Console.
- Navigate to **S3**.
- Click on **Create Bucket**.
- Enter a unique bucket name (e.g., `your-website-name`).
- Select the AWS Region.
- Uncheck "Block all public access" to allow public access.
- Click **Create Bucket**.

### 2. Upload Website Files

- Open your newly created bucket.
- Click on **Upload**.
- Add your `index.html` file and any other project files (e.g., CSS, JavaScript).
- Click **Upload** to finish.

### 3. Configure Bucket for Static Website Hosting

- Go to the **Properties** tab of your bucket.
- Scroll to **Static website hosting**.
- Select **Use this bucket to host a website**.
- Enter `index.html` as the **Index document**.
- Save changes.

### 4. Set Permissions Using ACL

- Navigate to the **Permissions** tab.
- Click on **Access Control List**.
- Under **Public Access**, check the box for **Everyone** next to **List** and **Read** permissions to allow public access.
- Save your changes.

### 5. Access Your Website

- Go to the **Properties** tab.
- Find the **Bucket website endpoint** URL.
- Visit this URL in your browser to view your website.

## Conclusion

You've successfully hosted a static website on Amazon S3 using ACL! For further customization and features, explore the AWS documentation on S3.

## License

This project is licensed under the MIT License.
