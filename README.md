Day-2 AWS assignment try   share screenshot's and delete the resources 
Cloud DevOps HUB
•
9:32 AM (Edited 11:20 AM)
2 points
Disaster Recovery (DR) – EC2 Backup & Restore
✅ Backup Strategy
OS (Operating System):
➤ Create an AMI (Amazon Machine Image) of the EC2 instance.
This includes the root volume, installed OS, configurations, and applications.

Data (Attached EBS volumes):
➤ Take Snapshots of the EBS volumes to back up the data.

🔄 Restore Strategy
To Restore Data:

Snapshot ➝ EBS Volume
Create a new volume from the snapshot and attach it to an EC2 instance.

To Restore the Whole EC2 Instance:

AMI ➝ EC2 Instance
Launch a new EC2 instance using the saved AMI.

Alternate Approach:

Snapshot ➝ AMI ➝ EC2 Instance
Convert the snapshot to an image (AMI), then launch an EC2 instance from that AMI.
