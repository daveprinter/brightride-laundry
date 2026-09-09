# BrightRide Laundry

Create an app called BrightRide Laundry Services. When the first pass first loads, there is a login page where the user is asked to create account, and the first card is, as a customer, and the other card is as a marketer or partner. When the user clicks on the either of the card, if he does not have an account, there is a process to create one. For the client, he's asked to enter their email, their phone number. Their first name and last name. And then proceed with the login. The login should be professional in such a way that if an email is entered in create account and the email already exists in the system, it has already created account with the app, it is-- it shows that error. If he tries to log in but the email, uh, uh, is not registered, he's asked to create one. Okay. Now, for the client or customer, upon logging in, uh, the, the make it professional in their dashboard. You will see, um, there will be cards to show ongoing service. If the user, there is a la-laundry service that he had ordered and it was picked up, there will be, uh, showing ongoing cleaning. When he clicks on the ongoing cleaning, it opens a page to see what is being cleaned and the estimated time that is remaining. You will see in cards, for example, uh, a duvet, carpet. It is showing like that and showing the progress. You will also have, um, a dashboard to navigate to, uh, uh, well, a card showing complaints. If he wants to file a complaint, he, he, he files the complaint there a-and types. For example, if the cleaning was not done thoroughly or anything, and he clicks send complaint to management, which will be seen in the management, uh, panel, which we'll come to later. Also, there will be another dashboard called referrals. No. For referrals, let it, uh, be only in the, um, market, um, in the marketer or the partner tab. Now, another, uh, button that will be in the, in, in the user, there will be, uh, order a new service. When he clicks order a new service, he selects from cards, uh, what to be cleaned. There will be carpet, and he input size of carpet, which is optional. There is duvet, there is sofa set, and then he selects whether it is one-seater, two-seater, or three-seater. There is clothes, uh, one laundry basket, which goes for three fifty. The carpet goes for, uh, one fifty and showing a discount w- because it was initially two hundred. Then there is shoes. Yeah. Then he, he, he, he adds to cart. He adds to cart, the service cart. So he can add the number of items he wants to be cleaned of such category. Then when he clicks execute service or order service now in the cart, it, it will, uh, send a message automatically to WhatsApp number, which I'm going to give you the WhatsApp number. It will send, uh, there with a pre-built message, pre-typed message that goes in different, uh, ways depending on the service which the customer has selected. It sends the service request there. And then in the management dashboard, when, when the user, uh, when the manager or the cleaner s- despite the message coming to WhatsApp, it also reflects in his management dashboard. Then he approves. Upon approving, they will call him or message him inside the app. So inside the app of the client, also add a messaging button and a dashboard. When the messaging is clicked, it opens a messaging, uh, panel where there is a field to input text and send images. So they should, it should have attach image, attach images and send message, and these messages should be real and should be flowing from the, the client to the management, to the manager dashboard. From the client to the manager, from the client to the manager.Yes. For a laundry-service platform, I’d structure it as three main interfaces:



1. Client Dashboard — customers ordering and tracking laundry.

2. Partner/Marketer Dashboard — people referring customers and earning commissions.

3. Admin/Management Panel — the business controls everything.



You can also later add a Staff/Operations Dashboard if the laundry has workers who collect, wash, package, and deliver orders.



---



1. 👤 Client Dashboard



You already have a good foundation. I would organize it like this:



🏠 Dashboard / Home



Show the customer a quick overview:



- Current active order

- Order status

- Estimated completion time

- Upcoming pickup/delivery

- Total orders

- Total amount spent

- Loyalty points

- Available discounts

- Outstanding balance

- Notifications

- Quick Order Service button



Example:



«Order #LW1025

Washing → In Progress

Expected completion: Today, 5:30 PM»



---



🛒 Order New Service



Your existing idea is good.



Allow customers to select:



Laundry categories



- Clothes

- Bedding

- Curtains

- Carpets

- Shoes

- Duvets

- Blankets

- Suits

- Towels

- Other



Then:



Quantity



- 1 shirt

- 2 trousers

- 1 duvet

- etc.



Or, if your business charges by weight:



«7 kg × KSh 150/kg = KSh 1,050»



The customer should then choose:



- Pickup

- Drop-off

- Pickup + delivery



And select a preferred date/time.



---



📦 My Orders



This is one of the most important sections.



Show:



- Pending orders

- Accepted orders

- Pickup scheduled

- Collected

- Washing

- Drying

- Ironing

- Quality check

- Ready

- Out for delivery

- Delivered

- Cancelled



Each order should have an order timeline.



For example:



Order #1025



"Ordered → Confirmed → Picked Up → Washing → Ironing → Ready → Delivered"



---



📍 Pickup & Delivery Tracking



If you provide delivery, this can be very useful.



Show:



- Pickup address

- Delivery address

- Driver/rider

- Rider phone/contact

- Estimated arrival

- Delivery status



Eventually you could integrate maps/live location.



---



💳 Payments & Wallet



Include:



- M-Pesa

- Card

- Other payment methods

- Payment history

- Pending payments

- Refunds

- Wallet balance

- Transaction receipts



For Kenya, M-Pesa would obviously be a major option.



---



🎟️ Coupons & Promotions



Customer can see:



- Available coupons

- Discount codes

- Expiry dates

- Used coupons

- Referral discounts



Example:



«WELCOME100

Get KSh 100 off your next laundry order.»



---



⭐ Loyalty / Rewards



This is a good feature for retaining customers.



For example:



100 points = KSh 50 discount



Show:



- Current points

- Points earned

- Points spent

- Available rewards

- Loyalty level



Example:



Bronze → Silver → Gold → VIP



---



🎁 Referral Program



Don't restrict referrals to marketers only.



Customers can also refer friends.



Example:



«Invite a friend

Your friend gets KSh 100 off.

You receive KSh 100 credit.»



This can connect directly to your partner/affiliate system.



---



💬 Messaging



You've already added this.



I'd make it more sophisticated than just a generic chat.



Allow:



- Customer → Manager

- Customer → Support

- Customer → Delivery staff

- Order-specific chat

- Attach photos

- Send documents

- Automated responses

- Read/unread status



For example, a customer can attach a picture:



«"This shirt was already damaged before pickup."»



That becomes useful for dispute management.



---



⚠️ Complaints / Disputes



You've already considered this.



Add structured complaint categories:



- Missing item

- Damaged item

- Wrong item

- Poor cleaning

- Late delivery

- Wrong price

- Missing clothing

- Delivery problem

- Staff behavior

- Other



Then give each complaint a status:



Submitted → Under Review → Investigation → Resolved



The admin can respond to it.



---



⭐ Ratings & Reviews



Allow customers to rate:



- Laundry quality

- Delivery

- Customer service

- Overall experience



Example:



⭐⭐⭐⭐⭐



And optionally:



«"Very fast service."»



You can also allow customers to rate individual orders.



---



👤 Profile



Include:



- Name

- Phone

- Email

- Profile picture

- Addresses

- Saved pickup locations

- Preferred payment method

- Notification settings

- Password/security

- Account verification



---



🔔 Notifications



Important notifications include:



- Order accepted

- Pickup reminder

- Laundry collected

- Washing started

- Order ready

- Delivery started

- Payment successful

- Payment failed

- Complaint response

- New promotion

- Referral reward

- Loyalty points earned



---



📜 Receipts & Invoices



Customers should be able to open an order and see:



Subtotal

Delivery fee

Discount

Tax, if applicable

Total



And download/share the receipt.



---



2. 🤝 Marketer / Partner Dashboard



Your idea is already strong.



I'd divide it into several sections.



📊 Partner Overview



Show:



- Total referrals

- Active customers

- New customers this month

- Completed referrals

- Total commission

- Pending commission

- Paid commission

- Conversion rate



Example:



«Customers Referred: 148

Active Customers: 92

Total Commission: KSh 24,500

Pending: KSh 4,200

Paid: KSh 20,300»



---



📈 Analytics



Give the marketer graphs for:



- Referrals over time

- Orders generated

- Revenue generated

- Commission earned

- Conversion rate

- Best-performing days/months



Also:



Top customers referred



---



🔗 Referral Link



Every marketer gets something like:



«"laundryapp.com/ref/DAVE123"»



When someone registers through it, the system automatically associates that customer with the marketer.



Could also generate:



- QR code

- WhatsApp referral link

- SMS referral link

- Social media sharing



---



💰 Commission



Very important.



Show:



- Commission rate

- Commission earned

- Pending commission

- Approved commission

- Paid commission

- Reversed commission

- Commission history



Example:



«Customer spends KSh 2,000

Commission = 10%

You earn KSh 200»



---



💸 Withdrawals



Partner can request payment.



Show:



- Available balance

- Minimum withdrawal

- Withdrawal history

- Pending withdrawal

- Approved withdrawals

- Rejected withdrawals



Admin approves the withdrawal.



---



👥 Referred Customers



List:



Customer| Joined| Orders| Revenue| Commission

John| Aug 20| 5| 8,500| 850

Mary| Aug 25| 2| 3,200| 320



---



🏆 Partner Levels



This can encourage marketers to bring more customers.



Example:



Starter — 5 customers

Bronze — 20

Silver — 50

Gold — 100

Platinum — 250



Higher levels can receive higher commissions.



---



🎯 Targets



Give partners goals:



«Monthly Target: 50 customers

Progress: 37 / 50»



Reward:



«Reach 50 referrals → KSh 2,000 bonus»



---



📢 Marketing Materials



Admin can upload:



- Posters

- Flyers

- Social media graphics

- Videos

- Promotional messages

- QR codes



Partners can download/share them.



---



3. 🛠️ ADMIN PANEL



This is where I'd put the serious business controls.



The admin panel should essentially be the control center of the entire platform.



---



📊 Admin Dashboard



At a glance:



- Total customers

- New customers today

- Active orders

- Completed orders

- Cancelled orders

- Revenue today

- Revenue this month

- Pending payments

- Pending complaints

- Active partners

- Commission liability

- Delivery orders

- Average customer rating



And graphs:



Revenue



Orders



Customers



Partner performance



---



👥 Customer Management



Admin can:



- View customers

- Search customers

- Create customers

- Edit customers

- Suspend accounts

- Delete accounts

- Verify accounts

- View order history

- View payment history

- View complaints

- View ratings

- View referral source

- Give discounts

- Add loyalty points



---



📦 Order Management



This should be one of the biggest admin sections.



Admin can:



- View all orders

- Search order number

- Filter by status

- Assign staff

- Assign delivery person

- Change order status

- Edit order

- Cancel order

- Refund order

- Add extra charges

- Apply discounts



And see:



«Order → Customer → Items → Price → Pickup → Processing → Delivery → Payment»



---



🧺 Service Management



Admin controls what customers can order.



For example:



Shirts



- Wash: KSh 100

- Iron: KSh 50

- Wash + Iron: KSh 130



Duvet



- Single: KSh 500

- Double: KSh 700

- King: KSh 900



Admin can:



- Add service

- Edit service

- Delete service

- Change prices

- Create categories

- Enable/disable services

- Create special pricing



---



💰 Financial Management



Admin should have a financial center.



Show:



- Gross revenue

- Net revenue

- Expenses

- Refunds

- Discounts

- Delivery fees

- Partner commissions

- Staff payments

- Outstanding payments

- Profit



And transaction history.



---



🤝 Partner/Marketer Management



Admin controls the affiliate system.



Admin can:



- Approve partners

- Reject partners

- Suspend partners

- Create commission rules

- Change commission percentage

- View referrals

- View partner revenue

- Approve commissions

- Reverse commissions

- Process withdrawals

- Give bonuses

- Create partner levels



---



🚚 Delivery Management



If your laundry provides pickup/delivery, this becomes essential.



Admin can:



- Add drivers/riders

- Assign orders

- Track deliveries

- See active deliveries

- Set delivery zones

- Set delivery fees

- Set delivery schedules

- Manage failed deliveries



---



👷 Staff Management



I'd actually create this as a separate role.



Staff accounts could have permissions such as:



Laundry Worker



- See assigned laundry

- Update washing status

- Update drying status

- Update ironing status

- Mark order ready



Driver



- See assigned deliveries

- Pickup order

- Mark delivered



Manager



- See almost everything except sensitive admin settings.



---



💬 Support / Messaging Center



Admin gets a unified inbox:



Customer messages



Complaints



Order conversations



Partner messages



You can add:



- Assign conversation to staff

- Mark resolved

- Internal notes

- Attachments

- Priority levels



---



⚠️ Complaint Management



Admin sees:



«Complaint #C1042

Customer: John

Order: #LW1025

Category: Damaged item

Priority: High

Status: Investigation»



Admin can:



- Respond

- Request evidence

- Upload evidence

- Assign investigator

- Approve refund

- Offer discount

- Close complaint



---



⭐ Review Management



Admin can see:



- Average rating

- Reviews

- Negative reviews

- Positive reviews

- Rating by service

- Rating by location/staff



You could automatically flag:



1–2 star reviews → Management attention



---



🎟️ Promotions & Coupons



Admin creates:



«NEWCUSTOMER

KSh 200 discount

Minimum order: KSh 1,000

Valid until: 30 Sept»



Controls:



- Percentage discount

- Fixed discount

- Minimum order

- Maximum discount

- Usage limit

- Customer-specific coupons

- Partner-specific promotions

- Expiry date



---



🎁 Loyalty System



Admin controls:



- Points per order

- Points per KSh spent

- Membership levels

- Rewards

- Bonuses

- Expiration



---



📢 Marketing / CMS



Admin should be able to control what customers see without modifying code.



For example:



- Homepage banners

- Promotions

- Announcements

- FAQs

- Terms

- Privacy policy

- Service descriptions

- Blog/news

- Push notifications



---



🔔 Notification Management



Admin can send:



All customers



Specific customer



Partners



Staff



Specific customer group



Through:



- In-app notification

- Push notification

- Email

- SMS

- WhatsApp, if integrated



---



⚙️ System Settings



This is where you put global settings:



- Business name

- Logo

- Phone

- Email

- Business locations

- Currency

- Tax

- Delivery settings

- Payment settings

- Commission settings

- Loyalty settings

- Notification settings

- Order settings



---



🔐 Roles & Permissions



This is very important, especially if you're going to give the system to a real laundry company.



Don't make every staff account an administrator.



Create:



Super Admin

→ Everything



Manager

→ Orders, customers, complaints, reports



Finance

→ Payments, refunds, commissions



Laundry Staff

→ Processing orders



Delivery Staff

→ Pickup/delivery



Customer Support

→ Messages and complaints



Partner Manager

→ Marketers and commissions



Each role gets specific permissions.



---



📝 Audit Logs



I'd strongly recommend this.



Record things such as:



«Admin David changed order #1025 from KSh 1,500 → KSh 1,200.»



«Manager Sarah refunded KSh 500.»



«Admin John suspended partner #P104.»



«Staff Mike marked order #1025 as delivered.»



This protects the business from internal fraud and disputes.



---



📈 Advanced Analytics



The admin should eventually get a proper business intelligence section.



Customer analytics



- New customers

- Returning customers

- Customer retention

- Customer lifetime value

- Most active customers



Laundry analytics



- Most ordered services

- Average order value

- Orders per day

- Average processing time

- Late orders



Financial analytics



- Revenue

- Profit

- Expenses

- Refunds

- Discounts



Partner analytics



- Top partners

- Referral conversion

- Revenue per partner

- Commission costs



---



🏗️ I'd Add One More Dashboard: Operations/Staff



This is something you haven't mentioned, but it can make the system much better.



The customer shouldn't be directly interacting with the admin system for operational work.



A worker gets:



«Order #1025

8 shirts

2 trousers

1 duvet»



Then buttons:



Collected → Washing → Drying → Ironing → Quality Check → Packed → Ready



The delivery person sees:



«Pickup: Customer A

Drop-off: Customer B»



And marks:



Picked Up → On Route → Delivered



That means the whole process becomes trackable.



---



🔄 The Complete System



I'd ultimately structure your application like this:



                    LAUNDRY PLATFORM

                           │

          ┌────────────────┼────────────────┐

          │                │                │

       CLIENT           PARTNER          ADMIN

          │                │                │

     ┌────┴────┐      ┌────┴────┐      ┌────┴────────┐

     │         │      │         │      │             │

   Orders   Support  Referrals Commission Customers  Orders

     │         │      │         │      │             │

 Payments   Complaints Analytics Withdrawals Services Finance

     │         │                         │             │

 Delivery   Ratings                   Marketing      Reports

 f    │                                    │             │

 Loyalty                               Promotions   Settings

                                             

                           │

                      OPERATIONS

                           │

                  ┌────────┼────────┐

                  │                 │yr

               LAUNDRY           DELIVERY

                STAFF              STAFF

                  │                 │

              Processing         Pickup/Drop



The most important principle



Don't put every feature into the admin dashboard. Give each type of user only what they need.



For example, a laundry worker shouldn't see:



«Business revenue: KSh 2,500,000

Partner commissions: KSh 180,000»



They only need to see their assigned laundry jobs.



Likewise, a partner shouldn't see other partners' customers or earnings.



This role-based architecture will make the application much more professional and much easier to secure.

This is the Whatsapp number+254 701 987338

Also when the app is fast opened let it show the official prompt to allow app access location so it shows location of the client only in the client dashboard and add in settings tab my location which shows the real location of the client for delivery and pickup services and a button to manually update location,,by entering address,also when app is opened in browser everytime or refreshed let it prompt the user to install app to device which when clicked installs the app which doesn't open like it's opening via browser but opens like a real app then the load of the app it should be an animation video like that rhymes with what the app does

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/359ca76b-4364-4289-a63f-631b5645c683).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
