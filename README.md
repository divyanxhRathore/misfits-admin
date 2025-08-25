# Problem statement

The management of venues selection and updation in clubs need a more stringent and seamless system for the operations team as there is much reliance over whatsapp communication for this.

# Objective
To make the venues selection/updation a seamless process for management 

# Current scenario
Venue selection seems like an agency service from Misfits to leaders, this leads to us being treated as an infinite resource. 
Both parties have an interaction only with Misfits and hence do not get into a mutually beneficial relationship, where they look to help out each other

# Ideal Scenario 
They are interacting with a matching product that helps them connect with venues and oversee the conversation. The product will have rules to prevent misuse/overuse. It is clear that the association is between the venue and the leader, and Misfits is just the mediator here, so that both parties want to help each other out

# Core entities
1. Admin view for venues
2. Venue Managers
3. Frontend interaction system

# Front-end system for leaders
1. Create/update club venue requests (with eligibility restrictions)
2. View allotted venues in the club dashboard
3. Filter and explore recommended venues in the VMS
4. Raise discrepancies on venue terms

# Venue Managers Admin app
1. Maintain venue details (terms, policies, amenities, cover charge prices)
2. Manage venue calendar (event bookings, blackout dates)
3. Respond to leader requests (Accept/Reject/Modify terms)

# Process:
The leader/misfits employee is supposed to first create the club from the misfits app. Once information is approved, The leader will get a prompt on the home page saying - The club is created and you can now explore venues. They can explore venues once the club is approved.

Frontend system for interaction
Before a user can fully access and utilize the VMS, several critical inputs are required to facilitate accurate venue recommendations and management:
Estimated Footfall in a Meetup: This figure helps venues gauge the potential attendance and assess their capacity and resource allocation needs.
Requirements for Equipment: Details about any specific equipment needed for the activity (e.g., projectors, sound systems, specialized sports gear) are crucial for venue suitability and preparation.
Is leader looking to collect upfront from venue? If yes, what is the amount? This addresses financial arrangements and informs venues about potential advance payment requests, which can influence their terms and conditions.

# 1.1 VMS Main
The Venue Management System (VMS) portal is designed to streamline the process of club leaders finding and managing venues for their activities. The system intelligently filters and presents relevant venue options based on the activity chosen by the leader during the club creation flow. To ensure accurate filtering, the following crucial information must be integrated into the system:
Area: This specifies the geographical location where the club intends to host its activities, enabling the system to display venues within that vicinity.
Activity: The specific type of activity (e.g., sports, arts, educational workshops) is essential for matching suitable venues with appropriate facilities and environments.
Note: these info is already taken at the time of club creation
Once these criteria are input, the VMS will display a series of venue cards, each providing essential details to aid the leader's decision-making. These cards can be sorted using various filters, allowing for efficient navigation through the available options.

Upon clicking a venue card, the leader will be directed toa dedicated details page. This page serves as the primary interface for sending queries to the venue management team. It's important to note a critical limitation: a user is permitted to send queries for a maximum of two venues. After reaching this limit, the query submission button for any subsequent venues will be automatically disabled, encouraging focused selection and preventing excessive inquiries.

# 1.2 Approval Management from Venues

To provide transparency and control over venue interactions, a dedicated "Manage Venues" option will be integrated into the user's profile settings. This feature will allow users to monitor the real-time status of all their queries and requests submitted to various venues.

The "Manage Venues" page will offer a comprehensive overview of the status of each request, categorizing them as:
Complete: Indicates that the venue has processed and responded to the query/request.
Rejected: Signifies that the venue has declined the request.
In-process: Shows that the venue is currently reviewing the query/request.
Once an approval is received from a venue, the club leader will be able to access all the terms and conditions, along with the final schedule proposed by the venue. In the event of any discrepancies or issues with the approved terms or schedule, the club leader must have the ability to raise a discrepancy. Upon receiving a discrepancy, the venue will be required to review the issue and issue a fresh approval with the revised terms or schedule, ensuring a fair and agreeable arrangement for both parties.

# Admin App for Venues
2.1 Introduction: The Misfits Venue Manager Application
This application is meticulously designed by the Misfits team specifically for its venue managers. Its primary purpose is to centralize the management of all events and to streamline the process of receiving and responding to requests for association from Misfits communities. The Misfits Venue Manager Application offers a comprehensive suite of capabilities, enabling venue managers to efficiently oversee their operations and foster effective collaborations.
Key Capabilities of the Misfits Venue Manager Application:
Detailed Venue Setup and Configuration:
Amenities Management: Venue managers can meticulously detail all available amenities, including but not limited to sound systems, projection equipment, seating arrangements, catering facilities, Wi-Fi availability, and accessibility features. This ensures that community leaders have a clear understanding of the venue's offerings when considering a partnership.
Interactive Map Integration: The application allows for the integration of an interactive map, providing precise location details, nearby landmarks, and directions. This aids both Misfits community members and event attendees in navigating to the venue.
Image Gallery: Venue managers can upload high-quality images and virtual tours of their spaces, showcasing the venue's ambiance, various rooms, and event setups. This visual representation helps community leaders visualize their events within the venue.
Terms of Association: The platform facilitates the clear articulation of the venue's terms of association, including pricing structures, cancellation policies, operational hours, and any specific rules or regulations for events. This promotes transparency and clarity from the outset of any potential partnership.
Association Request Management Dashboard:
Centralized Request Viewing: A dedicated dashboard provides venue managers with a centralized view of all incoming requests for association from Misfits club leaders. This includes details about the requesting club, proposed event type, desired dates, and estimated attendance.
Efficient Approval/Rejection Workflow: Venue managers can easily review each request and choose to either approve or reject it directly from the dashboard. This streamlined process ensures timely responses to potential partners.
Comprehensive Calendar Management:
Integrated Event Scheduling: The application offers a robust calendar management system, providing venue managers with the flexibility to add and manage both Misfits events and other external events in a single, unified view. This prevents scheduling conflicts and optimizes venue utilization.
Automatic Misfits Event Integration: Upon mutual approval of a partnership, Misfits events are automatically added to the venue's calendar, reducing manual input and ensuring accuracy. This seamless integration ensures that once a partnership is confirmed, the event details are immediately reflected in the venue's schedule.
2.2 Core Concepts: Operational Framework for Venue Managers
Individualized Venue Manager Accounts: Each venue manager will have their own dedicated and secure account within the system. This ensures data privacy and allows for personalized management of their associated venues.
Multi-Venue Management Capability: For venue managers overseeing more than one venue, the system provides a seamless switching mechanism. This allows them to effortlessly navigate between different venue profiles under their management, enabling efficient oversight of multiple locations from a single account.
Initial Setup and Dashboard Redirection: Upon their initial login, venue managers will be guided through a concise setup process. This initial configuration ensures that all essential venue details are captured. Once the setup is complete, they are automatically redirected to their personalized dashboard, where they can immediately begin viewing and managing association requests from Misfits club leaders.
Scheduling Meets with Leaders (Operations Team Facilitation): While direct communication and event scheduling are managed within the app, the process of scheduling an initial meet-and-greet or a detailed discussion with a club leader is facilitated through the Misfits operations team. Venue managers can send a request to the operations team via the app, detailing their preference for a meeting. The operations team will then coordinate and fix a suitable time and date for the meeting between the venue manager and the club leader. This ensures efficient scheduling and proper facilitation of important discussions.
Partnership Approval Workflow (Mutual Acceptance):
Case of Acceptance: When a venue manager approves a received association request, the system then requires the club leader to also provide their approval. This secondary approval from the club leader is contingent upon their review of all the required terms and conditions outlined by the venue. This mutual acceptance process ensures that both parties are in full agreement with the terms of the partnership, leading to a formally approved collaboration.
Case of Discrepancy Raised by Leader: In situations where a club leader receives an approved request from a venue but is not entirely satisfied with the proposed terms (e.g., pricing, dates, specific rules), they have the option to raise a discrepancy. The venue manager will be notified of this issue, allowing them to review the leader's concerns. The venue can then issue a revised approval to the leader, potentially with adjusted terms, to address the raised discrepancy and work towards a mutually agreeable partnership.

# Happy Paths:

Flow: Club Leader New Venue Request
Leader fills pre-entry form (footfall, equipment, fee collection)
Leader filters/sorts venue listings
Leader views venue details → Clicks "Request Venue" (limit applied)
Venue receives request → Reviews & Accepts / Sends modification
Leader reviews → Accepts → Partnership confirmed

Flow: Update the venue
Enable leader mode
Open club info
Select “Update Location” and choose “Temporary Update” or “Permanent Update”
Upon permanent update, redirect to VMS 
Note: The temporary updation will be handled by the operations team and out of scope of VMS








#   m i s f i t s - a d m i n  
 