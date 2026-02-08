# AWS-EC2-Nginx-App-Deployment

# Application Access

This application can be accessed using either an **Elastic IP** or the **Public IP of the EC2 instance**.

## Access Options

### Option 1: Access via Elastic IP (Recommended)

An **Elastic IP (EIP)** is a static IPv4 address provided by AWS. It remains the same even if the EC2 instance is stopped or restarted.

**Steps:**

1. Allocate an Elastic IP from the AWS EC2 dashboard.
2. Associate the Elastic IP with the running EC2 instance.
3. Access the application using:

   ```
   http://<Elastic-IP>:<PORT>
   ```

**Benefits:**

* Static and reliable IP address
* No need to update IP after instance restart

---

### Option 2: Access via EC2 Public IP

Each EC2 instance is assigned a public IP address when it is launched.

**Steps:**

1. Go to the EC2 dashboard.
2. Select the running instance.
3. Copy the **Public IPv4 address**.
4. Access the application using:

   ```
   http://<EC2-Public-IP>:<PORT>
   ```

**Limitations:**

* Public IP may change if the instance is stopped and started again

---
#Author#
Rutuja Patil


---

✅ Application should now be accessible via browser using either method.
