# AWS-COST-OPTIMIZATION

## <ins>Overview of Project:</ins>
This project is an AWS Lambda function designed to automatically manage and clean up unused Elastic Block Store (EBS) snapshots to reduce storage costs and clutter. It operates by identifying and deleting snapshots that meet specific criteria indicating they are no longer needed:
1) Snapshots not associated with any volume (orphaned).

2) Snapshots associated with a volume that is no longer attached to any active, running EC2 instance (meaning the volume is detached or the associated EC2 instance is terminated.
3) Snapshots whose associated source volume has been deleted

This lambda function is integrated with AWS CloudWatch through eventbridge and it triggers every 15 days.


## <ins>Tools and Technologies used:</ins>
- Amazon Web Services(AWS)
- AWS Lambda
- Python
- AWS EC2
- AWS EBS
- AWS CloudWatch
