# AWS Rekognition Image and Video Detection - GitHub Repository

## Overview
This repository demonstrates how to use **AWS Rekognition** for image and video detection. The code files included showcase the integration of AWS Rekognition’s capabilities for analyzing visual content, such as detecting objects, faces, and text in images, as well as processing video for activities and objects.

### Key Features
- **Image Detection**: Uses AWS Rekognition to analyze and detect objects, faces, and text within images.
- **Video Detection**: Analyzes video content to identify objects, scenes, activities, and more.

## Setup Instructions

### Prerequisites:
Before you begin, make sure you have the following:
- **AWS Account**: Set up an AWS account, and ensure you have the required **IAM permissions** to use **AWS Rekognition** and other services.
- **AWS CLI**: Install the AWS Command Line Interface (CLI) on your local machine. Follow the official documentation [here](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html).
- **Boto3 Library**: Install the Boto3 library (AWS SDK for Python) for interacting with AWS services:

  pip install boto3
  
### AWS Services Setup:
- **AWS Rekognition**: Make sure you have an AWS Rekognition service enabled in your AWS account.
- **S3 Bucket**: Create an S3 bucket to upload the input images or videos you want to process. Ensure that the S3 bucket permissions allow the Rekognition service to access the files.
- **IAM Role**: Create an IAM role with sufficient permissions to use Rekognition and access the S3 bucket.
- **AWS Lambda (Optional)**: If you're automating the process or need serverless execution, consider setting up AWS Lambda functions.
- **AWS Free Tier**: AWS Rekognition is available on the AWS Free Tier with 5,000 free images per month. Be aware that after exceeding 5,000 images, you will incur charges. Details on the pricing can be found on AWS Rekognition Pricing.
- **Input Files**:
Make sure to place your image or video files in the local directory and update the path to the input files in the code files accordingly.

### Code Files:
image_detection.py: This script processes images using AWS Rekognition to detect objects, faces, and text.
video_detection.py: This script processes video files to detect objects, scenes, and activities.

### Image Detection:

Update the image_file_path variable in image_detection.py with the path to the image you want to analyze.
Run the script:
python image_detection.py

### Video Detection:
Update the video_file_path variable in video_detection.py with the path to the video file you want to analyze.

Run the script:
python video_detection.py

### Important Notes:
Ensure that the services and IAM roles are set up before running the scripts.
The input image/video files should be available locally. Modify the path to your files in the code as needed.
You can test the solution using an AWS Free Tier account. However, note that only the first 5,000 images are free each month. Additional usage will incur charges. Keep track of your usage to avoid unexpected costs.
### Contributing:
Feel free to fork this repository and contribute by submitting pull requests. Any improvements, bug fixes, or additional features are welcome!

### License:
This project is licensed under the MIT License - see the LICENSE file for details.
