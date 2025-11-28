# CloudWatch Dashboard – Serverless Project

Mini dashboard that displays simulated CPU metrics using AWS Lambda, CloudWatch and S3.

## Architecture
EventBridge (1 min) → Lambda → CloudWatch Metrics → Dashboard → S3 (Web)

## Deployed Resources
- Lambda `envia-metricas` (Python 3.12)
- EventBridge rule every 1 min
- CloudWatch custom metric `CPUUtilization`
- S3 static website with dashboard link

## Cost
≈ 0.03 USD/month within the Free Tier.

## How to test
1. Open the dashboard:  
   https://us-east-1.console.aws.amazon.com/cloudwatch/home?region=us-east-1#dashboards:name=MiDashboard
2. Or visit the website:  
   http://mis-dashboard-123-456.s3-website-us-east-1.amazonaws.com

## Tech Stack
- Python
- AWS SAM (optional)
- HTML / CSS

## License
MIT

