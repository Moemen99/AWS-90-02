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


## Wavelength Zones

Wavelength is another infrastructure option provided by AWS, specifically designed for ultra-low latency applications.

### Characteristics
- Integrated with 5G networks
- Provides even lower latency than Local Zones
- Ideal for applications requiring the lowest possible latency

### Use Cases
- Mobile edge computing
- IoT devices
- Real-time gaming
- Machine learning inference at the edge

## AWS Regional Services List

When choosing a region for your AWS deployment, it's crucial to consider the available services in that region.

### Key Points
- Not all AWS services are available in every region
- New regions typically start with a core set of services
- Services are gradually added to regions over time

### Importance
- Check the AWS Regional Services list before choosing a region
- Ensure all required services are available in your chosen region
- Avoid potential issues with service availability after deployment

### Best Practice
- Regularly review the AWS Regional Services list
- Plan your infrastructure considering both current and future service needs

## Conclusion

AWS Global Infrastructure provides a range of options to meet diverse needs:

1. **Regions**: Core geographical areas with full service offerings
2. **Availability Zones**: Multiple data centers within a region for high availability
3. **Global Edge Network**: Content delivery optimization through CloudFront
4. **Local Zones**: Extended regional capabilities with lower latency
5. **Wavelength Zones**: Ultra-low latency integration with 5G networks

When planning your AWS infrastructure, consider:
- Geographic distribution of your users
- Latency requirements
- Regulatory and compliance needs
- Specific service requirements

Always check the AWS Regional Services list to ensure your chosen region supports all the services you need for your applications and workloads.
