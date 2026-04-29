# Flow Diagram

## User Journey

1. User Signup/Login
2. Browse Courses
3. Purchase Course (Razorpay)
4. Access Course
5. Watch Video (S3 streaming)
6. Attempt Quiz

## Payment Flow
Frontend → Backend → Razorpay Order API  
Razorpay → Success Callback → Backend verifies → DB update

## Video Flow
Frontend → Backend (get signed URL) → S3 → Stream video
