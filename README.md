# AWS Global Infrastructure

## Regions

- AWS has approximately 31 launched regions globally (subject to change)
- Some regions may be in preparation for future launch
- Regions are geographically distributed across many countries

## Availability Zones (AZs)

- Each region consists of at least 3 data centers (Availability Zones)
- AZs within a region are:
  - Connected together
  - Located within a 100 km diameter circle
  - Designed for high reliability and availability
- Some regions may have more than 3 AZs (up to 5)
- As of now, AWS has 99 Availability Zones globally

### Benefits of Multiple AZs
- Provides redundancy
- Ensures high availability
- If one AZ fails, others can handle the load
- Customers can choose to deploy across one or multiple AZs

## Global Edge Network

- Consists of approximately 450 points of presence (PoPs)
- These are mini or micro data centers
- Primary purpose: Support Amazon CloudFront (Content Delivery Network - CDN)

### CloudFront and CDN
- Simplifies content delivery process
- Distributes content (websites, media) closer to customers
- Content is distributed based on customer locations
- Reduces data latency, especially beneficial for:
  - Websites with high traffic
  - Audio and video streaming

### Edge Network Benefits
- Minimizes latency for end-users
- Improves performance for global audiences
- Provides scalability for content delivery

## Key Points
1. AWS's infrastructure is designed for high availability and global reach
2. Regions provide geographical diversity
3. Availability Zones ensure redundancy within regions
4. The Global Edge Network optimizes content delivery worldwide
