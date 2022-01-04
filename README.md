Model architecture planning

Membership 
- slug
- type(free, pro,entetrprise)
- price
- strip plan id

UserMembership
- user(foreign key to default user)
- stripe customer id
- membership type(foreign key to Membership)

Subscription
- user membership
- stripe subscriotion id(foreign key to UserMembership)
-active

Course
-slug
-title
-description
-allowed membersjips(foreign key to Membership)

Lesson
-slug
-title
-course (foreign key to Course)
-position
-vedio
-thumbnail