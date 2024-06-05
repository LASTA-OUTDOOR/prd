# Non-Functional Requirements for LASTA Project

We document the non-functional requirements that the MVP must satisfy to make it viable.

## Security, Privacy, and Data Retention Policies

### Security and Trust

- **Data Encryption**: All user data related to outdoor activities, preferences, and personal information must be encrypted both in transit and at rest to prevent unauthorized access.
- **Access Control**: Implement role-based access controls to restrict data access to authorized personnel only, ensuring that sensitive information about user locations and preferences is secure.
- **Regular Audits**: Conduct regular security audits and vulnerability assessments to ensure compliance with security standards, particularly focusing on the safe handling of location-based data.
- **Incident Response**: Maintain an incident response plan to promptly address any data breaches or security incidents, especially those that could compromise user location and activity data.

### Privacy Considerations

- **Location Permissions**: Users must be able to control and grant location access specifically for LASTA, ensuring transparency and consent for location-based recommendations.
- **Data Anonymization**: Personal identifiers should be anonymized where possible to protect user identity, particularly in activity tracking and recommendations.
- **User Consent Management**: Provide clear options for users to manage their data sharing preferences and withdraw consent at any time, with an emphasis on controlling location and activity data.

### Data Retention Policy

- **Minimal Data Storage**: Store only the necessary data required for providing the service, such as user preferences and location data for generating recommendations.
- **Data Deletion**: Implement policies for regular deletion of outdated or unnecessary data to minimize risk, such as periodically clearing old activity logs and location history.
- **User Control**: Allow users to request deletion of their data at any time, in compliance with applicable regulations like GDPR and CCPA, ensuring users can remove their activity history and personal data.

## Adoption, Scalability, and Availability

### Adoption

1. The application must, by default, have all push notifications disabled to avoid unnecessary digital distractions for users planning outdoor activities.
2. Users should have the option to selectively enable push notifications for specific functionalities within the app, such as weather alerts or activity suggestions.
3. The application’s user interface must include easily accessible settings for customizing notification preferences related to outdoor activity updates.
4. Adoption metrics must focus on user engagement quality rather than frequency, emphasizing the app’s value-add to the users’ outdoor experiences.

### Scalability

1. The application must be capable of scaling resources automatically to accommodate fluctuating user loads, particularly during weekends and holidays when users are more likely to plan outdoor activities.
2. The system should maintain optimal performance and response times, even under high traffic conditions, such as sudden spikes in user activity due to favorable weather conditions.
3. Scalability solutions must include database read-replicas and backend load balancing capabilities to ensure resource efficiency and service continuity, especially during peak usage times.

### Availability

1. The application must achieve a minimum uptime of 99.9%, ensuring consistent availability to users planning their outdoor adventures.
2. Implement comprehensive failover mechanisms to handle potential system disruptions, including power, network, and hardware failures, to maintain service availability during critical usage periods.
3. Regular data backups and a robust disaster recovery plan must be in place to enable quick restoration of services in case of system failures, ensuring users have continuous access to activity recommendations.
4. Continuous monitoring systems must be employed to detect and address performance issues and crashes proactively, maintaining a seamless user experience while exploring outdoor activities.