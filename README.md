Google Cloud Practice
========================

#   [Link to Qwiklabs Screenshots](https://drive.google.com/drive/folders/1kKf1kmnHi33msABB_VIIycuchuMRIBKH?usp=sharing)


**NB:** I have worked on 10 labs and each lab mentioned below links you to each of the screenshots required  saved in the google drive. 
 Together with 2 Translation tasks

## Course: Google Cloud Platform Fundamentals - Core Infrastructure

### Module: Getting Started with Google Cloud Platform

*   **[Getting Started with Cloud Marketplace].**

*   **[Getting Started with Compute Engine].**


### Module: Containers in the Cloud

*   **[Getting Started with Kubernetes Engine:].**



### Module: Applications in the Cloud

*   **[Getting Started with App Engine:].**



## Course: Essential Google Cloud Infrastructure: Foundation

### Module: Introduction to Google Cloud

*   **[Console and Cloud Shell:].**

*   **[Infrastructure Preview:].**

### Module: Virtual Networks

*   **[Implement Private Google Access and Cloud NAT:].**


### Module: Virtual Machines

*   **[Creating Virtual Machines:].**

### Module: Module: Developing, Deploying and Monitoring in the Cloud

*   **[ Getting Started with Deployment Manager and Stackdriver:]**




### Module: VPC Networking
*   **[ VPC Networking:]**



# Translation


Console and Cloud Shell
1.  gsutil mb gs://murgy-123
2.  gsutil cp sample.txt gs://murgy-123
3.  gcloud compute regions list
4.  INFRACLASS_REGION=us-central1
5.  echo $INFRACLASS_REGION
6.  mkdir infraclass
7.  echo INFRACLASS_REGION=$INFRACLASS_REGION >> ~/infraclass/config
8.  INFRACLASS_PROJECT_ID=qwiklabs-gcp-04-19829e311f08
9.  echo INFRACLASS_PROJECT_ID=$INFRACLASS_PROJECT_ID >> ~/infraclass/config
10.  source infraclass/config   && echo $INFRACLASS_PROJECT_ID
11.  nano .profile
12.  source infraclass/config
13.  echo $INFRACLASS_PROJECT_ID



Implement Private Google Access and Cloud NAT

SSH to vm-internal to test the IAP tunnel
 gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap

To test the external connectivity of vm-internal, run the following command:
 ping -c 2 www.google.com

To return to your Cloud Shell instance, run the following command:
exit

Copy an image from a public Cloud Storage bucket to your own bucket.

gsutil cp gs://cloud-training/gcpnet/private/access.svg gs://murgy-1

Access the image from your VM instance
gsutil cp gs://murgy-1/*.svg .
gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap

gsutil cp gs://murgy-1/*.svg .
gsutil cp gs://[my_bucket]/*.svg .

Try to update the VM instances
sudo apt-get update
gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap

sudo apt-get update

Verify the Cloud NAT gateway
sudo apt-get update

Configure and view logs with Cloud NAT Logging
Generating logs
gcloud compute ssh vm-internal --zone us-central1-c --tunnel-through-iap
sudo apt-get update







**NB:** WORK  **YES** check what 

