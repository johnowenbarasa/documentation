# 📌 Notification Subscription Task: Implement client subscription functionality

## 🧾 User Story

> As an admin user,
I want to be able to create a notification rule,
And add condition groups to the rule,
And assign members to each group,
So that I can control and configure how and to whom notifications should be sent based on specific criteria.



---

## ✅ Acceptance Criteria
I can create a new notification rule with a name and description.

✅ I can define one or more condition groups under a rule, each with logical operators (e.g., AND, OR).

✅ I can add one or more conditions to each group (e.g., field, comparison, value).

✅ I can assign members (e.g., user or target IDs) to each group who should receive the notification if the group conditions are met.

✅ When all conditions in a group are met (based on the group’s operator), notifications should be triggered to the specified members.

✅ I can update or remove groups and members as needed after rule creation.

---
## Notes
1. Admin user will search a client by entering their registered email or customer number, subscriber Id and clicking search. Handle  scenario for both existing and non-existent customer, only existing clients should be able to subscribe to events .
2. On Success a user will click on the returned Subscriber Information .
3. Navigate to Subscriber Home . The Subscriber Home should provide these tabs
   a) **Overview**
      - Read Only Details of the Subscriber including the status of the subscriber.
      - Update Call To Action
      - Deactivate Call To Action
   b) **Notification Rules**. with the below information
    - Displaying List of all Notification Rules
    - Ability to add new Rule
    - Ability to filter rules
    - Ability to search for a rule
   
5. Each Rule should be clickable to allow navigation to an individual rule 
---

### NOTIFICATION RULE HOME
Notification Rule Home should be able to capture and show the below details
1. Show Rule Header Information(group details)
2. Tabs to make it easy for user to filter the action they want to perform. Tabs to be considered
   - **Overview (Tab)**
     - Notification Rule Details. (provide away to update)
     - List Group (should be clickable to allow navigation)
     - Delete
   - **Group (Tab)**

---

## NOTIFICATION RULE GROUP

Notification Rule  Group Details will have the below the tabs
   - **Overview**
      - Show Group Details (provide away to update)
      - Show Group Conditions
      - Show Group Members
      - Delete
   - **Group Condition(Tab)**. Displays List of Conditions with call to action possibilities (remove, add, update)
   - **Group Members (Tab)**. Displays List of Members with call to action possibilities (remove, add)

**Domain Rule Representation**
- ✅ Name
- ✅ Description
- 🧠 Owner (Provided At Backend)


**Domain Group Representation**
   - ✅ Name 
   - ✅ Description

**Domain Group Condition**
- ✅ Field
- ✅ comparison
- ✅ value

**Domain Member Condition**
- ✅ FirstName
- ✅ LastName
- ✅ Email
- ✅ Mobile Number
- ✅ Preferred Channel (Mobile or Email)

---



---

## 🔥 Priority

**Must Have**

## 🎯 Story Points

**3**

## 🔗 Dependencies

- Email service must be operational.

---

## 📝 Notes

- Ensure compliance with GDPR for user data handling.
- Consider adding CAPTCHA to prevent automated requests.
