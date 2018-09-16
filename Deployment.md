# Gerrit and Website Deployment Services Comparison

## Needs

- Docker
- 1gb RAM
- 1 vcpu
- 80gb HDD space
- 1tb backups space (NAS is possible)

## Like-to-haves

- Lowest possible costs
- All on one service

## AWS

- Docker
  - ECS Cluster
- Instance
  - EC2
  - t2.micro
    - 750 hrs a month
    - Burstable compute
    - 1 vcpu
    - 1gb ram
- 100% uptime possible
- Storage
  - EBS
  - 30gb free, higher price for rest of storage
  - gp2, general purpose ssds
  - $0.10 per gb-month, making the extra 50gb $5 a month
  - 100 iops
- Backups
  - Glacier
  - 10gb free per month
  - $0.004 per gb-month, making the extra 990gb $3.96 a month
- All in one service

### AWS Free tier total

$8.96 a month

### AWS Paid total

$20.50 a month

### AWS First year total

$107.52

### AWS after first year total

$246

--------

## GCP

- $300 credits
- Docker
  - K8s
- Instance
  - n1-standard-1
    - 1 vcpu
    - 3.75gb ram
    - $24.27 per month
- 100% uptime possible
- Storage
  - 120 iops HDD
  - $3.20 a month
- Backups
  - Coldline
  - $7 a month
- All in one service

### GCP Free tier total

$8.27 a month

### GCP Paid tier total

#### Always Free

$33.27 a month

#### Paid

$34.47 a month

### GCP First year total

8 months no payment, followed by the 9th month at $24.24 and full price the next 3 months,
totalling $113.64 in a year

### GCP after first year total

$413.64
