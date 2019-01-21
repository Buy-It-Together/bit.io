# Buy It Together

## Specification of requirements
The application aggregates consumers who want to buy the same product online. Aggregation takes place in the area designated by the recipients. After summing up user offers, the system sends a chat invitation. The user can preview the suggested location of the meeting. After acceptance of the chat invitation, users can communicate in real time.

## A domain dictionary of concepts
- User - a person using the application
- Link - the address of the website with the offer.
- Offer - user defined desire to purchase a given item indicated under the link provided above.
- Chat - defines a set of users who want to purchase a given product.
- Chat invitation - information about the possibility of joining a chat.

## Functional requirements
- The user is authenticated based on the email address and password. During the registration process, the user must click on the activation link sent to the previously provided email address.
- The user's password is stored in the database in an undisclosed way.
- Each user can add an offer. The data entered must be validated. The destination address is to be converted from a user-readable form to geographical coordinates. When defining an offer, fill in the fields:
  - Link to the subject.
  - Destination address.
  - Distance that the user can overcome in order to pick up the item.
  - The number of products that you want to buy.
  - The number of products needed to get the promotion.
  - The offer expiration date.
- Each user can view their offers.
- After aggregating the offers, the user gets an invitation to chat. The user can view the proposed location before accepting the invitation.
- After accepting the invitation, the user can communicate in real time with other chat users.

## Non-functional requirements
- The user should be able to use the application on mobile platforms with Android.
- Use of the system should be intuitive and convenient for the user.
- The application should not use batteries unnecessarily.
- The system should be available at any time of the day.
- The application should use free solutions.
- The system should allow clients to be implemented on platforms other than Android without interfering with the server's source code.

## Business rules
- If the time of the logged-in user to the application exceeds the default defined session time on the server side, the user must repeat the login operation.
- No limit on the user adding offers.
- No limit of invitation invitations sent by the system.
- Only one invitation relating to the offer can be accepted.
- A person who is not logged into the system is not able to use it. The exception is the logging and logging functionality. 
