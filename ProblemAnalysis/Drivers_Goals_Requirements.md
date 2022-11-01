# Business Goals, Drivers and Requirements
---

## Goals

The HeyBlue App Project has the following set of key goals, aimed at fostering connections between civilians and police officers, and helping charities:

1. Incentivize connections between civilians and police officers, helping to form a healthier community and create a sense of belonging. Through allowing civilians and police officers to collect points on successful connections, and using points to buy goods from retail stores (civilians), pay fines/fees (civilians) or donating points to charities (civilians and police officers).
2. Increase visibility of charities by providing them a centralized platform, where they can buy the things they need to better serve the communities they support.
3. Provide a platform that is easy to use, secure, and engaging.
4. Gather analytics on app usage to measure impact of app in community.

## Drivers

The business drivers are created from the problem statements that the HeyBlue App Project faces:

1. There are few opportunities and incentives of friendly connections between police officers and civilians.
2. Engagement on the app by civilians and polcie officers will improve visibility of charities within the community.

## Architecturally Significant Requirements

| # | Significant Architectural Requirements | Business Goal |
|----|----|----|
| 1 | Ease of Use | 3 |
| 2 | Community Engagement  | 3 |
| 3 | Retail Stores Profiles  | 1 |
| 4 | Connect Charities  | 1, 2 |
| 5 | Connect Civilians and Police Officers  | 1 |
| 6 | Security  | 3 |
| 7 | Prevent misuse or abuse of the platform  | 3 |
| 8 | Analytics  | 4 |

### 1. Ease of use

- Intuitive UI
- Ability to register and login using social media profiles

### 2. Community Engagement

- Location tracking
- Push notifications
- Uploading to social media
- Connecting to users social media
- Allow Businesses/Charities to create a storefront on the app to encourage users to redeem or donate their points
- Allow local municipalities to offer points for fines/fees in order to get citizens back on the road (suspended licenses or to pay down any municipal fine)
- A intrinsic reward system created (Think: confetti falling, bells and whistles happening, trophies awarded) We also uploaded a cool quote about connection to be used for each time a connection is made)

### 3. Retail Stores Profiles

- The Platform must provide a way to allow Civilians to find retail establishments where they can redeem their points.
- Businesses should have a catalog of items that they are offering and the point value assigned to each item available. 

### 4. Connect Charities

- The Platform must provide a way to allow Officers to find Charities where they can gift their points.

### 5. Connecting Civilians and Police Officers

- Connecting with other users
- A connection can only happen if the community member and the police officer are within a 10 ft distance from each other
- Community members find the officers that are willing to connect, officers cannot find the community members
- Community members find the officers that are willing to connect, officers cannot find the community members
- Community members to be able to see how many connections each participating officer has made

### 6. Security

- The App must protect user data and consider what data is stored and what data is transient
- Officers location must automatically shut off after 15 minutes
- Officers and community members must have the ability to connect with each other without being found 

### 7. Prevent misuse or abuse of the platform

- Users can only have one connection per officer per 24 hour period
- Community members must link an email address to a particular phone and not be able to register multiple devices to a particular email address
- A connection can only happen if the community member and the police officer are within a 10 ft distance from each other

### 8. Analytics

- A way to track how the points were used for each user (civilian, officer, business, municipality)
- Allow Hey, Blue! to track all participation by zip code
- Web and Mobile-Based with back-end processing and reporting and analytics that tracks site activity, connections
- Analytics can take app data and aggregate it with other available public data to build comprehensive reports to show impact of app in community
- The ability for aggregated data to be automatically shared with local media outlets
- Tracking engagement is a hard requirement
