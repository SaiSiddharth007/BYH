# ByteX HydroHero - Complete Integration

## Components

- Frontend (Next.js, Cognito Auth, Image Upload)
- AWS S3 Integration for image storage
- AWS Lambda ML Inference
- Triggered via S3 Events
- ML Models:
  - plant_health_check.py
  - distance_estimation.py

## Deployment Notes

1. Deploy the Lambda functions using zipped handlers from `ml_models/`
2. Setup S3 trigger to invoke both functions on image upload
3. Ensure `aws-exports.js` is configured properly for Amplify
4. Run frontend via `npm run dev` after setting up AWS credentials

## AWS Config Used:
- Cognito Region: `ap-south-1`
- User Pool ID: `ap-south-1_yO13tiT8x`
- App Client ID: `1aj6j0teuv02qj738u14j2v6dp`
- S3 Bucket: `projectbucketlist`
