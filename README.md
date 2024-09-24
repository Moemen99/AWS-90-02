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



## Local Zones

Local Zones are an extension of AWS Regions, providing additional infrastructure closer to end-users.

### Characteristics
- Mini data centers with core AWS services
- Primarily focused on compute, storage, and networking services
- Connected to the nearest AWS Region

### Benefits

1. **Reduced Latency**
   - Closer proximity to end-users compared to full Regions
   - Latency reduced from 10-100 milliseconds to single-digit milliseconds
   - Critical for high-traffic applications and those requiring rapid response times

2. **Regulatory Compliance**
   - Allows data to remain within specific geographical boundaries
   - Useful for industries with strict data residency requirements (e.g., banking)

3. **Extended Regional Capabilities**
   - Access to core services of the parent Region
   - Combines benefits of local presence with full Regional capabilities

### Use Cases
- High-performance applications sensitive to latency
- Financial services requiring in-country data storage
- Any scenario where both local presence and access to full AWS services are needed

### Technical Advantages
- Single-digit millisecond latency for nearby users
- Seamless integration with parent AWS Region
- Access to essential AWS services without need for full Regional deployment

## Key Points
1. Local Zones extend AWS Regions' reach to more locations
2. They offer a balance between local presence and full AWS capabilities
3. Crucial for latency-sensitive and regulatory-compliant applications
4. Provide a solution for scenarios where data must remain within specific geographical boundaries
