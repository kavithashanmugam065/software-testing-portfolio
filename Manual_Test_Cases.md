# 🧪 Test Cases - Sample Module

| Test Case ID | Title                            | Module | Preconditions         | Test Data                         | Steps                                                                 | Expected Result                      | Status | Severity | Priority | Remarks |
|--------------|----------------------------------|--------|------------------------|-----------------------------------|-----------------------------------------------------------------------|--------------------------------------|--------|----------|----------|---------|
| TC_001       | Valid Login                      | Login  | On login page          | Username: user1<br>Password: 1234 | 1. Enter username<br>2. Enter password<br>3. Click login               | Navigate to dashboard                |        | Major    | High     |         |
| TC_002       | Invalid Password                 | Login  | On login page          | Username: user1<br>Password: wrong| 1. Enter username<br>2. Enter wrong password<br>3. Click login        | Show error: "Invalid credentials"    |        | Major    | High     |         |
| TC_003       | Empty Username and Password      | Login  | On login page          |                                   | 1. Leave fields blank<br>2. Click login                               | Show error: "Fields required"        |        | Minor    | Medium   |         |

# ✈️ Test Cases – MakeMyTrip

| Test Case ID | Title                                  | Module           | Preconditions               | Test Data                                | Steps                                                                                         | Expected Result                                       | Status | Severity | Priority | Remarks |
|--------------|----------------------------------------|------------------|------------------------------|-------------------------------------------|-----------------------------------------------------------------------------------------------|-------------------------------------------------------|--------|----------|----------|---------|
| TC_MMT_001   | Search Flights with valid input        | Flight Booking   | User on homepage            | From: Chennai<br>To: Mumbai<br>Date: 25-Jun| Enter source, destination, date → Click Search                                             | List of available flights displayed                  |        | Major    | High     |         |
| TC_MMT_002   | Search with past date                  | Flight Booking   | User on homepage            | From: Delhi<br>To: Goa<br>Date: 01-Jan-2023| Enter past date → Click Search                                                              | Error message: "Date cannot be in the past"          |        | Minor    | High     |         |
| TC_MMT_003   | Apply non-stop filter                  | Filters          | Search results loaded        | N/A                                       | Click on “Non-Stop” checkbox                                                                | Only non-stop flights should be displayed            |        | Minor    | Medium   |         |
| TC_MMT_004   | Check UI responsiveness on mobile      | UI/Responsiveness| Open site on mobile browser | N/A                                       | Open homepage → Scroll, Search → View filter section                                        | All components must be aligned and functional         |        | Major    | High     |         |
| TC_MMT_005   | Check broken links on homepage         | UI Testing       | User on homepage            | N/A                                       | Click all menu & footer links                                                              | All links should open valid pages (no 404 errors)    |        | Minor    | Low      |         |

# 💼 Test Cases – Amazon Jobs Portal

| Test Case ID | Title                                 | Module           | Preconditions        | Test Data                                  | Steps                                                                                      | Expected Result                                      | Status | Severity | Priority | Remarks |
|--------------|---------------------------------------|------------------|-----------------------|---------------------------------------------|--------------------------------------------------------------------------------------------|------------------------------------------------------|--------|----------|----------|---------|
| TC_AMZN_001  | Search job with valid keyword         | Job Search       | Logged in to account | Keyword: "Quality Analyst"<br>Location: India| Enter keyword and location → Click search                                                | Relevant jobs displayed                              |        | Major    | High     |         |
| TC_AMZN_002  | Apply without login                   | Job Application  | Not logged in         | Job ID: 12345                                | Go to job → Click Apply                                                                  | Prompt to log in or sign up                          |        | Major    | High     |         |
| TC_AMZN_003  | Upload resume in supported format     | Resume Upload    | Logged in             | File: `resume.pdf`                           | Navigate to profile → Upload resume                                                      | Resume uploaded successfully                         |        | Major    | High     |         |
| TC_AMZN_004  | Upload resume in unsupported format   | Resume Upload    | Logged in             | File: `resume.txt`                           | Navigate to profile → Upload resume                                                      | Show error: "Unsupported file format"                |        | Minor    | Medium   |         |
| TC_AMZN_005  | Check pagination in search results    | Job Search       | Search returns >10 jobs | N/A                                      | Scroll down → Click next page                                                            | Jobs from next page should be displayed              |        | Minor    | Medium   |         |

# 💬 WhatsApp – Test Cases

| Test Case ID | Title                               | Module             | Preconditions      | Test Data                       | Steps                                                                 | Expected Result                             | Status | Severity | Priority | Remarks |
|--------------|-------------------------------------|--------------------|--------------------|----------------------------------|------------------------------------------------------------------------|---------------------------------------------|--------|----------|----------|---------|
| TC_WA_001    | Send text message                   | Chat               | User logged in     | Message: "Hello World"           | Open chat → Type message → Tap Send                                   | Message is delivered with tick icon         |        | Major    | High     |         |
| TC_WA_002    | Send image                          | Media Sharing      | User logged in     | Select image from gallery        | Open chat → Tap attach → Select image → Tap send                      | Image is sent and viewable in chat          |        | Major    | High     |         |
| TC_WA_003    | Check blue ticks after seen         | Read Receipts      | Message delivered  | -                                | Send message → Receiver opens chat                                     | Two blue ticks appear                        |        | Minor    | Medium   |         |
| TC_WA_004    | Group name change by admin          | Group Management   | User is admin      | New Name: “Friends Group”        | Open group → Tap name → Edit → Save                                   | Group name updates for all users            |        | Minor    | Medium   |         |

# 📸 Instagram – Test Cases

| Test Case ID | Title                               | Module             | Preconditions      | Test Data                          | Steps                                                               | Expected Result                             | Status | Severity | Priority | Remarks |
|--------------|-------------------------------------|--------------------|--------------------|-------------------------------------|----------------------------------------------------------------------|---------------------------------------------|--------|----------|----------|---------|
| TC_IG_001    | Post a photo                        | Posting            | User logged in     | Photo + Caption                    | Tap + icon → Select photo → Add caption → Post                      | Post visible on profile                     |        | Major    | High     |         |
| TC_IG_002    | Follow another user                 | Follow System      | Logged in          | Username: @testaccount             | Search @testaccount → Tap Follow                                    | Button changes to "Following"               |        | Major    | High     |         |
| TC_IG_003    | View story                          | Story              | Story available    | -                                   | Tap on profile circle → Story opens                                 | Story loads full screen                     |        | Minor    | Medium   |         |






