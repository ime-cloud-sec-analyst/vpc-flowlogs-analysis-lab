# vpc-flowlogs-analysis-lab
AWS lab: Analyze VPC Flow Logs using Amazon S3, extract rejected IPs, and generate a security report.
# VPC Flow Logs Analysis Lab

This AWS lab project focuses on analyzing **VPC Flow Logs** stored in **Amazon S3**, identifying **rejected IPs**, and investigating **network activity** using AWS services and the CLI.

## 🧪 Lab Overview

In this lab, we:

- Created an S3 bucket to store VPC flow logs
- Enabled **VPC Flow Logs** for a specific ENI (Elastic Network Interface)
- Downloaded and decompressed `.log.gz` files
- Parsed logs to extract:
  - Source IPs that were **rejected** by security groups
  - Rejection frequency of each IP
- Converted log timestamps into human-readable format
- Visualized a security report in **Excel**
- Reviewed the EC2 security group inbound rules for improvement

## 📁 Project Files

- `flowlogs/*.log`: Sample flow log files in gzip format
- `rejected_ip_report.xlsx`: Final Excel report showing rejected IPs and their count

## 🛠 Tools Used

- Amazon EC2
- Amazon S3
- AWS VPC Flow Logs
- AWS CLI
- Python (pandas, gzip, re)
- GitHub

## 📊 Sample Output

| Source IP     | Rejection Count |
|---------------|------------------|
| 192.0.2.1     | 7                |
| 203.0.113.45  | 5                |

## 🔐 Security Insight

This lab demonstrates how to identify potentially malicious traffic being blocked by security groups, which is essential for improving cloud security posture.

## 📎 Author

**Ime Ben**  
AWS Cloud & Security Analyst  
GitHub: [ime-cloud-sec-analyst](https://github.com/ime-cloud-sec-analyst)
