Security Guide | PUBLIC

Document Version: 2.2 – 2026-05-08

Identity and Authentication Management in SAP
Business One

.

d
e
v
r
e
s
e
r
s
t
h
g
i
r

l
l

A

.
y
n
a
p
m
o
c
e
t
a

i
l

ffi
a
P
A
S
n
a
r
o
E
S
P
A
S
6
2
0
2
©

Content

1

1.1

1.2

1.3

1.4

1.5

1.6

1.7

1.8

1.9

Document History. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6

Change Log 10.0 SP 2605. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6

Change Log 10.0 FP 2602. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6

Change Log 10.0 SP 2511. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7

Change Log 10.0 FP 2508. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8

Change Log 10.0 SP 2505. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8

Change Log 10.0 FP 2502. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8

Change Log 10.0 SP 2411. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .9

Change Log 10.0 SP 2408. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9

Change Log 10.0 FP 2405. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10

1.10

Change Log 10.0 SP 2402. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10

1.11

1.12

1.13

2

3

Change Log 10.0 SP 2311. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11

Change Log 10.0 FP 2305. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11

Change Log 10.0 FP 2208. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .12

Introduction. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13

Configuring Identity and Authentication Management in the System Landscape Directory
. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15

3.1

Managing Identity Providers. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 16

Adding Identity Providers. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17

Deleting Identity Providers. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 52

Activating Identity Providers. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 53

Deactivating Identity Providers. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 54

3.2

Managing Identity Provider Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 55

Adding Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .56

Importing Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 59

Editing Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .60

Binding Users . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 61

Deleting Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .63

Copying User Mappings. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 63

Checking AD DS User Status. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 64

3.3

Managing SAP Business One Company Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 65

Unbinding Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 65

Editing Company Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 65

4

4.1

Reconfiguring Identity and Authentication Management. . . . . . . . . . . . . . . . . . . . . . . . . . . . . 67

Resetting Identity and Authentication Management. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 67

2

PUBLIC

Identity and Authentication Management in SAP Business One
Content

4.2

4.3

4.4

4.5

4.6

4.7

4.8

5

5.1

Renewing the Security Certificate . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 68

Changing the Port Number for Authentication Service. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 68

Activating B1SiteUser. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 69

Adding a User for Logging into the Authentication Service. . . . . . . . . . . . . . . . . . . . . . . . . . . . . 69

Activating B1SiteUser in the Authentication Service. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 70

Deleting the User. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 78

Changing Client ID and Client Secret in the Authentication Service. . . . . . . . . . . . . . . . . . . . . . . . . 80

Defining a Password Blocklist for Authentication Server Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . 82

Configure the Registry Key for Windows Domain Users. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .84

Configuring the Lifetime of the Access Tokens in Keycloak. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 86

Behavior Changes After Enabling Identity and Authentication Management. . . . . . . . . . . . . . 88

Logging into SAP Business One. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 89

No Identity Provider Is Activated. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 90

Only SAP Business One Authentication Server Is Activated. . . . . . . . . . . . . . . . . . . . . . . . . . . . 92

Only Active Directory Domain Services Is Activated. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 102

An External Identity Provider Is Activated. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 110

Multiple Identity Providers Are Activated. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 119

5.2

Managing Passwords. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 119

Changing Passwords. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .119

Complying with Password Policies . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 126

5.3  Windows Domain Single Sign-On After Upgrades. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 130

5.4

5.5

Single Sign-On After Enabling Browser Windows Integrated Authentication with AD FS. . . . . . . . . . 131

Other Changes in the SLD Control Center. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .131

Configuring the SLD and Authentication Server Addresses. . . . . . . . . . . . . . . . . . . . . . . . . . . . 131

Checking Personal Data and Change Log. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 132

5.6

Other Changes in the SAP Business One Client. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 133

Managing Technical Users . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 133

Lock Screen and Screen Locking Time. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 134

Permission Override. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 136

Company User Password Is Randomly Generated. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 137

Binding Users in SAP Business One Client. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .137

Password Never Expires and Change Password at Next Logon. . . . . . . . . . . . . . . . . . . . . . . . . 138

5.7

Single Logout (SLO). . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 139

6

6.1

6.2

Extensions. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 140

Scopes. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .140

SAP Business One Extension Single Sign-On Manager. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 141

Registering a New Client. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 141

6.3

End-to-End Scenario Overview. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 142

6.4  Walkthrough for Desktop Apps. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 143

Prerequisites. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 143

Identity and Authentication Management in SAP Business One
Content

PUBLIC

3

Dependencies. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 143

Creating Desktop App. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 144

Registering Desktop App. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .149

Creating Authentication WebView. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .151

OIDC Login. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 154

Retrieving Company List. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 156

Creating Choose Company WebView. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 157

Choosing Company. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 159

Connecting to Company. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 160

Refreshing Token. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 161

OIDC Logout. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 161

6.5  Walkthrough for Web Apps. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 161

Prerequisites. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 162

Dependencies. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 162

Creating Web App. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 162

Registering Web App. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 163

OIDC Login. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 165

Retrieving Company List. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 168

Choosing Company. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 168

Accessing the Service Layer. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 169

Refreshing a Token. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 171

OIDC Logout. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .171

OIDC Back-Channel Logout. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 171

6.6  Walkthrough for Single Page Apps. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 174

Prerequisites. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 174

Dependencies. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 175

Creating Single Page App. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 175

Registering Single Page App. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 176

OIDC Login. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 176

Retrieving Company List. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 179

Choosing Company. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 180

Accessing the Service Layer. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .181

Refreshing a Token. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 182

OIDC Logout. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 182

Configuring Audience in Keycloak. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 182

6.7

Walkthrough for Daemon Service. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 186

Prerequisites. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 186

Dependencies. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 186

Creating a Daemon Service. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 187

Registering the Daemon Service. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 188

Getting an Access Token. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 192

4

PUBLIC

Identity and Authentication Management in SAP Business One
Content

Getting a Company ID. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .194

Accessing the Service Layer. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 195

6.8

SLD API References. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .196

GetOpenIDConnectProvider. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 197

CurrentUserInfo. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 197

6.9

Connection References for Service Layer and DI API. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 198

6.10

Principal Propagation for SAP Business One. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 199

7

Limitations. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .200

Identity and Authentication Management in SAP Business One
Content

PUBLIC

5

1  Document History

The document history is a record of additions and major changes to the guide Identity and Authentication
Management in SAP Business One.

1.1  Change Log 10.0 SP 2605

Topic

All topics

Description

No updates.

Link to Related Section

1.2  Change Log 10.0 FP 2602

Topic

Description

Link to Related Section

Configuring Identity and
Authentication Manage-
ment in the System Land-
scape Directory

• The topic title is changed from Managing Users to

• Managing Identity Pro-

Managing Identity Provider Users.

• The description for the new Superuser checkbox is added

in the Binding Users topic.

• The Select All Results function is introduced in the Binding

Users topic.

• A new topic about managing company users is added.
• A new topic about editing company users is added.
• The Unbinding Users topic is moved to the new section

Managing SAP Business One Company Users.

• A note about simultaneously unbinding a user from more
than one company is added to the Unbinding Users topic.

vider Users
• Binding Users
• Managing SAP Busi-
ness One Company
Users

• Editing Company Users
• Unbinding Users

6

PUBLIC

Identity and Authentication Management in SAP Business One
Document History

Topic

Description

Link to Related Section

Behavior Changes After En-
abling Identity and Authen-
tication Management

The enhanced company selection interface is introduced.

• Logging in as Company

Users

• Logging into the SAP
Business One Client
• Logging into SAP Busi-
ness One, Web Client
• Logging into the SAP
Business One Client
• Logging into SAP Busi-
ness One, Web Client
• Logging into the SAP
Business One Client
• Logging into SAP Busi-
ness One, Web Client

Limitations

The limitation with the Report and Layout Manager: Advanced
Settings window is removed. For more information, see SAP

Limitations

Note 3606814

.

1.3  Change Log 10.0 SP 2511

Topic

Description

Configuring Identity and

A new topic about enabling browser Windows Integrated Au-

Authentication Manage-

thentication with AD FS is added.

ment in the System Land-

scape Directory

Reconfiguring Identity
and Authentication Man-
agement

The procedures are updated.

Behavior Changes After En-

A new topic about single sign-on after enabling browser Win-

abling Identity and Authen-

dows Integrated Authentication with AD FS is added.

tication Management

Link to Related Section

Enabling Browser Windows
Integrated Authentication
with AD FS

Adding a User for Log-
ging into the Authentication
Service

Single Sign-On After En-
abling Browser Windows
Integrated Authentication
with AD FS

Identity and Authentication Management in SAP Business One
Document History

PUBLIC

7

1.4  Change Log 10.0 FP 2508

Topic

Description

Link to Related Section

Extensions: Walkthrough for
Web Apps

Reconfiguring Identity
and Authentication Man-
agement

A new topic about OIDC Back-Channel Logout is added.

OIDC Back-Channel Logout

A new topic about Configuring the Lifetime of the Access To-
kens in Keycloak is added.

Configuring the Lifetime of
the Access Tokens in Key-
cloak

1.5  Change Log 10.0 SP 2505

Topic

Description

Behavior Changes After En-
abling Identity and Authen-
tication Management

The screenshots are replaced with the updated versions con-
taining the new SAP Business One logo.

Link to Related Section

Behavior Changes After En-
abling Identity and Authen-
tication Management

1.6  Change Log 10.0 FP 2502

Topic

Description

Link to Related Section

Configuring Identity and
Authentication Manage-
ment in the System Land-
scape Directory

• The description about adding AD DS users is updated.
• A new topic about importing users is added.
• A new topic about checking AD DS user status is added.
• The method of defining a user code is updated.

Reconfiguring Identity
and Authentication Man-
agement

• A new topic about deleting an administrator account by

executing queries is added.

• A new topic about defining a password blocklist for au-

thentication server users is added.

• A new topic about configuring the registry key for Windows

domain users is added.

• Adding Users
• Importing Users
• Checking AD DS User

Status

• Binding Users

• Deleting the User by
Executing Queries
• Defining a Password
Blocklist for Authenti-
cation Server Users
• Configure the Registry
Key for Windows Do-
main Users

Behavior Changes After En-
abling Identity and Authen-
tication Management

The method about binding the Support user is updated.

Managing Technical Users

8

PUBLIC

Identity and Authentication Management in SAP Business One
Document History

Topic

Extensions

Description

A new client type Daemon Service is added for registering a
new client in the SAP Business One Extension Single Sign-On
Manager.

Link to Related Section

• Registering a New Cli-

ent

• Walkthrough for Dae-

mon Service

1.7  Change Log 10.0 SP 2411

Topic

Description

Link to Related Section

Configuring Identity and
Authentication Manage-
ment in the System Land-
scape Directory

Behavior Changes After En-
abling Identity and Authen-
tication Management

The step about how to configure logout redirect URIs is added. Creating an Application in

the SAP IAS Admin Console
(Beta)

The note for the mobile service is updated.

Logging in as SAP Business
One Users

Logging in as SAP Business

One Users

Logging in as SAP Business

One Users

Password Never Expires
and Change Password at
Next Logon

Behavior Changes After En-
abling Identity and Authen-
tication Management

The behavior change for the fields Password Never Expires and
Change Password at Next Logon is added.

Limitations

Two limitations are added.

Limitations

1.8  Change Log 10.0 SP 2408

Topic

Introduction

Configuring Identity and
Authentication Manage-
ment in the System Land-
scape Directory

Description

Link to Related Section

Azure Active Directory (Azure AD) is renamed to Microsoft En-

Introduction

tra ID.

Azure Active Directory (Azure AD) is renamed to Microsoft En-

tra ID.

Adding Microsoft Entra ID
as an OIDC Identity Pro-
vider

Identity and Authentication Management in SAP Business One
Document History

PUBLIC

9

1.9  Change Log 10.0 FP 2405

Topic

Introduction

Reconfiguring Identity
and Authentication Man-
agement

Reconfiguring Identity
and Authentication Man-
agement

Reconfiguring Identity
and Authentication Man-
agement

Description

Link to Related Section

The link to the IAM guide for SAP Business One Cloud is added.

Introduction

A new step about deleting the parameters is added.

Adding a User for Log-
ging into the Authentication
Service

A new topic about resetting the password of B1SiteUser is
added.

Resetting the Password of
B1SiteUser

The topics about activating B1SiteUser in the authentication
service are restructured.

Activating B1SiteUser

1.10  Change Log 10.0 SP 2402

Topic

Description

The links to the administrator's guides are changed.

• Introduction
• Reconfiguring Identity
and Authentication

Management

Link to Related Section

• Introduction
• Renewing the Security

Certificate

• Changing the Port

Number for Authenti-

cation Service

10

PUBLIC

Identity and Authentication Management in SAP Business One
Document History

1.11  Change Log 10.0 SP 2311

Topic

Description

Link to Related Section

Reconfiguring Identity
and Authentication Man-
agement

• Updated the precedure in the topic Activating B1SiteUser

When It Is Locked.

• Updated the screenshots and procedures in the topic

Deleting the User.

• Updated the screenshots and procedures in the topic

Changing Client ID and Client Secret in the Authentication

Service.

• Adding a User for Log-
ging into the Authenti-

cation Service

Adding a User for Log-

ging into the Authenti-

cation Service
• Deleting the User
• Changing Client ID and
Client Secret in the Au-
thentication Service

1.12  Change Log 10.0 FP 2305

Topic

Description

Link to Related Section

Configuring Identity and
Authentication Manage-
ment in the System Land-
scape Directory

• Added a new topic Adding Okta as an OIDC Identity

• Adding Okta as an

Provider to Adding Identity Providers.

• Added a new topic Adding SAP IAS as an IODC Identity

Provider (Beta) to Adding Identity Providers.
• Added a new topic Deactivating Identity Providers
• Added a new topic Two-Factor Authentication for SAP

OIDC Identity Provider
• Adding SAP IAS as an
IODC Identity Provider

(Beta)

• Deactivating Identity

Business One Authentication Server Users to Adding Users.

Providers

• Added the description of the new checkbox Enable Two-
Factor Authentication to the Adding Users and Editing

Users topics.

• Updated the description for Company and User Code in

the Binding Users topic.

Reconfiguring Identity
and Authentication Man-
agement

Added a new topic Activating B1SiteUser When It Is Locked.

• Two-Factor Authentica-
tion for SAP Busi-

ness One Authentica-

tion Server Users

• Adding Users
• Editing Users
• Binding Users

Activating B1SiteUser When
it is Locked

Identity and Authentication Management in SAP Business One
Document History

PUBLIC

11

Topic

Description

Behavior Changes After En-
abling Identity and Authen-
tication ManagementActi-
vating B1SiteUser When It Is
Locked

• Added the newly supported components in the list of com-

ponents that support the authentication service
• Added a new note to the Logging in as Company Users

topic.

Link to Related Section

• Behavior Changes Af-
ter Enabling Identity

and Authentication

Management

• Added a new topic Changing Password from the Login

• Logging in as Company

Page.

• Added a new topic Binding Users in SAP Business One

Client.

• Added a new topic Single Logout (SLO).

Extensions

• Added a description of the single page apps to the Scopes

and Registering a New Client topics

• Added a new section Walkthrough for Single Page Apps
• Added a column about different connection methods via

Users

• Changing Password
from the Login Page
• Binding Users in SAP
Business One Client
• Single Logout (SLO)

• Scopes
• Registering a New Cli-

ent

• Walkthrough for Single

the Service Layer in different scenarios

Page Apps

• SL Connection Refer-

ences

1.13  Change Log 10.0 FP 2208

Topic

All topics

Description

First version.

12

PUBLIC

Identity and Authentication Management in SAP Business One
Document History

2

Introduction

The SAP Business One solution supports the identity and authentication management service. An identity
provider is a trusted provider that lets you use single sign-on (SSO) to access other websites. SSO enhances
usability by reducing password fatigue. It also provides better security by decreasing the potential attack
surface.

You can configure the identity providers and user bindings from the SAP Business One System Landscape
Directory (SLD) control center by using the following approaches:

• SAP Business One authentication service
• Microsoft Windows domain account authentication
• OpenID Connect (OIDC)

You can add an external identity provider by choosing the protocol OpenID Connect (OIDC). OIDC allows
clients to confirm an end user’s identity using authentication by an authorization server. With OIDC, you
can use a single and existing account (from identity providers such as Microsoft) to sign into SAP Business
One and further strengthen security by leveraging from IDP’s features, such as two-factor authentication
(2FA), without ever needing to create another username and password.
In this release, you can register the following external identity providers from the SLD control center:
• Active Directory Federation Service (AD FS)
• Microsoft Entra ID

 Note

Microsoft Entra ID is the new name for Azure Active Directory, Azure AD and AAD. For more
information, see https://learn.microsoft.com/en-us/entra/fundamentals/new-name

• Okta
• SAP Identity Authentication Service (IAS)

 Note

In this release, adding SAP IAS as an OIDC identity provider in SAP Business One is a beta feature.

When binding users in the SLD control center, you can perform the central user management actions, such as
resetting unified user passwords, and activating or deactivating user accounts, which effects all bound users
across companies in SAP Business One.

The identity and authentication management service is planned be rolled out in a phased manner.

In this release, the identity and authentication management service is supported by the following SAP Business
One products:

• SAP Business One
• SAP Business One, version for SAP HANA

As of 10.0 FP 2405, the IAM service is supported by the corresponding SAP Business One Cloud version. For
more information, see Identity and Authentication Management in SAP Business One Cloud.

Identity and Authentication Management in SAP Business One
Introduction

PUBLIC

13

This guide provides instruction on how to configure and enable the identity provider authentication services
for SAP Business One and SAP Business One, version for SAP HANA. It also documents the behavior changes
after enabling the identity provider authentication services, such as SAP Business One client login.

For information about the installation of the SAP Business One Authentication Service component, see the
Administrator's Guide:

SAP Business One Administrator's Guide

SAP Business One Administrator's Guide, version for SAP HANA

14

PUBLIC

Identity and Authentication Management in SAP Business One
Introduction

3  Configuring Identity and Authentication

Management in the System Landscape
Directory

To enable identity and authentication management, you need to access the SLD control center in a Web
browser to set up identity providers and users.

The overall configuration procedure of the identity and authentication management service is as follows:

1. Adding Identity Providers [page 17]

2. Adding Users [page 56]

3. Binding Users [page 61]

4. Activating Identity Providers [page 53]

This section provides information on how to manage identity providers and users in the SLD control center.

 Recommendation

To ensure that the IAM service works correctly, we highly recommend that you first add an identity provider
and 2 IDP users to carry out a test before binding more IDP users. You can perform the following steps
during the test:

1. Add an identity provider.

2. Add two IDP users.

3. Assign one user as a landscape administrator.

4. Bind another user to a company user.

5. Log in to the SLD contrl center with the landscape administrator’s account.

6. Log in to the SAP Business One client with the bound SAP Business One user.

 Recommendation

We recommend that you regularly back up the databases of the SLD and authentication service after
enabling identity and authentication management.

 Note

Make sure that you synchronize computer clocks within your landscape.

Time synchronization problem may cause errors during the authentication process.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

15

3.1  Managing Identity Providers

You typically use only one identity provider in SAP Business One, but you have the option to add more. This
section shows you how to add, delete an identity provider to your SLD control center.

The Identity Providers tab of the SLD control center displays all registered identity providers in SAP Business
One, including the SAP Business One authentication server, Active Directory Domain Services and other
external identity providers.

SAP Business One Authentication Server

The SAP Business One Authentication Server is a default identity provider. After installing SAP Business One,
you can find this option when logging into the SLD.

You cannot delete the registration of the SAP Business One authentication server.

Active Directory Domain Services

If you have enabled domain user authentication during the installation of the System Landscape Directory, you
can find this option when logging into the SLD.

You cannot delete the registration of the Active Directory Domain Services.

Prior to 10.0 FP 2208, SAP Business One supports Microsoft Windows domain single sign-on (SSO)
functionality. You can bind an SAP Business One user account to a Microsoft Windows domain account.

If you upgrade SAP Business One from a lower version to 10.0 FP 2208 or higher, after the upgrade you may
find a different status based on the different scenarios. For more information, see Windows Domain Single
Sign-On After Upgrades [page 130].

External Identity Providers

You can register external identity providers by choosing the protocol OpenID Connect (OIDC) in the SLD control
center.

You can delete the registered external IDPs.

The default status for a default or registered identity provider is Inactive. To enable the identity provider
authentication service, you need to change the status of the identity provider to Active by choosing Activate.

 Note

Before activating identity providers, make sure that you have created and bound IDP users to SAP Business
One company users across all companies. You cannot log into SAP Business One with company users after
activating the identity provider.

16

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

Related Information

Adding Identity Providers [page 17]

Deleting Identity Providers [page 52]

Activating Identity Providers [page 53]

3.1.1  Adding Identity Providers

In addition to the built-in identity providers, you can register external identity providers from the SLD control
center.

Prerequisites

• You have registered an application on the related IDP site.
• You have installed SAP Business One 10.0 FP 2208 or higher.

Context

In this release, you can register the following external identity providers from the SLD control center:

• Active Directory Federation Service (AD FS)
• Microsoft Entra ID

 Note

Microsoft Entra ID is the new name for Azure Active Directory, Azure AD and AAD. For more
information, see https://learn.microsoft.com/en-us/entra/fundamentals/new-name

• Okta
• SAP Identity Authentication Service (IAS)

 Note

In this release, adding SAP IAS as an OIDC identity provider in SAP Business One is a beta feature.

For more details about how to add the respective identity providers , see the relevant topics in this section.

Procedure

1. Log into the SLD control center.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

17

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the following information and then choose OK.
• Protocol: Select the protocol for the connection between SAP Business One and the identity provider.

Choose OIDC for an external identity provider.
• IDP Alias: Define an alias for the identity provider.

 Caution

The alias starts with b1- and may only use the following characters:
• English letters (a-z/A-Z)
• Numbers (0-9)
• Underscores (_)
• Hyphen (-)

• Redirect URI: The redirect URI of SAP Business One, where authentication responses can be sent and
received by SAP Business One. It must exactly match the redirect URI you registered on the IDP site.
The redirect URI is created once you define an IDP alias. The address is https://<Server
Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP Alias>/endpoint.

• IDP Display Name: Specify the identity provider’s display name.
• OIDC Discovery URL: Copy the discovery URL (metadata document) from the related IDP site and

paste it here. The path is …/.well-known/openid-configuration.
OpenID Connect describes a metadata document that contains most of the information required for
an app to carry out a sign-in. This includes information such as the URL to use and the location of the
service’s public signing keys.

• Client ID: Copy the client ID from the related IDP site and paste it here. The client ID is assigned to your

application when you register the app in the IDP site. It is a public identifier for apps.

• Client Secret: Copy the client secret from the related IDP site and paste it here. The client secret is

assigned to your application when you register the app on the IDP site. It is a secret known only to the
application and the authorization server.

• Claim Name: Enter the claim name you specified when registering the application in the IDP site.

When the IDP forwards an ID token to the SAP Business One authentication service, the claim name of
the ID token will be used to identify the unique user name in SAP Business One.

• Email Domain: Enter the email domain name of the IDP.

The email domain is used to identify IDPs. If you activate multiple IDPs, you will be directed to the
related IDP login page when you log into SAP Business One with one IDP user account.

18

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

4. Choose OK to close the window.

Related Information

Adding AD FS as an OIDC Identity Provider [page 19]

Adding Microsoft Entra ID as an OIDC Identity Provider [page 30]

Adding Okta as an OIDC Identity Provider [page 38]

Adding SAP IAS as an OIDC Identity Provider (Beta) [page 45]

3.1.1.1

Adding AD FS as an OIDC Identity Provider

The Active Directory Federation Service (AD FS) is a single sign-on (SSO) feature developed by Microsoft that
provides safe, authenticated access to any domain, device, web application, or system within the organization’s
active directory (AD), as well as approved third-party systems.

To enable login for users with an AD FS account, you need to create an application group in AD FS management
and register the AD FS in the SAP Business One SLD control center.

To enable single sign-on (SSO) for users with an AD FS account, you can set up the browser to use the Windows
Integrated Authentication (WIA) with AD FS.

Related Information

Creating a Redirect URI from the SLD Control Center [page 20]

Creating an Application Group in AD FS Management [page 21]

Creating the OIDC Discovery URL [page 25]

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

19

Importing the AD FS Certificate to SAP JVM [page 26]

Registering the AD FS in the SLD Control Center [page 27]

Enabling Browser Windows Integrated Authentication with AD FS [page 29]

3.1.1.1.1

Creating a Redirect URI from the SLD Control
Center

Prerequisites

You have installed SAP Business One version for 10.0 FP 2208 or higher.

Procedure

1. Log into the SLD control center.

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the alias of the AD FS in IDP Alias.

 Caution

The alias starts with b1- and may only use the following characters:
• English letters (a-z/A-Z)
• Numbers (0-9)
• Underscores (_)
• Hyphen (-)

Results

After entering the IDP alias, the following redirect URI is created automatically:

https://<Server Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP Alias>/endpoint

For example: https://<IP address>:40020/auth/realms/sapb1/broker/b1-SME/endpoint

Copy the redirect URI value to your notepad. It will be used later as the value for Redirect URI during the
creation of the application group in the AD FS.

20

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.1.1.1.2

Creating an Application Group in AD FS
Management

Prerequisites

• You have installed AD FS in Windows Server 2016 or 2019.
• You have created a redirect URI from the SAP Business One SLD control center.

Procedure

1.

In Server Manager, select Tools, and then select AD FS Management.

2.

In AD FS Management, right-click on Application Groups and select Add Application Group.

3. On the Application Group Wizard Welcome screen:

1. Enter the name of your application. For example, mocca2.com.

2. Under Standalone applications, select the Server application template.

3. Choose Next.

4. On the Application Group Wizard Server Application screen:

1. Copy the Client Identifier value to your notepad. It will be used later as the value for the Client ID in the

SLD control center.

2. Paste the redirect URI that has been created in the SLD control center to the Redirect URI, and then

choose Add.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

21

3. Choose Next.

5. On the Application Group Wizard Configure Application Credentials screen:

1. Select Windows Integrated Authentication and choose Select….

2. Under Enter the object name to select, enter the name of a domain admin user. Choose OK.

22

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3. Choose Next, and then Next to complete the application registration wizard.

4. Choose Close.

6.

In the Application Groups window, now you can see the newly created application group.

7. Go to create a client secret by performing the following steps:

1.

2.

In the Application Groups window, select the newly created application group.

In the <Application Group Name> Properties window, in the Applications area, select <Application
Group Name> – Server application.

3.

In the <Application Group Name> – Server application Properties window, select the Confidential tab.

4. Choose Create client secret.

5.

In the Create Client Secret window, choose Copy to Clipboard.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

23

6. Paste the client secret to your notepad. It will be used later for the Client Secret in the SLD control

center.

7. Choose Apply, then choose OK.

24

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

Troubleshooting Wrong Client Credentials

If the services encounter wrong client information or authentication issues, reset the client secret as follows:

1.

2.

In the Application Groups window, select the application group.

In the <Application Group Name> Properties window, in the Applications area, select <Application Group
Name> – Server application Properties.

3.

In the Confidential tab, select Reset client secret.

4. Copy and paste the client secret to Client Secret in the SLD control center.

5. Choose Apply, then choose OK.

3.1.1.1.3

Creating the OIDC Discovery URL

Prerequisites

• You have installed the AD FS in Windows Server 2016 or 2019.
• You have your host name and domain name.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

25

Procedure

1.

In AD FS Management, choose Service → Endpoints.

2. On the Endpoints screen, under the OpenID Connect area, find the row for the type of OpenID Connect

Discovery.

3. Copy the URL path (for example, adfs/.well-known/openid-configuration) from this row.

4. Add https://<Host name>.<Domain name>/ before the URL path you copied in the last step. For
example, https://computer1/latte.com/adfs/.well-known/openid-configuration.

5. Copy the full URL path to your notepad. It will be used later for the OIDC Discovery URL in the SLD control

center.

3.1.1.1.4

Importing the AD FS Certificate to SAP JVM

Context

If you use a purchased AD FS certificate, you can ignore this step and go on to register the AD FS in the SLD
control center now.

If you use a self-signed certificate, you need to import the AD FS certificate to SAP JVM.

26

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

 Note

No matter which certificate you use, make sure the AD FS certificate is issued to the full qualified domain
name (FQDN).

Procedure

1. Copy the certificate to your local folder.

2. Execute the following script:

"/<Installation Folder>/SAPBusinessOne/Common/sapmachine_11/bin/keytool"
-importcert -alias "adfs" -keystore "/<Installation Folder>/SAPBusinessOne/
Common/sapmachine_11/lib/security/cacerts" -storepass changeit -file "/home/
adfs.cer"

Results

The AD FS certificate is imported to SAP JVM. You can now register the AD FS in the SLD control center.

 Note

If you intend to restart the SAP Business One Server Tools Authentication Service, perform the following
steps:

• On a Windows machine, restart this service from the Services app.
• On a Linux machine, perform the following commands: systemctl restart sapb1servertools-

authentication.service.

3.1.1.1.5

Registering the AD FS in the SLD Control Center

Prerequisites

• You have created an application group in AD FS Management.
• You have created an OIDC discovery URL.
• You have created a client secret in AD FS.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

27

Procedure

1. Log into the SLD control center.

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the following information and then choose OK.
• Protocol: Choose OIDC.
• IDP Alias: Enter the IDP alias you defined previously.
• Redirect URI: The redirect URI is created automatically after you enter the IDP alias.
• IDP Display Name: Specify an IDP name for the registration.
• OIDC Discovery URL: Copy the OIDC discovery URL that you created.
• Client ID: Copy the client ID that you got in AD FS.
• Client Secret: Copy the client secret that you created in AD FS.

If the services encounter wrong client information or authentication issues, reset the client secret in
AD FS. For more information about how to reset the client secret, see Troubleshooting Wrong Client
Credentials in Creating an Application Group in AD FS Management [page 21].

• Claim Name: Enter upn
• Email Domain: Enter the domain name.

4. Choose OK to close the window.

When AD FS is successfully registered in the SLD control center, you can see its information in the table on
the Identity Providers tab. The default status of the registered IDP is Inactive. If you want to activate the IDP,
see Activating Identity Providers [page 53] to get more information.

28

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.1.1.1.6

Enabling Browser Windows Integrated
Authentication with AD FS

Configure the browser to use Windows Integrated Authentication (WIA) with AD FS, to enable single sign-on
(SSO) for SAP Business One components, such as the SAP Business One client, Web client, and mobile
service. The configuration is not required for using AD FS as an identity provider.

Prerequisites

 Caution

Enabling this setting on public computers poses a risk, as it may permit unauthorized access to SAP
Business One company data.

Make sure all servers are synchronized to the same time.

Procedure

1. On the server where the AD FS is installed, add the required browser user agents to the AD FS

configuration.

You can use the following command to enable WIA with AD FS for Google Chrome and the latest version of
Microsoft Edge.

Set-AdfsProperties -WIASupportedUserAgents ((Get-ADFSProperties | Select
-ExpandProperty WIASupportedUserAgents) + "Chrome")

2. Set service principal names (SPNs) for AD FS using the following command:

setspn -A HTTP/${ADFS FQND} ${Domain user}

3. Restart the AD FS service.

4. On the server hosting the browsers, make sure that WIA is enabled in your browser.

For Internet Explorer and Google Chrome, select the checkbox Enable Integrated Windows Authentication

under

Internet Options

 Advanced

 Security .

5. Configure client computers to trust the account federation server. For more information, see Configure

Client Computers to Trust the Account Federation Server

.

Results

After binding AD FS users to SAP Business One company users and activating AD FS in the SLD control center,
you can log in to SAP Business One components with SSO. For more information about login scenarios, see
Single Sign-On After Enabling Browser Windows Integrated Authentication with AD FS [page 131].

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

29

If you want to disable browser WIA with AD FS, run the following command on the AD FS server, and restart the
AD FS service:

Set-ADFSProperties -WIASupportedUserAgents @("MSAuthHost/1.0/In-Domain",
"MSIE 6.0", "MSIE 7.0", "MSIE 8.0", "MSIE 9.0", "MSIE
10.0", "Trident/7.0", "MSIPC", "Windows Rights Management Client",
"MS_WorkFoldersClient","=~Windows\s*NT.*Edge")

3.1.1.2

Adding Microsoft Entra ID as an OIDC Identity
Provider

The Microsoft Entra ID is an enterprise identity service that provides single sign-on, multifactor authentication,
and conditional access to guard against cybersecurity attacks.

To enable login for users with an Microsoft Entra ID, you need to register an application in Microsoft Entra ID
and register Microsoft Entra ID in the SAP Business One SLD control center.

 Note

Microsoft Entra ID is the new name for Azure Active Directory, Azure AD and AAD. For more information,
see https://learn.microsoft.com/en-us/entra/fundamentals/new-name

Related Information

Creating a Redirect URI from the SLD Control Center [page 30]

Registering an Application on Microsoft Entra ID [page 31]

Adding Optional Claims on Microsoft Entra ID [page 33]

Creating a Client Secret on Microsoft Entra ID [page 34]

Copying the Discovery URL and Client ID from Microsoft Entra ID [page 36]

Registering Microsoft Entra ID in the SLD Control Center [page 36]

3.1.1.2.1

Creating a Redirect URI from the SLD Control
Center

Prerequisites

You have installed SAP Business One version for 10.0 FP 2208 or higher.

30

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

Procedure

1. Log into the SAP Business One SLD control center.

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the alias of the Microsoft Entra ID in IDP Alias.

 Caution

The alias starts with b1- and may only use the following characters:
• English letters (a-z/A-Z)
• Numbers (0-9)
• Underscores (_)
• Hyphen (-)

Results

After entering the IDP alias, the following redirect URI is created automatically:

https://<Server Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP Alias>/endpoint

For example: https://<IP address>:40020/auth/realms/sapb1/broker/b1-azure/endpoint

Copy the redirect URI value to your notepad. It will be used later as the value for the Redirect URI during the
registration of the application on Microsoft Entra ID.

3.1.1.2.2

Registering an Application on Microsoft Entra ID

Prerequisites

• You have an Microsoft Entra ID account that has an active subscription.
• You have created a redirect URI from the SAP Business One SLD control center.

Procedure

1. Sign in to the Azure Portal

.

2. Search for and select Microsoft Entra ID.

3. Under Manage, select App registrations → New registration.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

31

4. Enter a display Name for your application. You can change the display name at any time.

5. Under Supported account types, specify who can use the application. You can select the default one.

6. For the Redirect URI (optional), select Web and enter the redirect URI you previously created from the SAP

Business One SLD control center.

7. Choose Register.

8. You can now see the new application under All applications .

32

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.1.1.2.3

Adding Optional Claims on Microsoft Entra ID

After registering an application, you need to add the upn claims from Microsoft Entra ID.

Prerequisites

• You have an Azure account that has an active subscription.
• You have registered an application on Microsoft Entra ID.

Procedure

1.

In Microsoft Entra ID, under Manage, select App registrations.

2. Select the application you want to add upn claims for in the list.

3. From the Manage section, select Token configuration.

4. Select Add optional claim.

5. For the Token type, select ID.

6. Select the optional claim upn.

7. Choose Add.

You do not need to select the checkbox Turn on the Microsoft Graph profile permission (required for claims
to appear in token).

You can now find a new row for the claim upn with the token type ID.

You need to continue the following steps to add another token type of upn.

8. Select Add optional claim.

9. For the Token type, select Access.

10. Select the optional claim upn.

11. Choose Add.

You do not need to select the checkbox Turn on the Microsoft Graph profile permission (required for claims
to appear in token).

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

33

12. You can now find another row for the claim upn with the token type Access.

3.1.1.2.4

Creating a Client Secret on Microsoft Entra ID

You need to create a client secret that will be used later as the value for the Client Secret in the SLD control
center.

Prerequisites

• You have an Azure account that has an active subscription.
• You have registered an application on Microsoft Entra ID.

Procedure

1.

In the Microsoft Entra ID, under Manage, choose App registrations.

2. Select the application you want to create a client secret for in the list.

3.

4.

In the left menu, choose Overview.

In the right panel, under Essentials, in Client credentials, choose Add a certificate or secret.

5. Under Client secret tab, choose New client secret.

6. Enter a description for this client secret.

7. Define a valid period.

34

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

 Note

Please note that the valid period cannot be changed on Microsoft Entra ID once you define it. If you
want to extend the valid period, you can only go to the SAP Business One Authentication Service to
make the change.

8. Choose Add.

9.

In the newly added row, copy the secret value (not secret ID) to the clipboard.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

35

3.1.1.2.5

Copying the Discovery URL and Client ID from
Microsoft Entra ID

You can now copy and record the OIDC discovery URL and client ID from Microsoft Entra ID. The information
will be used later when you register Microsoft Entra ID in the SLD control center.

Procedure

1. Copy OpenID Connect metadata document from Endpoints. It will be used later as the value for the OIDC

Discovery URL in the SLD control center.

1.

In the Microsoft Entra ID, under Manage, choose App registrations.

2. Select the application you want to copy information for in the list.

3.

4.

In the left menu, choose Overview.

In the right panel, choose Endpoints.

5. Copy the URL of OpenID Connect metadata document.

2. Copy Application (client) ID. It will be used later as the value for the Client ID in the SLD control center.

1.

In the Microsoft Entra ID, under Manage, choose App registrations.

2. Select the application you want to copy information for in the list.

3.

4.

In the left menu, choose Overview.

In the right panel, under Essentials, copy the value of the Application (client) ID.

3.1.1.2.6

Registering Microsoft Entra ID in the SLD Control
Center

Prerequisites

• You have created an application on Microsoft Entra ID.
• You have added the upn claims from Microsoft Entra ID.
• You have created the client secret from Microsoft Entra ID.

Procedure

1. Log into the SLD control center.

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the following information and then choose OK.

36

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

• Protocol: Choose OIDC.
• IDP Alias: Enter the IDP alias you defined previously.
• Redirect URI: The redirect URI is created automatically after you enter the IDP alias.
• IDP Display Name: Specify an IDP name for the registration.
• OIDC Discovery URL: Paste the OIDC discovery URL that you previously copied from Microsoft Entra

ID.

• Client ID: Paste the client ID that you previously copied from Microsoft Entra ID.
• Client Secret: Paste the client secret that you previously created in Microsoft Entra ID.

 Note

Paste the value of the client secret (not secret ID) here.

• Claim Name: Enter upn.
• Email Domain: Enter the domain name.

4. Choose OK to close the window.

When AD FS is successfully registered in the SLD control center, you can see its information in the table on
the Identity Providers tab. The default status of the registered IDP is Inactive. If you want to activate the IDP,
see Activating Identity Providers [page 53] to get more information.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

37

3.1.1.3

Adding Okta as an OIDC Identity Provider

Okta is an enterprise-grade, identity management service, built for the cloud, but compatible with many
on-premise applications.

To enable login for users with a Okta account, you need to create an app integration in the Okta Admin Console
and register Okta in the SAP Business One SLD control center.

Related Information

Creating a Redirect URI from the SLD Control Center [page 38]

Creating an App Integration in the Okta Admin Console [page 39]

Copying the Client ID and Client Secret [page 41]

Creating the OIDC Discovery URL [page 43]

Registering Okta in the SLD Control Center [page 44]

3.1.1.3.1

Creating a Redirect URI from the SLD Control
Center

Prerequisites

You have installed SAP Business One version for 10.0 FP 2305 or higher.

Procedure

1. Log into the SAP Business One SLD control center.

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the alias of the Okta in IDP Alias.

 Caution

The alias starts with b1- and may only use the following characters:
• English letters (a-z/A-Z)
• Numbers (0-9)
• Underscores (_)
• Hyphen (-)

38

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

Results

After entering the IDP alias, the following redirect URI is created automatically:

https://<Server Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP Alias>/endpoint

For example: https://<IP address>:40020/auth/realms/sapb1/broker/b1-okta/endpoint

Copy the redirect URI value to your notepad. It will be used later as the value for Sign-in redirect URIs and
Sign-out redirect URIs during the creation of the new app integration in Okta Admin Console.

3.1.1.3.2

Creating an App Integration in the Okta Admin
Console

Prerequisites

• You have an active Okta administrator account.
• You have created a redirect URI from the SAP Business One SLD control center.

Procedure

1. Sign in to your Okta Admin Console

 with your administrator account.

2.

3.

In the Okta Admin Console, in the left menu, choose  Applications Applications .

In the right panel, choose Create App Integration.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

39

4. On the Create a new app integration screen, select OIDC - OpenID Connect and Web Application, and

choose Next.

5. On the New Web App Integration screen:

1. Enter the name of your application, for example, B1Okta.

2. Under Sign-in rediret URIs, paste the following redirect URI that has been created in the SLD

control center: https://<Server Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP
Alias>/endpoint

3. Under Sign-out redirect URIs, paste the redirect URI that has been created in the SLD control center

and follow the URI with /logout_response as follows:
https://<Server Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP Alias>/
endpoint/logout_response

4. Under Assignments, select Allow everyone in your organization to access.

5. Choose Save.

40

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.1.1.3.3

Copying the Client ID and Client Secret

Context

You can now copy and record the client ID and client secret from the Okta Admin Console. The information will
be used later when you register Okta in the SLD control center.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

41

Procedure

1.

In the Okta Admin Console, in the left menu, choose  Applications

 Applications .

2.

In the right panel, select the application (for example, B1Okta) that you want to copy information from.

3. On the General tab, under Client Credentials, copy the client ID to your notepad. It will be used later for the

client ID in the SLD control center.

4. Under CLIENT SECRETS, copy the client secret to your notepad. It will be used later for the client secret in

the SLD control center.

42

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.1.1.3.4

Creating the OIDC Discovery URL

Prerequisites

You have your Okta domain name.

Procedure

1.

In the Okta Admin Console, choose your user account in the upper right corner.

2. Copy your Okta domain (<ID>.okta.com).

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

43

3. On your notepad, paste the Okta domain into the following URL:

https://<yourOktaDomain>/.well-known/openid-configuration

For example, https://<ID>.okta.com/.well-known/openid-configuration

The URL will be used later for the OIDC Discovery URL in the SLD control center.

3.1.1.3.5

Registering Okta in the SLD Control Center

Prerequisites

• You have created an app integration in the Okta Admin Console.
• You have copied the client ID and client secret from the Okta Admin Console.
• You have created the OIDC discovery URL.

Procedure

1. Log into the SLD control center.

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the following information and then choose OK.
• Protocol: Choose OIDC.
• IDP Alias: Enter the IDP alias you defined previously.
• Redirect URI: The redirect URI is created automatically after you enter the IDP alias.
• IDP Display Name: Specify an IDP name for the registration.
• OIDC Discovery URL: Paste the OIDC discovery URL that you previously created.

44

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

• Client ID: Paste the client ID that you previously copied from the Okta Admin Console.
• Client Secret: Paste the client secret that you previously copied from the Okta Admin Console.
• Claim Name: Enter email
• Email Domain: Enter your Okta domain name.

4. Choose OK to close the window.

When Okta is successfully registered in the SLD control center, you can see its information in the table on
the Identity Providers tab. The default status of the registered IDP is Inactive. If you want to activate the IDP,
see Activating Identity Providers [page 53] for more information. .

3.1.1.4

Adding SAP IAS as an OIDC Identity Provider (Beta)

The Identity Authentication Service is a public cloud solution to enable single sign-on for SAP Cloud
applications. It provides services for authentication, single sign-on, risk-based authentication, on-premise
integration and user self-services, such as registration or password reset for employees, partners, and
consumers.

To enable login for users with an SAP account, you need to create an application in the SAP IAS administration
console and register SAP IAS in the SAP Business One SLD control center.

 Note

Currently, adding SAP IAS as an OIDC identity provider in SAP Business One is a beta feature.

Beta features aren't part of the officially delivered scope that SAP guarantees for future releases. For more
information, see Important Disclaimers and Legal Information.

Related Information

Creating a Redirect URI from the SLD Control Center (Beta) [page 46]

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

45

Creating an Application in the SAP IAS Admin Console (Beta) [page 47]

Creating Client ID and Client Secret (Beta) [page 49]

Registering SAP IAS in the SLD Control Center (Beta) [page 51]

3.1.1.4.1

Creating a Redirect URI from the SLD Control
Center (Beta)

Prerequisites

You have installed SAP Business One, version for 10.0 FP 2305 or higher.

Procedure

1. Log into the SAP Business One SLD control center.

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the alias of the SAP IAS in IDP Alias.

 Caution

The alias starts with b1- and may only use the following characters:
• English letters (a-z/A-Z)
• Numbers (0-9)
• Underscores (_)
• Hyphen (-)

Results

After entering the IDP alias, the following redirect URI is created automatically:

https://<Server Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP Alias>/endpoint

For example: https://<IP address>:40020/auth/realms/sapb1/broker/b1-SAPIAS/endpoint

Copy the redirect URI value to your notepad. It will be used later as the value for during the configuration of the
new application in SAP IAS.

46

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.1.1.4.2

Creating an Application in the SAP IAS Admin
Console (Beta)

Prerequisites

• You have an active SAP IAS administrator account.
• You have created a redirect URI from the SAP Business One SLD control center.

Procedure

1. Log on to the administration console for the SAP Identity Authentication Service with your administrator

account.

For more information about SAP IAS, see Identity Authentication Service Documentation on the SAP Help
Portal.

In the admin console, in the left menu, choose  Applications & Resources Applications .

In the right panel, choose Create.

2.

3.

4. On the Create Application screen,

1.

In the Display Name field, enter the name of your application (for example, B1-IAS ).

2. Leave the other fields empty and choose Save.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

47

You can now see the new application under Charged Applications.

5. Choose the new application, and in the right panel, configure the protocol.

1. On the Trust tab, under Single Sign-On, choose Protocol.

2.

In the new screen, select OpenID Connect to replace the default option SAML 2.0 and choose Save.
You can now see the protocol is OpenID Connect.

6. Configure the OpenID Connect.

1. On the Trust tab, under Single Sign-On, choose OpenID Connect Configuration.

2.

In the OpenID Connect Configuration screen, define the name for the OpenID Connect (for example,
B1-OIDC).

3. Under Redirect URIs, choose Add and paste the following redirect URI that has been created in the SLD

control center:
https://<Server Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP Alias>/
endpoint
For example: https://<IP address>:40020/auth/realms/sapb1/broker/b1-SAPIAS/
endpoint

48

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

4. Under Post Logout Redirect URIs, choose Add and paste the redirect URI that has been created in the

SLD control center and follow the URI with /logout-response as follows:
https://<Server Address>:<Port>/auth/realms/sapb1/broker/b1-<IDP Alias>/
endpoint/logout_response
For example, https://<IP address>:40020/auth/realms/sapb1/broker/b1-SAPIAS/
endpoint/logout_response

3.1.1.4.3

Creating Client ID and Client Secret (Beta)

Context

You can now create, copy and record the client ID and client secret from the SAP IAS administration console.
The information will be used later when you register SAP IAS in the SLD control center.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

49

Procedure

1.

In the admin console, in the left menu, choose  Applications & Resources Applications .

2.

In the right panel, select the application (for example, B1-IAS).

3. On the Trust tab, under Application APIs, choose Client Authentication.

4.

In the Client Authentication screen, Choose Add for Secrets.

5.

In the Add Secret screen, you can add the description for the new secret (for example, B1-OIDC) and
choose Save.

 Note

You don't need to make changes to other default settings.

50

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

6.

In the popup screen, copy the client ID and client secret to your notepad. They will be used later for the
client ID and client secret in the SLD control center.

3.1.1.4.4

Registering SAP IAS in the SLD Control Center
(Beta)

Prerequisites

• You have created an application in the SAP IAS administration console.
• You have copied the client ID and client secret from the SAP IAS administration console.

Procedure

1. Log into the SLD control center.

2. On the Identity Providers tab, choose Add.

3.

In the Add Identity Provider window, specify the following information and then choose OK.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

51

• Protocol: Choose OIDC.
• IDP Alias: Enter the IDP alias you defined previously.
• Redirect URI: The redirect URI is created automatically after you enter the IDP alias.
• IDP Display Name: Specify an IDP name for the registration.
• OIDC Discovery URL: Enter the OIDC discovery URL. The format of the discovery URL is https://

<Server IP>:<Port Number>/.well-known/openid-configuration

 Note

When port number 443 is used, the format of the discovery URL is https://<Server
IP>/.well-known/openid-configuration

The default port number 443 is optional.

• Client ID: Paste the client ID that you previously copied from the SAP IAS admin console.
• Client Secret: Paste the client secret that you previously copied from the SAP IAS admin console.
• Claim Name: Enter mail
• Email Domain: Enter sap.com

4. Choose OK to close the window.

When SAP IAS is successfully registered in the SLD control center, you can see its information in the table
on the Identity Providers tab. The default status of the registered IDP is Inactive. If you want to activate the
IDP, see Activating Identity Providers [page 53] to get more information.

3.1.2  Deleting Identity Providers

Prerequisites

You have deleted all relevant IDP users for the identity provider from the SLD control center.

52

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

Context

You can delete the registered external identity providers from the SLD control center.

 Note

You cannot delete the identity providers SAP Business One Authentication Server and Active Directory
Domain Services.

Procedure

1. Log into the SAP Business One SLD control center.

2. On the Identity Providers tab, select the identity provider you want to delete and choose Delete.

Related Information

Deleting Users [page 63]

3.1.3  Activating Identity Providers

Prerequisites

• You have added the identity provider in the SLD control center.
• You have created and bound IDP users to SAP Business One company users across all companies.
• You have set at least one user of the to-be-activated identity provider as a landscape administrator.
• You have adopted the IDP properly for add-ons.

Context

The default status of an identity provider is Inactive. To enable the identity provider authentication service, you
need to activate at least one identity provider.

 Recommendation

To manage it more easily, we recommend that you activate only one identity provider for your SAP Business
One.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

53

Procedure

1. Log into the SAP Business One SLD control center.

2. On the Identity Providers tab, select the identity provider you want to activate and choose Activate.

3.

In the Confirmation window, choose Yes.

Related Information

Activating Identity Providers [page 53]

Adding Users [page 56]

Binding Users [page 61]

3.1.4  Deactivating Identity Providers

Context

To disable an identity provider, you need to deactivate it from the SLD control center.

When logging into the SLD control center with a landscape administrator’s account, you can deactivate any
other identity providers, except the current administrator’s identity provider. As the landscape administrator,
you cannot change your own role to SAP Business One User.

 Note

If only the SAP Business One Authentication Server is active, you can deactivate it with its landscape
administrator account.

Procedure

1. Log into the SAP Business One SLD control center.

2. On the Identity Providers tab, select the identity provider you want to disable and choose Deactivate.

3.

In the Confirmation window, choose Yes.

54

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.2  Managing Identity Provider Users

In the SLD control center, you can manage the users of identity providers and bind them to SAP Business One
company users.

SAP Business One Authentication Server User

B1SiteUser is the super user of the SAP Business One authentication server. It was created during the
installation of the SLD. When you log into the SLD, you can find B1SiteUser on the Users tab.

B1SiteUser is a default landscape admin user. You can change the status and password of B1SiteUser.

You can also add other users for the SAP Business One authentication server in the SLD control center.

 Note

The default password expiration period for users of the SAP Business One authentication server is set
to 180 days. Upon logging in with expired user accounts, users will receive a prompt to change their
passwords. The default expiration period can be modified via the authentication service console. For more
information, see SAP Note 3542302

.

Microsoft Windows Domain User

You can add Windows domain users if the Active Directory Domain Service is available on the Identity Providers
tab.

You can change the statuses of Windows domain users, or remove domain users, from the table.

 Note

If you upgrade SAP Business One from a lower version to 10.0 FP 2208 (or higher) and in the lower version,
you have bound Windows domain users to SAP Business One company users, after the updates you can
find the bound users on the Users tab.

Other External Identity Provider Users

You can add other external identity provider users if you have registered the relevant identity providers on the
Identity Providers tab.

You can change the status or remove external IDP users from the table.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

55

 Note

Once you bind IDP users to SAP Business One company users, you cannot log into SAP Business One with
the company user accounts.

Related Information

Adding Users [page 56]

Editing Users [page 60]

Binding Users [page 61]

Unbinding Users [page 65]

Deleting Users [page 63]

Copying User Mappings [page 63]

3.2.1  Adding Users

Prerequisites

• For external IDP users, you have registered the relevant identity provider on the Identity Providers tab.
• For external IDP users, you have created the user account on the identity provider site.

Procedure

1. Log into the SLD control center.

2. On the Users tab, choose Add.

3.

In the Add User window, specify the following information and then choose OK.
• Identity Provider: Select an identity provider for the user. You can find the identity provider as long as

you registered it on the Identity Providers tab.

• Domain: Enter a domain name.
• User Name: Define a user name.

For an SAP Business One authentication server user, you need to make sure the user name starts with
a letter and contains only the following characters:
• Letters
• Digits
• Underscore symbols (_)

56

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

• Dots (.)
When adding a Microsoft Windows domain user, the SLD will verify if the user already exists in Active
Directory Domain Services (AD DS). If the user does not exist in AD DS, you can choose to stop or
continue adding the user.
For all external identity provider users, you can only enter an email address as a user name. The email
address must contain the email domain of the identity provider.

• Password: Define a password for the SAP Business One user and confirm the password. It is only

visible when you select SAP Business One Authentication Server.
The user will be required to change the password at the next login.

 Note

You can only define and change a password for a user of the SAP Business One authentication
server. For other IDP users, you need to log into the relevant IDP sites to change the account
passwords.

• Landscape Administrator: If you want to assign the role of Landscape Administrator to the user,

select this checkbox. The landscape administrator serves as a landscape-level authentication for
performing various administrative tasks, such as all operations performed in the SLD control center,
accessing and performing operations in Web-based service control centers (for example, job service,
Administration Console of the analytics platform).
If you don’t select this checkbox, the default role of the user is SAP Business One User.

 Note

You cannot bind a landscape admin user to an SAP Business One company user.

• Inactive: It is only visible when you add a user for SAP Business One authentication server. By default,
the newly added users are active. When you select this checkbox, you cannot log into SAP Business
One with this user account.

• Enable Two-Factor Authentication: It is only visible when you add a user for the SAP Business

One authentication server. It is automatically selected when you select the checkbox Landscape
Administrator (you can manually deselect Enable Two-Factor Authentication for a landscape
administrator).
For more information about two-factor authentication, see Two-Factor Authentication for SAP
Business One Authentication Server Users [page 58].

 Note

You cannot enable two-factor authentication for B1SiteUser.

Related Information

Adding Identity Providers [page 17]

Two-Factor Authentication for SAP Business One Authentication Server Users [page 58]

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

57

3.2.1.1

Two-Factor Authentication for SAP Business One
Authentication Server Users

Context

Two-factor authentication (2FA) is an authentication process that requires two different authentication factors
to establish identity. In SAP Business One, you can enable two-factor authentication for a user of the SAP
Business One authentication server (except for B1SiteUser) . If you enabled two-factor authentication for a
user of the SAP Business One authentication server, you need to provide the user password and a one-time
password (OTP) when logging on to SAP Business One.

At the first logon, you need to set up the Mobile Authenticator to activate your account.

Procedure

1.

Install one of the following applications on your mobile.
• FreeOTP
• Google Authenticator

2. Open the application and scan the barcode on the screen.

3. Enter the one-time code provided by the application and click Submit to finish the setup.

You can provide a Device Name to help you manage your OTP devices.

58

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

Results

From the next login, you just need to enter the one-time code upon the completion of the user name password
authentication.

You can disable the two-factor authentication from the SLD control center. After deselecting the checkbox
Enable Two-Factor Authentication, you don't need to enter the one-time code from the next login. For more
information, see Editing Users [page 60].

3.2.2  Importing Users

You can bulk-import AD DS users and other external IDP users by uploading a CSV file.

Prerequisites

You have prepared a CSV file to be used for importing IDP users. For more information, see SAP Note
3552513

.

Procedure

1. Log into the SLD control center.

2. On the Users tab, choose Import.

3.

In the Import User window, specify the following information:
• Identity Provider: Select an identity provider for the user. You can find the identity provider as long as

you registered it on the Identity Providers tab.

 Note

Users of the SAP Business One authentication server cannot be imported. You need to manually
add the authentication server users by choosing Add on the Users tab.

• Server: Select a server.
• Path to CSV File: Choose the CSV file that you will upload.

4. Choose Upload. The Validation Results window pops up.

You can export the validation results to a CSV file by choosing Export Results.

 Note

You must follow the error messages to resolve any problems before proceeding to the next step.

5. Choose Import.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

59

Results

You can now find the imported users in the table on the Users tab.

3.2.3  Editing Users

Procedure

1. Log into the SLD control center.

2. On the Users tab, select the user you want to edit and choose Edit.

3.

In the Edit User window, you can change the following information:
• Landscape Administrator: If you want to assign the role of Landscape Administrator to the user,

select this checkbox. The landscape administrator serves as a landscape-level authentication for
performing various administrative tasks, such as all operations performed in the SLD control center,
accessing, and performing operations in Web-based service control centers (for example, job service,
Administration Console of the analytics platform).
If you have bound the user to company users, you cannot assign the role of Landscape Administrator to
the user.

 Note

You cannot deselect this checkbox for the default B1SiteUser.

• Inactive

After changing the status to Inactive, you cannot log into SAP Business One with this user account.
You can only deactivate SAP Business One authentication server users except the default user
B1SiteUser.

 Note

For Windows domain users and other external IDP users, the default statutes in the SLD control
center are Active and cannot be changed. The user statuses in the SLD may not reflect the real
state (active or inactive) in the identity provider site-level user management system since the SLD
currently does not capture the user state change from external IDP sites.

If the user state in the IDP site is inactive, you cannot log into SAP Business One with the user
account, even though the status in the SLD is active and you have bound it with company users.

• Change Password

 Note

You can only change the password for users of the SAP Business One authentication server, and
the user will be required to change the password at the next login.

If you want to change passwords for external IDP users, you may go to the relevant external IDP
sites.

60

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

• Enable Two-Factor Authentication: You can select or deselect this checkbox for a user for the SAP

Business One authentication server.
For more information about two-factor authentication, see Two-Factor Authentication for SAP
Business One Authentication Server Users [page 58].

 Note

You cannot enable two-factor authentication for B1SiteUser.

Related Information

Two-Factor Authentication for SAP Business One Authentication Server Users [page 58]

Adding Users [page 56]

3.2.4  Binding Users

After adding identity provider users into the SLD control center, you can now bind them to SAP Business One
company users.

Procedure

1. Log into the SLD control center.

2. On the Users tab, select the user you want to edit and choose Bind.

3.

In the Bind User window, you can define the following information:
• Server: Select the network address of the server
• Company: Select one or more company databases on the server.
• User Code: Select an existing user code in the companies, or define a new use code. You may input the
text to search for a specific user code. The Select All Results option enables you to select all search
results once they have been retrieved. If the user code is newly defined for all selected companies, the
label (New) shows after the user code. The default user code is the IDP user name.
An SAP Business One user can be bound to a same user code across different company databases.
Once an SAP Business One user is bound to a company user code, it cannot be bound to another user
code no matter if it is in the same company or across different companies.

 Example

You bind the SAP Business One user B1User1 to user code Julia in the company DB China. In
parallel, you can bind B1User1 to the same user code Julia in the company DB Brazil and DB US.
However, you cannot bind B1User1 to any other user code in DB China or any other companies.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

61

 Note

If you upgrade SAP Business One from a lower version to 10.0 FP 2208, you may encounter the
following situations:

• In the lower version, if you bound a Windows domain user to one SAP Business One company
user, after the updates you can find the Windows domain user and the bound company user
on the Users tab, and you can only bind the Windows domain user to the same user code in
different companies.

• In the lower version, if you bound a Windows domain user to more than one SAP Business

One company users, after the updates you can find the Windows domain user and all bound
company users on the Users tab. When you intend to bind the Windows domain user to one
more company user, you can select one bound user from the bound user dropdown list.

 Note

You cannot bind the same company user to different SAP Business One users. One company user
is only allowed to be bound to one SAP Business One user.

• Skip the binding confirmation in SAP Business One: When deselecting this checkbox, the bound

company user will be required to enter the SAP Business One user credentials in order to confirm
the binding when logging on to SAP Business One.

• Superuser: Select this checkbox to assign the Superuser role to the company user for all selected

companies.

Results

After binding SAP Business One users to company users, you can now log into SAP Business One with the SAP
Business One user accounts.

 Note

Make sure that you activate the relevant identity providers and SAP Business One users before logging in
with IDP user accounts in SAP Business One.

Related Information

Adding Users [page 56]

62

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.2.5  Deleting Users

Prerequisites

You have unbound company users from the SAP Business One user.

Procedure

1. Log into the SLD control center.

2. On the Users tab, select the user you want to delete and choose Delete.

 Caution

You cannot log into the SLD control center after deleting the last landscape admin user.

 Note

You cannot delete the default user B1SiteUser.

Related Information

Unbinding Users [page 65]

3.2.6  Copying User Mappings

You can copy user mappings between two companies, provided that the same user exists in both companies.

Context

Each user is identified by the user code (not the username).

Typical scenarios for this function are as follows:

• You have moved your company schema from a test system to a productive system.
• You have moved your company schema to another server.
• You have imported and renamed your company schema (the old schema also exists on the same server).

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

63

Procedure

1. Log into the System Landscape Directory in a Web browser.

2. On the Users tab, choose Copy User Mappings.

3.

In the Copy User Mappings Between Companies window, specify the source and target companies.

 Note

To be available for selection, the servers must be registered in the System Landscape Directory.

However, the company schema versions do not matter.

4. To display SAP Business One users whose mappings can be copied, choose Check.

If a user only exists in the source company but is bound to an IDP user, the user is displayed as missing in
the target company. However, if a user only exists in the target company, the user is not displayed.

5. To copy user mappings to the target company, choose Copy.

3.2.7  Checking AD DS User Status

Context

For Microsoft Windows domain users registered in the System Landscape Directory (SLD) control center, you
can check their status in Active Directory Domain Services (AD DS).

Procedure

1. Log into the SLD control center.

2. Choose Check AD DS User Status.

Results

The statuses of the AD DS users in the table are refreshed, accurately reflecting the current state of users
within AD DS.

64

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

3.3  Managing SAP Business One Company Users

In the SLD control center, you can manage the SAP Business One company users.

3.3.1  Unbinding Users

You can unbind identity provider users from the bound SAP Business One company users.

Procedure

1. Log into the SLD control center.

2. On the Users tab, in the Company Users in SAP Business One area, select the user you want to unbind and

choose Unbind.

 Note

As of 10.0 FP 2602, you can select multiple rows in the table to simultaneously unbind a user from
more than one company.

3.3.2  Editing Company Users

Context

You can edit the Superuser role assignment for SAP Business One company users.

Procedure

1. Log into the SLD control center.

2.

3.

In the Company Users in SAP Business One area, select the user you want to edit and choose Edit.

In the Edit window, select or deselect the Superuser checkbox.

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

PUBLIC

65

Results

The status is changed in the Superuser column.

66

PUBLIC

Identity and Authentication Management in SAP Business One
Configuring Identity and Authentication Management in the System Landscape
Directory

4  Reconfiguring Identity and

Authentication Management

This section offers several methods to help you meet the reconfiguration demands of identity and
authentication management. For example, you can restore the identity provider settings if you don’t need
to log into SAP Business One with the IDP user accounts.

4.1  Resetting Identity and Authentication Management

If you still need to log into the SAP Business One client with company users, you can restore the identity
provider settings from the SLD control center.

Procedure

1. Log into the SAP Business One SLD control center.

 Note

If you have only one active identity provider SAP Business One Authentication Server, you can skip step
1-4 and start from step 5 directly.

2. On the Identity Providers tab, select the identity provider SAP Business One Authentication Server and

choose Activate.

3.

In the Confirmation window, choose Yes.

4. Log out of the SAP Business One SLD control center.

5. Log into the SAP Business One SLD control center with the user account B1SiteUser.

6. On the Identity Providers tab, select each active identity provider and choose Deactivate.

Results

You can log into the SAP Business One client with company users.

The landscape administrator account B1SiteUser serves as a landscape-level authentication for performing
various administrator tasks, such as accessing the SLD control center and configuring services.

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

67

4.2  Renewing the Security Certificate

If you need to change or renew the security certificate for the authentication service, perform a reconfiguration
using the components wizard in SAP Business One or the server components setup wizard in SAP Business
One, version for SAP HANA . In the Specify Security Certificate window, you can change the certificate used for
authentication.

For more information about the reconfiguration, see the Administrator's Guide on the SAP Help Portal.

SAP Business One Administrator's Guide

SAP Business One Administrator's Guide, version for SAP HANA

4.3  Changing the Port Number for Authentication Service

If you need to change the port number for the authentication service, perform a reconfiguration using the
components wizard in SAP Business One or the server components setup wizard in SAP Business One,
version for SAP HANA . In the Authentication Service Ports window, you can change the port number for the
authentication service.

68

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

For more information about the reconfiguration, see the Administrator's Guide on the SAP Help Portal.

SAP Business One Administrator's Guide

SAP Business One Administrator's Guide, version for SAP HANA

4.4  Activating B1SiteUser

If you cannot log into the SLD control center or authentication service with B1SiteUser or any other external
IDP landscape administrator, you need to activate B1SiteUser from the authentication service.

This section introduces the methods and procedures about activating B1SiteUser.

4.4.1  Adding a User for Logging into the Authentication

Service

If you are working with SAP Business One, version for SAP HANA, perform the following steps:

1. Log in to the Linux server as root.

2. Navigate to the path by entering the following command:

cd <Installation Folder>/sap/SAPBusinessOne/Common/keycloak/tools/

3. Enter the following command:
./startup.sh add-admin

4. Enter the administrator account and password as requested. The default user account is b1admin.

5. Restart the SAP Business One Server Tools Authentication Service by performing the following commands:

systemctl restart sapb1servertools-authentication.service.

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

69

If you are working with SAP Business One, perform the following steps:

1. Run Windows PowerShell as the administrator.

2. Navigate to the path by entering the following command:

cd "<Installation Folder>\SAP\SAP Business One SetupFiles\keycloak\tools"

3. Enter the following command:
.\startup.ps1 add-admin

4. Enter the administrator account and password as requested. The default user account is b1admin.

5. Restart the SAP Business One Server Tools Authentication Service from the Services app.

4.4.2  Activating B1SiteUser in the Authentication Service

With the newly created user account, you can log into the authentication service and activate B1SiteUser by
choosing one of the following solutions :

• Activating B1SiteUser When It Is Locked [page 70]
• Activating SAP Business One Authentication Server When Any Other IDP Landscape Administrator Cannot

Log into the SLD [page 72]

• Resetting the Password of B1SiteUser [page 76]

4.4.2.1  Activating B1SiteUser When It Is Locked

Context

When the B1SiteUser is locked after a certain number of failed logon attempts, you can try to activate
B1SiteUser in the authentication service.

Procedure

1.

In a Web browser, access the SAP Business One authentication service by navigating to the following URL:
https://<Server Address>:<Port>/auth/. The default port number is 40020.

2. On the Welcome to Keycloak screen, choose Administration Console.

3.

In the login window, enter the username and password you defined previously in Adding a User for Logging
into the Authentication Service [page 69] .

4. After logging into the Admin Console, first check if you are working as SAP Business One. If not, choose

SAP Business One from the dropdown list in the left navigation bar.

70

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

5.

6.

In the left bar, choose Users.

In the right panel, in the user list, find and choose b1siteuser.

7.

In the b1siteuser screen, switch to Enabled in the upper right corner. and choose Save.

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

71

Results

You can now log into the SLD control center with the B1SiteUser account.

4.4.2.2  Activating SAP Business One Authentication Server

When Any Other IDP Landscape Administrator
Cannot Log into the SLD

Prerequisites

• You have deactivated the SAP Business One Authentication Server in the SLD control center.
• You have activated one or more external identity providers in the SLD control center.

Context

If you did not enable the SAP Business One authentication server, and no other external IDP landscape
administrator is able to log into the SLD and authentication service due to an unexpected issue, you can try to

72

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

activate the SAP Business One authentication server and then use the B1SiteUser account to log in to the
SLD.

Procedure

1.

In a Web browser, access the SAP Business One authentication service by navigating to the following URL:
https://<Server Address>:<Port>/auth/.

2.

In the Welcome to Keycloak screen, choose Administration Console.

3. On the login window, enter the username and password you defined previously in Adding a User for

Logging into the Authentication Service [page 69].

4. After logging into the Admin Console, first check if you are working as SAP Business One. If not, choose

SAP Business One from the dropdown list.

5.

6.

In the left bar, choose Authentication.

In the right panel, choose the Flows tab.

7. Choose the flow name B1 browser.

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

73

8.

In the B1 browser screen, find the step B1 Dynamic IDP Redirector (authen rules) and choose the Settings
icon.

9.

In the B1 Dynamic IDP Redirector config screen, switch the B1 Authentication Server login to On and choose
Save.

74

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

Results

You can now log into the SLD control center with theB1SiteUser account.

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

75

4.4.2.3  Resetting the Password of B1SiteUser

Context

If you forget your password of B1SiteUser, you can reset the password in the authentication service.

Procedure

1.

In a Web browser, access the SAP Business One authentication service by navigating to the following URL:
https://<Server Address>:<Port>/auth/. The default port number is 40020.

2. On the Welcome to Keycloak screen, choose Administration Console.

3.

In the login window, enter the username and password you defined previously in Adding a User for Logging
into the Authentication Service [page 69] .

4. After logging into the Admin Console, first check if you are working as SAP Business One. If not, choose

SAP Business One from the dropdown list in the left navigation bar.

5.

6.

In the left bar, choose Users.

In the right panel, in the user list, find b1siteuser and choose the user name.

76

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

7.

In the b1siteuser screen, go to the Credentials tab and choose Reset password.

8.

In the Reset password for b1siteuser window, enter and confirm your new password. Switch Temporary to
Off and choose Save.

 Note

You must change the password on next login if you enable Temporary.

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

77

Results

You can now log into the SLD control center with the new password of B1SiteUser.

4.4.3  Deleting the User

After activating B1SiteUser, you need to delete the user that you defined previously.

Procedure

1.

2.

3.

In the Admin Console, choose the Keycloak user from the dropdown list.

In the left bar, choose Users.

In the right panel, in the User list tab, select the user you defined previously in Adding a User for Logging
into the Authentication Service [page 69] and choose Delete user.

 Caution

We do not recommend that you make any changes in Keycloak, except the instructions we
documented in this guide. Changing other settings in Keycloak may cause the whole SAP Business
One landscape to stop working.

Results

You cannot log into the SLD control center or authentication service with the user acount you defined
previsouly, but can log in with the B1SiteUser account.

78

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

4.4.3.1  Deleting the User by Executing Queries

Prerequisites

You have backed up the B1AS schemas.

Context

If you forget the user name or password for the previously created user and are unable to log into the
authentication service admin console, you may resolve this issue by deleting the user account through
executing database queries.

 Note

If an existing administrator account is present in the authentication service, it is not possible to create a
new admin user. Consequently, it is necessary to remove the existing admin account before proceeding
with the creation of a new one.

Procedure

1. Execute the queries in the database studio.

• If you are working with SAP Business One, version for SAP HANA, run the following queires in the SAP

HANA Studio:
DELETE FROM B1AS.USER_ROLE_MAPPING WHERE USER_ID IN (SELECT ID FROM
B1AS.USER_ENTITY WHERE SERVICE_ACCOUNT_CLIENT_LINK is null and REALM_ID in
(SELECT ID FROM B1AS.REALM WHERE NAME = 'master'));
DELETE FROM B1AS.CREDENTIAL WHERE USER_ID IN (SELECT ID FROM B1AS.USER_ENTITY
WHERE SERVICE_ACCOUNT_CLIENT_LINK is null and REALM_ID in (SELECT ID FROM
B1AS.REALM WHERE NAME = 'master'));
DELETE FROM B1AS.USER_ATTRIBUTE WHERE USER_ID IN (SELECT ID FROM
B1AS.USER_ENTITY WHERE SERVICE_ACCOUNT_CLIENT_LINK is null and REALM_ID in
(SELECT ID FROM B1AS.REALM WHERE NAME = 'master'));
DELETE FROM B1AS.USER_ENTITY WHERE SERVICE_ACCOUNT_CLIENT_LINK is null and
REALM_ID in (SELECT ID FROM B1AS.REALM WHERE NAME = 'master');

• If you are working with SAP Business One, run the following queires in the Microsoft SQL Server

Management Studio:
DELETE FROM B1AS.dbo.USER_ROLE_MAPPING WHERE USER_ID IN (SELECT ID FROM
B1AS.dbo.USER_ENTITY WHERE SERVICE_ACCOUNT_CLIENT_LINK is null and REALM_ID
in (SELECT ID FROM B1AS.dbo.REALM WHERE NAME = 'master'));

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

79

DELETE FROM B1AS.dbo.CREDENTIAL WHERE USER_ID IN (SELECT ID FROM
B1AS.dbo.USER_ENTITY WHERE SERVICE_ACCOUNT_CLIENT_LINK is null and REALM_ID
in (SELECT ID FROM B1AS.dbo.REALM WHERE NAME = 'master'));
DELETE FROM B1AS.dbo.USER_ATTRIBUTE WHERE USER_ID IN (SELECT ID FROM
B1AS.dbo.USER_ENTITY WHERE SERVICE_ACCOUNT_CLIENT_LINK is null and REALM_ID
in (SELECT ID FROM B1AS.dbo.REALM WHERE NAME = 'master'));
DELETE FROM B1AS.dbo.USER_ENTITY WHERE SERVICE_ACCOUNT_CLIENT_LINK is null
and REALM_ID in (SELECT ID FROM B1AS.dbo.REALM WHERE NAME = 'master');

2. Restart the SAP Business One Server Tools Authentication Service from the Services app.

Results

The previously created user account is deleted from the authentication service.

4.5  Changing Client ID and Client Secret in the

Authentication Service

If you have changed the client ID and client secret on an external identity provider’s site for some reason, you
must synchronize the changes in the authentication service.

Prerequisites

You have changed the client ID and client secret on the external identity provider’s site.

Procedure

1.

2.

3.

In a Web browser, access the SAP Business One authentication service by navigating to the following URL:
https://<Server Address>:<Port>/auth/admin/sapb1/console.

In the left bar, choose Identity Providers.

In the right panel, select the external identity provider from the IDP list.

80

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

4.

In the right panel, choose the Settings tab.

5. Go to the OpenID Connect settings area.

6. Replace the ID and secret values in the fields Client ID and Client Secret. Make sure that you enter the same

values as on the IDP site.

7. Choose Save.

 Caution

We do not recommend that you make any changes in Keycloak, except the instructions we
documented in this guide. Changing other settings in Keycloak may cause the whole SAP Business
One landscape to stop working.

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

81

4.6  Defining a Password Blocklist for Authentication Server

Users

Context

As the landscape administrator, you can define a password blocklist for the authentication server users in the
System Landscape Directory (SLD).

Procedure

1. Create a folder named password-blacklists.

• If you are working with SAP Business One, create the folder under the path <installation

folder>\SAP Business One SetupFiles\keycloak\data

• If you are working with SAP Business One, version for SAP HANA, create the folder under the path

<installation folder>/SAPBusinessOne/Common/keycloak/data/

 Note

The authentication service may create the folder automatically. Please verify the existence of the
folder before attempting to create it.

2. Prepare a blocklist file.

• Blocklist files are UTF-8 plain-text files with Unix line endings. Every line represents a blacklisted

password.

• All passwords in the blocklist file must be lowercase.

 Example

File name: 100k_passwords.txt

Content in the file:

test_initial1

test_initial2

test_initial3

82

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

3. Upload the blocklist file to the folder which was created in the preceding step.

 Note

If the blocklist file already exists, you need to delete it first and then restart the authorization service.
Subsequently, a new blocklist file should be added with the correct file name.

4. Add the blocklist file in the authentication service.

1.

In a Web browser, access the SAP Business One authentication service by navigating to the following
URL: https://<Server Address>:<Port>/auth/admin/sapb1/console and log in with the
B1SiteUser account. The default port number is 40020.

2. On the Welcome to Keycloak screen, choose Administration Console.

3.

4.

5.

In the login window, enter the username and password of the administrator.

In the left bar, choose Authentication.

In the right panel, choose the Policies tab.

6. Choose Password Policy. In the Add policy dropdown list, select Password Blacklist.

7. Scroll down to the bottom of the page. In the newly added field Password Blacklist, enter the name of

the blocklist file (for example, 100k_passwords.txt).

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

83

Results

When you add a user for the authentication server in the SLD, or when you attempt to change the password of
an existing authentication server user, the entered password will be denied if it is in the blocklist file.

 Note

The SLD compares passwords in a case-insensitive manner.

4.7  Configure the Registry Key for Windows Domain Users

Context

As a Microsoft Windows domain user who has been bound to SAP Business One company users, you can
change the registry key value to access the SAP Business One login page and log in using a Support user
account or an IDP user account.

84

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

Procedure

1. Open the Registry Editor on your Windows machine.

2. Navigate to the path Computer\HKEY_LOCAL_MACHINE\SOFTWARE\SAP\SAP Manage\SAP Business

One

Th default value for SSO is Y.

3. Double click SSO.

4.

In the Edit String window, change the value data from Y to N and choose OK.

Results

When you launch the SAP Business One client, you need to enter the credentials of the Support user account
or an IDP user accoount on the following screen:

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

85

4.8  Configuring the Lifetime of the Access Tokens in

Keycloak

When a user logs off from the system, the token becomes invalid, however some components might cache the
token file. During its 30-minute validity, the token can be reused for logging on. This creates a time window for
attackers with stolen tokens. To reduce this risk, you can control session and token timeouts in Keycloak.

Procedure

1.

2.

3.

In the Admin Console, choose the Keycloak user from the dropdown list.

In the left bar, choose the Realm settings menu.

In the right panel, on the Tokens tab, configure the Access Token Lifespan field.

It is recommended that this value be equal to or shorter than the SSO session idle timeout: 30 minutes.
You can find the SSO Session Idle field on the Sessions tab.

 Note

Reducing the lifetime of access tokens increases the frequency of issuing new tokens. If you set the
lifetime to a small value, the heavy workload can decline the performance of SAP Business One.

86

PUBLIC

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

 Caution

We do not recommend that you make any changes in Keycloak. Changing other settings in Keycloak
may cause the whole SAP Business One landscape to stop working.

Identity and Authentication Management in SAP Business One
Reconfiguring Identity and Authentication Management

PUBLIC

87

5  Behavior Changes After Enabling Identity

and Authentication Management

This section describes the behavior changes in SAP Business One after you enable identity and authentication
management.

In this release, the following SAP Business One components support the authentication service:

• System Landscape Directory
• License Service
• Extension Manager
• Job Service
• Mobile Service

 Note

If your SAP Business One Sales or SAP Business One Service mobile app is used with SAP Business
One 10.0 FP 2208 or higher, you cannot use touch ID to log in on Android devices.

• Analytics Platform
• Service Layer
• SAP Business One, Web Client
• API Gateway Service
• Outlook Integration Server
• SAP Business One Client
• DI API
• Excel Report and Interactive Analysis
• Data Transfer Workbench (DTW)
• Microsoft 365 Integration
• SAP Business One Studio Suite
• Electronic Document Service (EDS)
• Electronic File Manager: Format Definition (EFM)
• SAP Crystal Reports, version for the SAP Business One Application
• Workflow Service
• Browser Access Service
• Browser Access Service Process Monitor
• DI Server

 Note

For the components that do not support the authentication service in this release, you can only bind
SAP Business One user accounts to Micorsoft Windows domain accounts, which means you can only
activate the one identity provider Active Directory Domain Services.

For more information about components supported by IAM in SAP Business One, see SAP Note 3252125

.

88

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

 Note

When upgrading SAP Business One or SAP Business One, version for SAP HANA with the setup wizard, you
can only enter the password for the site super user B1SiteUser in the Site User Logon window.

5.1

Logging into SAP Business One

After registering and enabling identity providers in the SLD control center, you can log in with the
authentication server user account, or the existing external user accounts, without having to create a new
account just for your SAP Business One application.

This section introduces the different login scenarios when you set up different identity providers, including:

• No identity provider is activated
• Only SAP Business One Authentication Server is activated
• Only Active Directory Domain Services is activated
• An external identity provider is activated
• Multiple identity providers are activated

 Note

After activating one or more identity providers and binding users, only the bound IDP users, rather than the
SAP Business One company user accounts, can log into SAP Business One.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

89

5.1.1  No Identity Provider Is Activated

This section introduces the new login pages if no identity provider is activated and you log into SAP Business
One as landscape administrators or SAP Business One company users.

5.1.1.1

Logging in as Landscape Administrators

For the landscape administrator login pages, you may find that the user interface has changed but you still
need to enter the super landscape user (B1SiteUser) credentials to log into the relevant Web pages.

The new landscape administrator login page applies to the following components or services:

• System Landscape Directory control center
• License control center
• Job service
• Administration console of the analytics platform
• Service Layer controller
• Workflow service
• Browser Access service process monitor

5.1.1.2

Logging in as Company Users

If no identity provider is activated, SAP Business One company user login pages for most components (such as
SAP Business One client and Web client) remain unchanged.

90

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

 Note

You can only create company users with the user account B1SiteUser if no identity provider is activated.

As of 10.0 FP 2208, the user interfaces of company user login pages for Outlook Integration and Data Transfer
Workbench (DTW) are changed. If no identity provider is activated, you need to enter the company user
credentials on the following screen:

 Note

You can see the localization and version information in the company list when logging into SAP Business
One Web-based applications, such as Web client, no matter if any identity providers have been activated.

As of version 10.0 FP 2602, when a company with a long name is selected from the drop-down list in
the Choose Company window, the full company name is displayed beneath the Select Company field. The
company name, database name, version and localization information are presented in three separate rows.
Alternatively, a new icon  Value Help appears in the Select Company field within the Choose Company
window. Choosing this icon opens a modal window that provides a comprehensive overview of all available
companies, improving the visibility for companies with long names. Within this interface, you can perform
selection, search, filtering, and sorting operations efficiently.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

91

5.1.2  Only SAP Business One Authentication Server Is

Activated

This section introduces the new login pages when you only activate the SAP Business One authentication
server, and log into SAP Business One as landscape administrators or SAP Business One users.

5.1.2.1

Logging in as Landscape Administrators

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher.
• You have set at least one authentication server user as Landscape Administrator in the SLD control center.
• You have activated SAP Business One Authentication Server in the SLD control center.

Context

You need to enter the landscape administrator’s credentials when logging into the Web-based service control
centers, including:

• System Landscape Directory control center
• License control center
• Service Layer controller
• Job service
• Administration Console of the analytics platform
• Workflow service
• Browser Access service process monitor

Procedure

1.

In a Web browser, navigate to the relevant URL for the Web-based service control center.

For example, the URL for the SLD control center https://<Server Address>:<Port>/
ControlCenter.

92

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

2.

3.

In the login window, enter the name of the landscape administrator and choose Log In.

In the next window, enter the user password and choose Log In.

4. At the first login, you are required to change the password in the Change Password window. Define and

confirm a new password and choose Submit.

Results

You open the relevant SAP Business One Web-based service control center (for example, the SLD control
center).

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

93

5.1.2.2

Logging in as SAP Business One Users

After activating the SAP Business One authentication server and binding its users to company users, you just
need to enter the credentials of bound users (SAP Business One authentication server users) when logging into
SAP Business One applications and components, including:

• SAP Business One Client
• SAP Business One, Web Client
• Outlook Integration
• Excel Report and Interactive Analysis
• Data Transfer Workbench (DTW)
• Microsoft 365 Integration
• Mobile Service

 Note

As of SAP Business One Sales mobile app version 1.0.42 and SAP Business One Service mobile app
version 1.0.13, you can use Touch ID to log in to the apps on Android devices.

• SAP Business One Studio Suite
• Electronic File Manager: Format Definition (EFM)
• SAP Crystal Reports, version for the SAP Business One Application
• Browser Access Service

In this section, we introduce the new login pages in the SAP Business One client and Web client.

5.1.2.2.1

Logging into the SAP Business One Client

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher .
• You have bound SAP Business One authentication server users to SAP Business One company users in the

SLD control center.

• You have activated SAP Business One Authentication Server in the SLD control center.

Procedure

1. Launch the SAP Business One client.

2.

If you want to log into a company, choose Log In.

94

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

 Note

If you select Skip this page and go to the login page directly, you will skip this screen and go to the login
page directly from the next login. You can also enable or disable the checkbox Skip this page and go to
the login page directly by performing the following steps:

1. On your workstation, open the file named b1-current-user.xml in the path %UserProfile%

\AppData\Local\SAP\SAP Business One\Log\BusinessOne.

2. Set the value to Y if you intend to skip the page and go to the login page directly.

<leaf kind="single" name="AlwaysLogin" type="String">
<value>Y</value>
</leaf>

Set the value to N if you don’t intend to skip the page.

<leaf kind="single" name="AlwaysLogin" type="String">
<value>N</value>
</leaf>

If you skip the page and intend to create a new company, you can go to the SAP Business One Main

Menu and choose  Administration Choose Company New .

3.

In the login window, enter the name of the bound SAP Business One user and choose Log In.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

95

4.

In the next window, enter the user password and choose Log In.

You can choose Change Password to change your login password. For detailed steps, see Changing
Password from the Login Page [page 120].

5. At the first login, you are required to change the password in the Change Password window. Define and

confirm a new password and choose Change Password and Log In.

96

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

6.

If you have bound the SAP Business One user to a user code in only one company, you can open the SAP
Business One client directly after entering the user's name and password.

If you have bound the SAP Business One user to a user code in more than one companies, you need to
choose one company in the Choose Company window.

You can see the localization and version information when choosing a company from the drop-down list.
The company that you logged into last time is selected by default.

As of version 10.0 FP 2602, when a company with a long name is selected from the drop-down list in
the Choose Company window, the full company name is displayed beneath the Select Company field. The
company name, database name, version and localization information are presented in three separate rows.
Alternatively, a new icon  Value Help appears in the Select Company field within the Choose Company
window. Choosing this icon opens a modal window that provides a comprehensive overview of all available

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

97

companies, improving the visibility for companies with long names. Within this interface, you can perform
selection, search, filtering, and sorting operations efficiently.

7.

If you want to create a new company, choose Create Company in the first window.

 Note

In the Create Company drop down list, you can also choose Create Using Wizard or Create from Package
to create a new company. For more information about how to create a new company using the express
configuration wizard or from the solution package, see the online help for SAP Business One.

a. Log in with a landscape administrator account.

b. Select a server and choose OK.

98

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

c.

In the Create New Company window, define the required values and choose OK.

d.

In the User Binding window, select Identity Provider and IDP User to bind manager to an IDP user.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

99

e. Choose Bind.

After binding the IDP user successfully, you go to the login page.

5.1.2.2.2

Logging into SAP Business One, Web Client

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher.
• You have bound SAP Business One authentication server users to SAP Business One company users in the

SLD control center.

• You have activated SAP Business One Authentication Server in the SLD control center.

Procedure

1.

In a Web browser, navigate to the URL for Web client.

2.

In the login window, enter the name of the bound SAP Business One user and choose Log In.

100

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

3.

In the next window, enter the user password and choose Log In.

4. At the first login, you are required to change the password in the Change Password window.

Define and confirm a new password and choose Submit.

5.

If you have bound the SAP Business One user to a user code in only one company, you can go to the home
page of Web client directly after entering the user’s name and password.

If you have bound the SAP Business One user to a user code in more than one company, you need to
choose one company in the Choose Company window.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

101

You can see the localization and version information when choosing a company from the drop-down list.

As of version 10.0 FP 2602, when a company with a long name is selected from the drop-down list in
the Choose Company window, the full company name is displayed beneath the Select Company field. The
company name, database name, version and localization information are presented in three separate rows.
Alternatively, a new icon  Value Help appears in the Select Company field within the Choose Company
window. Choosing this icon opens a modal window that provides a comprehensive overview of all available
companies, improving the visibility for companies with long names. Within this interface, you can perform
selection, search, filtering, and sorting operations efficiently.

5.1.3  Only Active Directory Domain Services Is Activated

This section introduces the new login pages when you only activate Active Directory Domain Services, and log
into SAP Business One as landscape administrators or SAP Business One users.

5.1.3.1

Logging in as Landscape Administrators

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher.
• You have bound Windows domain users to Landscape Administrator in the SLD control center.
• You have activated Active Directory Domain Services in the SLD control center.

102

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

Context

You need to enter the landscape administrator’s credentials when logging into the Web-based service control
centers, including:

• System Landscape Directory control center
• License control center
• Service Layer controller
• Job service
• Administration Console of the analytics platform
• Workflow service
• Browser Access service process monitor

Procedure

1.

In a Web browser, navigate to the relevant URL for the Web-based service control center.

For example, the URL for the SLD control center https://<Server Address>:<Port>/
ControlCenter

2.

In the login page, you can only choose to log in with a bound domain user account.

Enter the bound Windows domain username and password, and then choose Log In.

Results

You open the relevant SAP Business One Web-based service control center (for example, the SLD control
center).

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

103

5.1.3.2

Logging in as SAP Business One Users

After activating Active Directory Domain Services and binding its users to company users, you can choose
to use the bound domain user accounts or company user accounts when logging into SAP Business One
applications and components, including:

• SAP Business One Client
• SAP Business One, Web Client
• Outlook Integration
• Excel Report and Interactive Analysis
• Data Transfer Workbench (DTW)
• Microsoft 365 Integration
• Mobile Service

 Note

As of SAP Business One Sales mobile app version 1.0.42 and SAP Business One Service mobile app
version 1.0.13, you can use Touch ID to log in to the apps on Android devices.

• Service Layer
• SAP Business One Studio Suite
• Electronic File Manager: Format Definition (EFM)
• SAP Crystal Reports, version for the SAP Business One Application
• Browser Access Service

In this section, we introduce the new login pages in the SAP Business One client and Web client.

5.1.3.2.1

Logging into the SAP Business One Client

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher.
• You have bound Windows domain users to SAP Business One company users in the SLD control center.
• You have activated Active Directory Domain Services in the SLD control center.

Procedure

1. Launch the SAP Business One client.

2.

If you want to log into a company, choose Log In.

104

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

• If you have bound the domain user to a user code in only one company, you can open the SAP

Business One client directly after choosing Log In.

• If you have bound the domain user to a user code in more than one company, after choosing Log In,

you need to choose one company in the Choose Company window.
You can see the localization and version information when choosing a company from the drop-down
list. The company that you logged into last time is selected by default
As of version 10.0 FP 2602, when a company with a long name is selected from the drop-down list
in the Choose Company window, the full company name is displayed beneath the Select Company
field. The company name, database name, version and localization information are presented in three
separate rows. Alternatively, a new icon  Value Help appears in the Select Company field within the
Choose Company window. Choosing this icon opens a modal window that provides a comprehensive
overview of all available companies, improving the visibility for companies with long names. Within this
interface, you can perform selection, search, filtering, and sorting operations efficiently.

 Note

If you want to log in using a Support user account or an external IDP user account, you can change the
registry key value to access the login page. For more information, see Configure the Registry Key for
Windows Domain Users [page 84].

 Note

If you select Skip this page and go to the login page directly, you will skip this screen and go to the login
page directly from the next login. You can also enable or disable the checkbox Skip this page and go to
the login page directly by performing the following steps:

1. On your workstation, open the file named b1-current-user.xml in the path %UserProfile%

\AppData\Local\SAP\SAP Business One\Log\BusinessOne.

2. Set the value to Y if you intend to skip the page and go to the login page directly.

<leaf kind="single" name="AlwaysLogin" type="String">
<value>Y</value>
</leaf>

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

105

Set the value to N if you don't intend to skip the page.

<leaf kind="single" name="AlwaysLogin" type="String">
<value>N</value>
</leaf>

If you skip the page and intend to create a new company, you can go to the SAP Business One Main

Menu and choose  Administration

 Choose Company New  .

3.

If you want to create a new company, choose Create Company in the first window.

 Note

In the Create Company drop down list, you can also choose Create Using Wizard or Create from Package
to create a new company. For more information about how to create a new company using the express
configuration wizard, or from the solution package, see the online help of SAP Business One.

a. Log in with a landscape administrator account.

106

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

b. Select a server and choose OK.

c.

In the Create New Company window, define the required values and choose OK.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

107

d.

In the User Binding window, select Identity Provider and IDP User to bind manager to an IDP user.

e. Choose Bind.

After binding the IDP user successfully, you go to the login page.

108

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

5.1.3.2.2

Logging into SAP Business One, Web Client

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher.
• You have bound Windows domain users to SAP Business One company users in the SLD control center.
• You have activated Active Directory Domain Services in the SLD control center.

Procedure

1.

In a Web browser, navigate to the URL for Web client.

2.

In the login page, enter the account and password of a bound domain user and then choose Log In.

• If you have bound the domain user to a user code in only one company, you can open Web client

directly after entering the user’s name and password.

• If you have bound the domain user to a user code in more than one company, you need to choose one

company in the Choose Company window.
You can see the localization and version information when choosing a company from the drop-down
list.
As of version 10.0 FP 2602, when a company with a long name is selected from the drop-down list
in the Choose Company window, the full company name is displayed beneath the Select Company
field. The company name, database name, version and localization information are presented in three
separate rows. Alternatively, a new icon  Value Help appears in the Select Company field within the
Choose Company window. Choosing this icon opens a modal window that provides a comprehensive
overview of all available companies, improving the visibility for companies with long names. Within this
interface, you can perform selection, search, filtering, and sorting operations efficiently.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

109

5.1.4  An External Identity Provider Is Activated

This section introduces the new login pages when you activate only one external identity provider and log into
SAP Business One as landscape administrators or SAP Business One users.

 Note

In this release, you can add and activate AD FS, Microsoft Entra ID, Okta or SAP IAS as an external identity
provider.

Microsoft Entra ID is the new name for Azure Active Directory, Azure AD and AAD. For more information,
see https://learn.microsoft.com/en-us/entra/fundamentals/new-name

Related Information

Adding AD FS as an OIDC Identity Provider [page 19]

Adding Microsoft Entra ID as an OIDC Identity Provider [page 30]

Adding Okta as an OIDC Identity Provider [page 38]

Adding SAP IAS as an OIDC Identity Provider (Beta) [page 45]

5.1.4.1

Logging in as Landscape Administrators

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher.
• You have set at least one external IDP user as Landscape Administrator in the SLD control center.
• You have activated the external IDP in the SLD control center.

Context

You need to enter the landscape administrator’s credentials when logging into the Web-based service control
centers, including:

• System Landscape Directory control center
• License control center
• Service Layer controller
• Job service

110

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

• Administration Console of the analytics platform
• Workflow service
• Browser Access service process monitor

Procedure

1.

In a Web browser, navigate to the relevant URL for the Web-based service control center.

For example, the URL for the SLD control center https://<Server Address>:<Port>/
ControlCenter

2.

In the login window, enter the name of the landscape administrator (only the IDP relevant user) and choose
Log In.

As a result, you are directed to the external IDP login page.

3.

In the login page (for example, AD FS login page), enter the bound IDP user credentials and choose Sign In.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

111

Results

You open the relevant SAP Business One Web-based service control center (for example, the SLD control
center).

5.1.4.2

Logging in as SAP Business One Users

After activating an external entity provider and binding its users to company users, you need to enter the
credentials of bound IDP users when logging into SAP Business One applications and components, including:

• SAP Business One Client
• SAP Business One, Web Client
• Outlook Integration
• Excel Report and Interactive Analysis
• Data Transfer Workbench (DTW)
• Microsoft 365 Integration
• Mobile Service

 Note

As of SAP Business One Sales mobile app version 1.0.42 and SAP Business One Service mobile app
version 1.0.13, you can use Touch ID to log in to the apps on Android devices.

• SAP Business One Studio Suite
• Electronic File Manager: Format Definition (EFM)
• SAP Crystal Reports, version for the SAP Business One Application

112

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

• Browser Access Service

In this section, we introduce the new login pages in the SAP Business One client and Web client.

5.1.4.2.1

Logging into the SAP Business One Client

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher.
• You have bound the IDP relevant users to SAP Business One company users in the SLD control center.
• You have activated the external identity provider (for example, AD FS) in the SLD control center.

Procedure

1. Launch the SAP Business One client.

2.

If you want to log into a company, choose Log In.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

113

 Note

If you select Skip this page and go to the login page directly, you will skip this screen and go to the login
page directly from the next login. You can also enable or disable the checkbox Skip this page and go to
the login page directly by performing the following steps:

1. On your workstation, open the file named b1-current-user.xml in the path %UserProfile%

\AppData\Local\SAP\SAP Business One\Log\BusinessOne.

2. Set the value to Y if you intend to skip the page and go to the login page directly.

<leaf kind="single" name="AlwaysLogin" type="String">
<value>Y</value>
</leaf>

Set the value to N if you don't intend to skip the page.

<leaf kind="single" name="AlwaysLogin" type="String">
<value>N</value>
</leaf>

If you skip the page and intend to create a new company, you can go to the SAP Business One Main

Menu and choose  Administration

 Choose Company New  .

As a result, you are directed to the external IDP login page.

3.

In the login page (for example, AD FS login page), enter the bound IDP user credentials and choose Sign In.

4.

If you have bound the SAP Business One user to a user code in only one company, you can open SAP
Business One client directly after entering the user's name and password.

If you have bound the SAP Business One user to a user code in more than one company, you need to
choose one company in the Choose Company window.

114

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

You can see the localization and version information when choosing a company from the drop-down list.
The company that you logged into last time is selected by default

As of version 10.0 FP 2602, when a company with a long name is selected from the drop-down list in
the Choose Company window, the full company name is displayed beneath the Select Company field. The
company name, database name, version and localization information are presented in three separate rows.
Alternatively, a new icon  Value Help appears in the Select Company field within the Choose Company
window. Choosing this icon opens a modal window that provides a comprehensive overview of all available
companies, improving the visibility for companies with long names. Within this interface, you can perform
selection, search, filtering, and sorting operations efficiently.

5.

If you want to create a new company, choose Create Company in the first window.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

115

 Note

In the Create Company drop down list, you can also choose Create Using Wizard or Create from Package
to create a new company. For more information about how to create a new company using the express
configuration wizard, or from the solution package, see the online help for SAP Business One.

a. Log in with a landscape administrator account.

b. Select a server and choose OK.

c.

In the Create New Company window, define the required values and choose OK.

116

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

d.

In the User Binding window, select Identity Provider and IDP User to bind manager to an IDP user.

e. Choose Bind.

After binding the IDP user successfully, you go to the login page.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

117

5.1.4.2.2

Logging into SAP Business One, Web Client

Prerequisites

• You have installed SAP Business One version for 10.0 FP 2208 or higher.
• You have bound the IDP relevant users to SAP Business One company users in the SLD control center.
• You have activated the external identity provider (for example, AD FS) in the SLD control center.

Procedure

1.

In a Web browser, navigate to the URL for Web client.

2. You are directed to the external IDP login page.

In the login page (for example, AD FS login page), enter the bound IDP user credentials and choose Sign In.

• If you have bound the IDP user to a user code in only one company, you can open Web client directly

after entering the user’s name and password.

• If you have bound the IDP user to a user code in more than one company, you need to choose one

company in the Choose Company window.
You can see the localization and version information when choosing a company from the drop-down
list.
As of version 10.0 FP 2602, when a company with a long name is selected from the drop-down list
in the Choose Company window, the full company name is displayed beneath the Select Company
field. The company name, database name, version and localization information are presented in three
separate rows. Alternatively, a new icon  Value Help appears in the Select Company field within the
Choose Company window. Choosing this icon opens a modal window that provides a comprehensive

118

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

overview of all available companies, improving the visibility for companies with long names. Within this
interface, you can perform selection, search, filtering, and sorting operations efficiently.

5.1.5  Multiple Identity Providers Are Activated

If you enabled more than one identity provider in the SLD control center, you will be directed to the relevant IDP
login page according to the bound user account (email address) you entered in the following login page.

5.2  Managing Passwords

SAP Business One supports changing passwords or defining password policies for site users and company
users.

After enabling the identity provider authentication service, you may need to manage passwords on external IDP
sites.

5.2.1  Changing Passwords

After enabling the identity provider authentication services, you can log into SAP Business One with an existing
SAP Business One authentication server user account, Windows domain user account or registered external
IDP user accounts. If you intend to change the login password, you need go to the SLD control center or the
relevant external IDP sites.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

119

In the SAP Business One client, you can only change the password for technical users (for example, B1i user),
or for troubleshooting or backward compatibility purposes.

5.2.1.1

Changing Password When SAP Business One
Authentication Server Users Are Bound

If you bind a user of the SAP Business One authentication server to a company user code, you only need to
enter the name and password of the SAP Business One authentication server user when logging into the SAP
Business One client.

If you intend to change the login password, you can choose one of the following methods:

• Changing the password from the login page when you log into SAP Business One with the bound user

account.

• Changing the password from the SLD control center when you log into the SLD control center with the

landcape adminstrator's account.

 Note

The passwords set by the landscape administrators in the SLD control center are only initial
passwords. Users will be required to change the passwords at their first login.

Related Information

Changing Password from the Login Page [page 120]

Changing Password from the SLD Control Center [page 123]

5.2.1.1.1

Changing Password from the Login Page

Context

If you bind a user of the SAP Business One authentication server to a company user code, you only need
to enter the name and password of the SAP Business One authentication server user when logging into the
SAP Business One client. You can choose to change the password from the login page when you log into SAP
Business One with the bound user account.

120

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

Procedure

1. Launch the SAP Business One client.

2. Choose Log In.

3. Enter the name of the bound SAP Business One user and choose Log In.

4. Choose Change Password.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

121

5. Enter the old password and choose Next.

6. Enter and confirm the new password and choose Change Password and Log In.

122

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

5.2.1.1.2

Changing Password from the SLD Control Center

Context

If you bind a user of the SAP Business One authentication server to a company user code, you only need to
enter the name and password of the SAP Business One authentication server user when logging into the SAP
Business One client. You can change the password from the SLD control center when you log into the SLD
control center with the landcape adminstrator's account..

 Note

The passwords set by the landscape administrators in the SLD control center are only initial passwords.
Users will be required to change the passwords at their first login.

Procedure

1. Log into the SLD control center with the landcape administrator's account.

2. On the Users tab, select the user you want to change the password for and choose Edit.

3.

4.

In the Edit User window, choose Change Password.

In the Change Password window, enter and confirm your new password.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

123

5.2.1.2  Changing Password When External IDP Users Are

Bound

If you bind a Windows domain user or other external IDP user to a company user code, you only need to enter
the user’s name and the password of the domain user or external IDP user when logging into the SAP Business
One client.

If you intend to change the SAP Business One login password, you must go to the relevant IDP site to change
the password of the IDP user.

5.2.1.3  Resetting Password for the Landscape

Administrator When No Landscape Administrator
Can Log into the SLD

Context

If you forget the password of any landscape administrator (either internal or external IDP user) , you cannot log
in to the SLD control center. You need to log in to the authentication service with a newly created user account
and change the credentials for one SAP Business One authentication server user (landscape administrator).
After that, you can log in to the SLD control center with this SAP Business One authentication server user
account.

You can perform the following steps to reset the password for a landscape administrator of the SAP Business
One authentication server.

Procedure

1. Add a user for logging into the authentication service. For more details, see Adding a User for Logging into

the Authentication Service [page 69].

2.

In a Web browser, access the SAP Business One authentication service by navigating to the following URL:

https://<Server Address>:<Port>/auth/

3.

In the Wecome to Keycloak screen, choose Administration Console.

4. On the login window, enter the username and password you defined previously in Adding a User for

Logging into the Authentication Service [page 69].

5. After logging into the Admin Console, first check if you are working as Sapb1. If not, choose Sapb1 from the

dropdown list.

124

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

6.

In the left menu, choose Users.

7.

In the right panel, choose Lookup tab.

8. Choose View all users.

9.

In the user list, select the ID of the user you want to reset the password for.

10. In the new screen, choose the Credentials tab.

11. Enter your new password and confirm.

12. Choose Set Password.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

125

13. Delete the user you added in step 1. For more information, see Deleting the User [page 78].

 Caution

We do not recommend that you make any changes in Keycloak, except the instructions we
documented in this guide. Changing other settings in Keycloak may cause the whole SAP Business
One landscape to stop working.

Results

You can now log into the SLD control center with the landscape administrator that you reset the password.

5.2.2  Complying with Password Policies

After enabling the identity provider authentication services, you must comply with the password policies of the
identity providers.

• If you activated the SAP Business One authentication server, you must comply with the password policy

that is managed in the SAP Business One Authentication Service. Otherwise. you may get an internal error
message.
For more information about how to manage the password policy in the SAP Business One Authentication
Service, see Defining Password Policy in the SAP Business One Authentication Service [page 127] and
Defining Max Login Failures [page 128].

• If you activated external identity providers, you must comply with the password policies that are managed

on the respective IDP sites.

126

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

• If you activated the SAP Business One authentication server and external identity providers in parallel, you
must respectively comply with password policies defined in SAP Business One and on the external IDP
sites.

During the new installation of SAP Business One, you are required to specify a strong landscape administrator
password. You can check the password policies in the installation wizard. For more information, see the SAP
Business One Administrator’s Guide or SAP Business One Administrator’s Guide, version for SAP HANA on SAP
Help Portal.

5.2.2.1  Defining Password Policy in the SAP Business One

Authentication Service

Prerequisites

You have installed SAP Business One version for 10.0 FP 2208 or higher.

Procedure

1. To access the SAP Business One authentication service, in a Web browser, navigate to the following URL:

http://<Server Address>:<Port> /auth/admin/sapb1/console

For more information about the port number, see the administrator’s guide.

2. On the login page, enter the landscape administrator’s name (B1SiteUser) and password, and then

choose Log In.

 Note

The landscape administrator’s name is case sensitive.

 Note

If you have enabled an external identity provider authentication service, you will be directed to the
relevant IDP login page on which you need to enter the IDP user’s credentials.

3.

4.

In the Admin Console, choose Authentication in the left menu.

In the right panel, choose the Password Policy tab.

5. Define the password policy by selecting options from the Add policy dropdown list.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

127

6. Choose Save.

 Caution

We do not recommend that you make any changes in Keycloak, except the instructions we
documented in this guide. Changing other settings in Keycloak may cause the whole SAP Business
One landscape to stop working.

5.2.2.2  Defining Max Login Failures

By default, the functionality of defining the number of failed logins attempts before a successful login is not
enabled. If you intend to define the maximum number of login failures, you can enable the settings in the SAP
Business One authentication service.

Prerequisites

You have installed SAP Business One version for 10.0 FP 2208 or higher.

Procedure

1. To access the SAP Business One authentication service, in a Web browser, navigate to the following URL:

http://<Server Address>:<Port> /auth/admin/sapb1/console

For more information about the port number, see the administrator’s guide.

2. On the login page, enter the site user name (B1SiteUser) and password, and then choose Log In.

128

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

 Note

The site user name is case sensitive.

 Note

If you have enabled an external identity provider authentication service, you will be directed to the
relevant IDP login page on which you need to enter the IDP user’s credentials.

3.

In the Admin Console, choose Realm Settings in the left menu.

4.

In the right panel, choose  General

 Security Defenses

 Brute Force Detection .

5. Switch on Enabled.

6. Switch on Permanent Lockout.

 Note

Make sure you switch on both Enabled and Permanent Lockout. If Permanent Lockout is not enabled, an
unexpected error may occur.

7. Define values in the fields Max Login Failures, Quick Login Check Milli Seconds and Minimum Quick Login

Wait.

8. Choose Save.

 Caution

We do not recommend that you make any changes in Keycloak, except the instructions we
documented in this guide. Changing other settings in Keycloak may cause the whole SAP Business
One landscape to stop working.

Results

When the user exceeds the maximum number of login failures, the user account will be disabled in both the
authentication service and the SLD control center.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

129

 Note

If you enabled User Temporarily Locked in the SAP Business One authentication service, the user statuses
in the SLD may not reflect the real state (Active or Inactive).

5.3  Windows Domain Single Sign-On After Upgrades

Prior to 10.0 FP 2208, SAP Business One supports Microsoft Windows domain single sign-on (SSO)
functionality. You can bind an SAP Business One user account to a Microsoft Windows domain account.

If you upgrade SAP Business One from a lower version to 10.0 FP 2208 or higher, after the upgrade you may
find a different status based on the different scenarios:

• No identity provider is active after the upgrade

Before the upgrade, if you have not enabled the SSO functionality, or not assigned any Windows domain
user as a site user, no identity provider is active in the SLD control center after the upgrade.
The bound domain users are displayed on the Users tab, and the roles are SAP Business One User.
However, you cannot log into SAP Business One applications with the domain users because the relevant
identity provider (Active Directory Domain Services) is not active. You can log into SAP Business One
applications with the company user accounts.
If you intend to log into SAP Business One with domain users, you must go to the SLD control center with
the B1SiteUser account to set one domain user as the Landscape Administrator on the Users tab, and
then activate the identity provider Active Directory Domain Services on the Identity Providers tab.

• Only Active Directory Domain Services is active after the upgrade

Before the upgrade, if you have enabled the SSO functionality and assigned at least one Windows domain
user as a site user, the Active Directory Domain Services identity provider is active in the SLD control
center after the upgrade.
The bound domain users are displayed on the Users tab. The user role is the Landscape Administrator if a
domain user was bound to a site user. The user role is the SAP Business One User if a domain user was
bound to company users.
After the upgrade, you can only log into the SLD control center with landscape administrators and only log
into SAP Business One applications with bound domain users.

 Note

Prior to 10.0 FP 2208, if you enable Microsoft Windows domain single sign-on (SSO) functionality, you
could log on to SAP Business One applications with Windows domain user accounts and SAP Business
One company user accounts in parallel.

As of 10.0 FP 2208, the behavior is different. If you enable the SSO functionality in a lower version
and then upgrade SAP Business One to 10.0 FP 2208 or higher, you can only log on to SAP Business
One applications with bound domain users after the upgrade. If you intend to log on to SAP Business
One applications with a non-domain user account, you can bind company users to SAP Business One
Authentication Server users, and activate the SAP Business One Authentication Server in parallel to
Active Directory Domain Services from the SLD control center.

In this case, you cannot use the B1SiteUser account to perform the landscape-level operations.

130

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

5.4  Single Sign-On After Enabling Browser Windows

Integrated Authentication with AD FS

By configuring the browser to use Windows Integrated Authentication (WIA) with AD FS, users with an AD FS
account can log in to all SAP Business One components with single sign-on (SSO). For more details on the
configuration, see Enabling Browser Windows Integrated Authentication with AD FS [page 29].

After the configuration, you may encounter the following login scenarios:

• When only AD FS is active as the identity provider, you can log in to SAP Business One without entering

your user name and password.

• When multiple identity providers are active, you need to provide your user name. If the user name you

enter is bound to an AD FS account, you can log in without entering a password.

Related Information

Logging into SAP Business One [page 89]

5.5  Other Changes in the SLD Control Center

In addition to the new tabs Users and Identity Providers, you may find some other changes in the SLD control
center, such as the SLD address configuration.

5.5.1  Configuring the SLD and Authentication Server

Addresses

Context

As of 10.0 FP 2208, the internal and external addresses for the System Landscape Directory are unified. If you
intend to update the SLD address, you need to change it from the Security tab. In addition, you can also edit the
address of the authentication address.

 Note

If you upgrade SAP Business One from a lower version to 10.0 FP 2208 or higher, you must reconfigure the
SLD and authentication server address on the Security tab.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

131

If you have configured a nginx reverse proxy, you need to download the updated nginx file which contains
the authentication server.

Procedure

1. Log into the SLD control center.

2. On the Security tab, in the SAP Business One Authentication Service area, choose Edit.

3.

In the Update Address window, update the address and port number for the authentication server or SLD.

 Note

Make sure that you define a correct address for the SLD and authentication server. The whole SAP
Business One landscape will not work if the address is incorrect.

Make sure that the address is accessible to both internal and external networks. You can add a record
in the DNS to make the address accessible for the internal networks.

4. After updating the address of the authentication service, restart all component services and log into the

SLD control center again with the new network address.

5.5.2  Checking Personal Data and Change Log

You can check the logs for personal data changes regarding the identity provider authentication service.

The audit log records a time stamped list of all changes to system landscape directory resources (such as
adding identity providers and binding users), including the user that made the change and the request.

The audit log records changes made using the SLD control center. To access the audit log, in the SLD control
center, choose the Audit Logs tab.

The Audit Logs area provides an overview of all changes to SLD resources, and displays the following
information for each change:

• Sequence Number – Indicates the order in which the changes to the SLD resources occurred.
• Request – The request sent to the SLD Service API. The request is either an SLD function or an SLD entity.
• Resource – The SLD resource that was changed, and the operation that was performed.
• User Name – The name of the landscape administrator who made the change.
• Changed On – The date and time at which the SLD resource was changed.

To view detailed information about the properties that were changed for a specific resource, select the row for
the corresponding request in the audit log.

For more information about working with audit logs, see the SAP Business One Administrator’s Guide or SAP
Business One Administrator’s Guide, version for SAP HANA on SAP Help Portal.

132

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

5.6  Other Changes in the SAP Business One Client

In addition to the login page and password management, you may find other behavior changes in the SAP
Business One client after activating the identity provider authentication service.

5.6.1  Managing Technical Users

Most technical users still work after the identity provider authentication service is enabled.

• Workflow

You can use the Workflow user to log into SAP Business One for the workflow service and alert service,
and you can change the password for the Workflow user from the SAP Business One client.
The payment wizard is run in the Job Service under the Workflow user.
When using Microsoft 365 account of user Workflow to send emails directly or send approval process
notification via email, certain operations are not supported. For more information, see Limitations [page
200].
• AlertSvc

As of 10.0 FP 2208, the technical user AlertSvc is not used in SAP Business One. You can use the
technical user Workflow for the alert service.

• Support

The Support user must be bound to one IDP user if an identity provider is activated. When binding users,
you can either enter Support manually in the User Code field, or select Support from the User Code
drop-down list.
We recommend that you create a new SAP Business One authentication server user (for example,
Support) specifically for building the Support user.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

133

When you log into SAP Business One with the bound IDP user account, the following window pops up:

You can continue the login process after providing the required details.

 Note

You can activate the Support user either via the System Status Report (SSR) upload from the Remote
Support Platform (RSP), or through the SLD control center. The session timeout for the Support user
is standardized to 4 hours, irrespective of the activation method used.

• B1i

You can use the B1i user to log into SAP Business One and can change the password for B1i from the
SAP Business One client.

5.6.2  Lock Screen and Screen Locking Time

When an identity provider (either internal or external) is activated, the Lock Screen field in the File menu is not
visible.

134

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

When an identity provider (either internal or external) is activated, the Screen Locking Time (Min.) field on the

Service tab of the General Settings window ( Main Menu

 Administration

 System Initialization

 General

Settings ) is not visible.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

135

5.6.3  Permission Override

When the SAP Business One authentication server or an external identity provider is activated in the SAP
Business One client, you cannot ask a superuser to grant you authorizations in the Permission Override
window. The button Authorized by Another User is not visible.

 Note

When the Active Directory Domain Service is activated, the button Authorized by Another User is still
visible.

136

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

5.6.4  Company User Password Is Randomly Generated

After enabling identity and authentication management, you need to log into the SAP Business One client with
bound IDP user accounts. In this case, if you create a new company user in SAP Business One, the password of
the company user account is randomly generated.

If you intend to disable the IAM and log into SAP Business One with the company user credentials, you need to

specify a password in the SAP Business One client ( Administration

 Setup

 General

 Users

 General

 Password ) first, and then deactivate the IDP from the SLD control center.

5.6.5  Binding Users in SAP Business One Client

If you have activated one identity provider in the SLD control center, you can bind users in the SAP Business
One client by the following methods:

• After creating a company, you can bind the user manager to an IDP user in the User Binding pop-up

window.

• If you have the respective authorizations for the subject of Users, you can bind existing users by choosing
the Bind button that is next to the Login Account field on the General tab in the Users -Setup window

( Main Menu Administration Setup

 General Users ).

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

137

 Note

You cannot bind the current logon user, or a nonexistent user, to an IDP user. To bind a new user, you need
to define and add the user in SAP Business One first, then find the user to bind on the Users -Setup window.

5.6.6  Password Never Expires and Change Password at Next

Logon

When an identity provider (either internal or external) is activated, the fields Password Never Expires

and Change Password at Next Logon on the General tab of the Users - Setup window ( Main Menu

Administration

 Setup

 General

 Users ) are not visible.

138

PUBLIC

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

5.7  Single Logout (SLO)

Single Logout (SLO) is the counterpart to Single Sign On (SSO). As of 10.0 FP 2305, SAP Business One
supports Single Logout (SLO).

When you initiate a logout from an SAP Business One Web-based application (for example, SAP Business
One, Web client), Web-based service (for example, SAP Business One Microsoft 365 Integration) or Web-based
control center (for example, System Landscape Directory) in a Web browser, the identity provider logs you
out of all SAP Business One Web-based pages in the current identity provider login session in the same Web
browser.

Identity and Authentication Management in SAP Business One
Behavior Changes After Enabling Identity and Authentication Management

PUBLIC

139

6  Extensions

This section describes end-to-end scenarios on how to build DI API and Service Layer extensions step-by-step
so partners can easily adopt the identity provider authentication mechanism.

 Note

Adaptations are only needed when one of the IDPs is activated and partners want to adopt the new access
token login mechanism. If no IDP is activated, partners do not need to adapt their solutions. Please note
that for backward compatibility, when one or more IDPs are activated, partners can still use the previous
login mechanism.

For newly developed solutions, we recommend that partners use the new login mechanism.

6.1  Scopes

We will work with the apps that use certified third-party authentication libraries to get security tokens and
access protected resources. Low-level protocol details, which are usually only required when you manually craft
and issue raw HTTP requests to execute the OIDC flow, are not in our scope and are not recommended.

 Note

If your add-on uses DI API or Service Layer code to connect companies, and don’t have a frontend login
interface, you just need to adjust the parameter values in your code with the new login credentials in the
Connect method of DI API or the Login method of the Service Layer.

If you only enabled the identity provider SAP Business One Authentication Server, the DIAPI and Service
Layer login interfaces allow you to use the SAP Business One Authentication Server user and password to
login.

For the samples codes that are provided in this section, we will focus on the key code snippets explanation
instead of covering all code details.

The current supported app or extension types are listed as below:

• Desktop Apps

Typically for DI API add-ons running on the Microsoft Windows desktop environment.

• Web Apps

Typically for web apps that have a frontend and backend. Users can go through the OIDC flow from the
frontend and get an access token from the backend. With that token, users can access the Service Layer.

• Single Page Apps

Typically for web apps that only have a frontend. Users can go through the OIDC flow and get an access
token from the frontend with third-party libraries, such as oidc-client and jquery. After enabling Cross
Origin Resource Sharing (CORS) in the configuration of the Service Layer, users can access the Service
Layer with the token.

140

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

• Technical User Authentication (Daemon Service)

For scenarios where partner applications want to access the SAP Business One application in the
backend without user interaction, a technical user solution can be used when authenticating via the OIDC
mechanism.
To work with the technical user solution, you need to perform the following steps:

1. Register a technical user in the SAP Business One application.

2. Register a daemon service in the SAP Business One Extension Single-Sign-On Manager.

3.

Implement a daemon service which needs to integrate with the SAP Business One application.

6.2  SAP Business One Extension Single Sign-On Manager

To allow partners and customers to register extensions and to fully support the end-to-end scenario, a new
component, SAP Business One Extension Single Sign-On Manager, is added to the landscape. It is installed
along with the Extension Manager. By using the registration wizard, you will get the following essential OIDC
client information, which is the prerequisite to start the OIDC flow.

• Client ID
• Client Secret
• Redirect URI

The Client ID must start with b1-ext and follow the naming pattern: b1-ext-<guid>.

For example:

b1-ext-1c372a2e-d992-4d28-9ab1-1b81cadc4ba0

 Note

A Client ID in another format will not be accepted by the SAP Business One Authentication Server.

6.2.1  Registering a New Client

Procedure

1.

2.

In the SAP Business One Extension Single Sign-On Manager, go to Extensions and choose the Register
button.

In the Client Information step of the registration wizard, enter the name of the client and choose one of the
following client types:
• Desktop App

It is typically a public app that runs natively on a desktop machine. During the registration process, a
client ID will be generated. You have the option to specify your own redirect URI or use an automatically

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

141

created URI, which is the recommended option in most cases. For the URI, use the following naming
pattern:
b1-ext://<guid>/auth

• Daemon Service

It is an app that runs in the backend. Users can create technical users and bind them to companies or
service units. The Daemon Service will return the client ID and corresponding credentials. As there is
no front-end in this app, the redirect URI could be empty.

• Web App

It is an app that is served by code running on a server and has a frontend. Besides the client ID, the
client secret will also be generated, which can be safely saved in the app backend. For the redirect URI,
you need to provide a reachable URI of your web app so that the URI can be visited during the OIDC
authentication flow.

 Note

The client secret is only displayed one time. Please copy the value and save it securely. You will not
be able to retrieve it after you leave the registration page.

• Single Page App

It is an app that runs on a browser without a backend. Only the client ID is saved in the app frontend.
The redirect URI is used as the destination when the authentication response, namely the token,
is returned after successful authentication or logoff. The redirect URI should therefore match the
reachable URI of the single page app.

• Mobile App

It is typically an app that runs natively on a mobile device. It behaves similarly to the desktop app.

3.

In the Redirect URIs step of the registration wizard, accept the generated URI or specify your own redirect
URI.

4. Choose Review and Finish in the wizard. Copy the client ID, client secret and redirect URI, and save them in

your app.

6.3  End-to-End Scenario Overview

Context

To adopt the OIDC mechanism in your apps, it is generally required that you go through the following steps:

Procedure

1. Register the app to the SAP Business One Extension Single Sign-On Manager and save the registration

result to the app.

142

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

2. Get the authentication server endpoint by invoking the SLD APIs.

3.

Import the OIDC client library and properly configure it with the registered client information and
authentication server endpoint.

4. Program by following the OIDC protocol to get tokens.

5. Access the SLD with the access token to get the company list for the current user.

6. Select one company and get the selected company ID.

7. Connect DI API or Service Layer with the token and company ID to access the exposed business objects.

The subsequent sections will give some detailed explanations on how to accomplish the entire OIDC flow.

6.4  Walkthrough for Desktop Apps

Considering most DI API extensions are created using C#, we will use C# as the programming language to
illustrate how to create a desktop app step-by-step. During the walkthrough, a certified third party OIDC client
library, along with the web view will be adopted to initiate the OIDC flow, interact with it and accomplish it.
As the desktop app is a form of public client, the Proof Key for Code Exchange (PKCE)
additional security to the OAuth 2.0 Authorization Code flow will be used in the OIDC scenario.

, a mechanism with

You can download the complete source code package here.

6.4.1  Prerequisites

You have installed the following software components:

• SAP Business One 10.0 DI API
• Visual Studio 2017
• .Net Framework 4.7.2 or higher
• WebView2

6.4.2  Dependencies

• Microsoft.Web.WebView2

The WebView2 control enables you to embed web technologies (HTML, CSS, and JavaScript) in your native
applications powered by Microsoft Edge (Chromium).

• IdentityModel.OidcClient

RFC8252 compliant and certified OpenID Connect and OAuth 2.0 client library for native applications.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

143

6.4.3  Creating Desktop App

Procedure

1. Create a default C# desktop app.

2. Make sure the Target framework is 4.7.2.

You can change it by opening the property page once the project is created.

144

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

3. Uncheck Prefer 32-bit, because we will create an app with 64 bit DI API.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

145

4. Right click References and choose Add Reference to import SAP Business One DI API version 10.0.

146

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

5. Open your project file in an editor and then add the following third-party package references in a group.

 <ItemGroup>
    <PackageReference Include="IdentityModel.OidcClient">
      <Version>5.0.0</Version>
    </PackageReference>
    <PackageReference Include="Microsoft.Extensions.Logging.Abstractions">
      <Version>6.0.0</Version>
    </PackageReference>
    <PackageReference Include="Microsoft.Web.WebView2">
      <Version>1.0.1264.42</Version>
    </PackageReference>
  </ItemGroup>

 Note

Microsoft.Extensions.Logging.Abstractions is the dependency of
IdentityModel.OidcClient. For more details, please see here

.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

147

As an alternative, you can also manage the packages with the NuGet Package Manager, from which you
can browse and install packages as below:

6. Build and run the project.

148

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

The entire reference in the solution explorer is shown below:

6.4.4  Registering Desktop App

Procedure

1. Log on to the SAP Business One Extension Single Sign-On Manager, go to Extensions and choose the

Register button to start the registration wizard.

2.

In the Client Information step, use DesktopApp1 as the name of the client, and choose Desktop App for the
client type.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

149

3.

In the Redirect URIs step, select the Use default URI checkbox and accept the generated URI.

4. Choose Review and Finish in the wizard.

5. Copy the client ID and the redirect URI and save them in App.config.

<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <!--Above content is ignored-->
  <appSettings>
    <add key="clientID" value="b1-ext-846f5e6e-4194-47fb-b69d-71aa10cbb2c0" />
    <add key="redirectUri" value="b1-ext://846f5e6e-4194-47fb-
b69d-71aa10cbb2c0/auth" />
  </appSettings>
</configuration>

6. To read the app settings, add System.Configuration to the project References accordingly.

150

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

6.4.5  Creating Authentication WebView

Context

Browser is the indispensable client to start the OIDC flow. All the interactive operations for the authentication
need to be performed in a browser context. To create such a context, we will implement a browser interface to
provide the browser functionality and leverage the web view.

As such, we will define a class DIAppWebView in file DIAppOidcWebView.cs for this purpose with the
following details:

Procedure

1.

Inherit from the browser interface of the OIDC client and prepare a form factory to create a form as a
container for the web view, which will be used as an embedded browser to accomplish the OIDC flow.

using IdentityModel.OidcClient.Browser;
using Microsoft.Web.WebView2.WinForms;
using System;
using System.Threading;
using System.Threading.Tasks;
using System.Windows.Forms;
namespace DesktopApp1
{
    public class DIAppWebView : IBrowser
    {
        private readonly Func<Form> _formFactory;
        private BrowserOptions _options;
        public DIAppWebView(Func<Form> formFactory)
        {
            _formFactory = formFactory;
        }
        // Create a Form for authenticating.
        public DIAppWebView(string title = "Authenticating ...", int width =
1024, int height = 768)
            : this(() => new Form
            {
                Name = "DIAppAuthentication",
                Text = title,
                Width = width,
                Height = height
            })
        { }
        // ...
    }
}

2. Provide the implementation of the method InvokeAsyncx to dynamically create a form and a web view.

public class DIAppWebView : IBrowser
{
    // ...
    // Create a web view to go through the OIDC flow.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

151

    public async Task<BrowserResult> InvokeAsync(BrowserOptions options,
CancellationToken token)
    {
        _options = options;
        using (var form = _formFactory.Invoke())
        {
            using (var webView = new WebView2()
                   {
                       Dock = DockStyle.Fill
                   })
            {
                // Create a semaphore to protect this critical section so
that only one thread can access it.
                var signal = new SemaphoreSlim(0, 1);
                var browserResult = new BrowserResult
                {
                    ResultType = BrowserResultType.UserCancel
                };
                form.FormClosed += (o, e) =>
                {
                    signal.Release();
                };
                try
                {
                    // Embed the web view in the form.
                    form.Controls.Add(webView);
                    webView.Show();
                    form.Show();
                    // Initialization for the web view.
                    await webView.EnsureCoreWebView2Async(null);
                    // Delete existing cookies so previous logins won't be
remembered.
                    webView.CoreWebView2.CookieManager.DeleteAllCookies();
                    // ...
                    await signal.WaitAsync();
                }
                finally
                {
                    form.Hide();
                    webView.Hide();
                }
                return browserResult;
            }
        }
    }
}

In the meantime, to protect the flow, a semaphore is created to protect this critical section so that only one
thread can access it.

3. Take advantage of the OIDC client to get the authentication URL from the input browser options, and use it

to start the web view navigation by calling webView.CoreWebView2.Navigate.

try
{
    // ...
    // Delete existing cookies so previous logins won't be remembered.
    webView.CoreWebView2.CookieManager.DeleteAllCookies();
    // The StartUrl is generated by the OIDC library and has the below query
parameters:
    // - response_type
    // - code_challenge/code_challenge_method
    // - client_id
    // - redirect_uri
    // - state
    // This is the starting point for OIDC flow navigation.
    webView.CoreWebView2.Navigate(_options.StartUrl);

152

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

    await signal.WaitAsync();
}

With the PKCE

 mechanism, the authentication URL is as follows:

// Line breaks for legibility only
https://<authorization server>/auth/realms/sapb1/protocol/openid-connect/auth?
response_type=code
&state=T_LC0tCOJKtIFMvMq4RTSw
&code_challenge=XumS4iK1S-fMDpR8W77SVmjCxVSs7GFv4UJXTr1phsI
&code_challenge_method=S256
&client_id=b1-ext-846f5e6e-4194-47fb-b69d-71aa10cbb2c0
&scope=openid
&redirect_uri=b1-ext%3A%2F%2F846f5e6e-4194-47fb-b69d-71aa10cbb2c0%2Fauth

4. Control the OIDC navigation flow by implementing the web view method NavigationStarting and finish

the OIDC flow if navigating to the redirect URI.

// ...
form.FormClosed += (o, e) =>
{
    signal.Release();
};
webView.NavigationStarting += (s, e) =>
{
    // Finish the OIDC flow if navigating to the redirect Uri.
    if (IsNavigatingToRedirectUri(new Uri(e.Uri)))
    {
        e.Cancel = true;
        // The authorization code is included in the browser result
        browserResult = new BrowserResult()
        {
            ResultType = BrowserResultType.Success,
            Response = new Uri(e.Uri).AbsoluteUri
        };
        signal.Release();
        form.Close();
    }
};
// ...

Add a method IsNavigatingToRedirectUri to check if navigation is ending.

// The OIDC flow ends on navigating to the redirect Uri.
private bool IsNavigatingToRedirectUri(Uri uri)
{
    return uri.AbsoluteUri.StartsWith(_options?.EndUrl);
}

5. From the browser result, you can get the authorization code from the redirect URI like below, which will be

used by the OIDC client library to retrieve tokens.

// Line breaks for legibility only
b1-ext://846f5e6e-4194-47fb-b69d-71aa10cbb2c0/auth?
state=sztOJzIT88r5btSkDIPo4A
&session_state=ec8fc136-8f2d-4c65-8548-36215cb18619
&code=abd217bb-8792-4691-
a1f6-38ba02854384.ec8fc136-8f2d-4c65-8548-36215cb18619.75cc4c77-e743-4926-
b16a-f1350e9b0b2

For the complete code snippet, please see ChooseCompanyWebView.cs in the downloaded source code
package.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

153

6.4.6  OIDC Login

Context

With the authentication web view in place, we can use the OIDC client library to start the OIDC login flow.

Procedure

1. Get the SLD address.

In the productive environment, you can get the SLD address from b1-local-machine.xml. In this
sample, for the sake of simplicity, we directly hardcode it.

2. Get the SAP Business One Authentication Server discovery endpoint.

SLD provides APIs to get the endpoint. For the API references, please see GetOpenIDConnectProvider
[page 197].

In the sample, a method GetAuthorityAsync is defined in Form1.cs for this purpose.

private async Task<string> GetDiscoveryUriAsync(string sldAddress)
{
  // ...
  using (HttpClient = new HttpClient())
  {
    httpClient.DefaultRequestHeaders.Accept.Add(new
MediaTypeWithQualityHeaderValue("application/json"));
    string url = sldAddress + "/sld/sld0100.svc/GetOpenIDConnectProvider";
    HttpResponseMessage response = await httpClient.GetAsync(url);
    response.EnsureSuccessStatusCode();
    string content = await response.Content.ReadAsStringAsync();
    using (var jsonDoc = JsonDocument.Parse(content))
    {
      string discoveryUri = jsonDoc.RootElement
        .GetProperty("d")
        .GetProperty("GetOpenIDConnectProvider")
        .GetProperty("DiscoveryUri")
        .GetString();
      return discoveryUri;
    }
  }
}

OpenID Connect describes a metadata document (RFC) that contains most of the information required
for an app to carry out a sign in. This includes information such as the URLs to use and the location
of the service's public signing keys. You can find this document by appending the discovery document
path /.well-known/openid-configuration to the authority URL.

3. Configure the OIDC client options and start the OIDC login by using the OIDC client library.

In the button1_Click function of Form1.cs, let's read the configuration items.

private async void button1_Click(object sender, EventArgs e)
{

154

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

    string sldAddress = "https://<your SLD hostname>:40000";
    // Get the authority endpoint by calling the SLD API.
    // It is like https://<your oidc server>:4200/auth/realms/sapb1/.well-
known/openid-configuration
    string authority = await GetAuthorityAsync(sldAddress);
    // You can get the client id and redirectUri from your App.config
    string clientId = ConfigurationManager.AppSettings["clientId"];
    string redirectUri = ConfigurationManager.AppSettings["redirectUri"];

    // ...
}

In the button1_Click function of Form1.cs, let's create an OidcClient instance with the OIDC client
options, and invoke LoginAsync to start the OIDC login.

private async void button1_Click(object sender, EventArgs e)
{
    // ...
    var options = new OidcClientOptions
    {
        Authority = authority,
        ClientId = clientId,
        Scope = "openid",
        RedirectUri = redirectUri,
        PostLogoutRedirectUri = redirectUri,
        Browser = new DIAppWebView()
    };
    // OIDC Login
    OidcClient = new OidcClient(options);
    LoginResult = await oidcClient.LoginAsync();
    if (loginResult.IsError)
    {
        throw new Exception(loginResult.Error);
    }
    // ...
}

4. From LoginResult, we can get the following token information, which will be used in the subsequent

OIDC scenarios:
• AccessToken
• IdentityToken
• RefreshToken
• AccessTokenExpiration

5. Build and run. The following authentication pages pop up.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

155

6.4.7  Retrieving Company List

SLD provides an API to get the current user information, including the relevant company list. For the API
references, please see CurrentUserInfo [page 197].

In the sample, a method GetCompanyList is defined in ChooseCompanyWebView.cs for this purpose. The
access token is set in the request header to invoke the SLD API.

private static async Task<string> GetCompanyList(string accessToken, string
sldAddress)

156

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

 {
     // ...
     using (HttpClient = new HttpClient())
     {
         httpClient.DefaultRequestHeaders.Authorization = new
AuthenticationHeaderValue("Bearer", accessToken);
         httpClient.DefaultRequestHeaders.Accept.Add(new
MediaTypeWithQualityHeaderValue("application/json"));
         string url = sldAddress + "/sld/sld0100.svc/CurrentUserInfo?
IncludeB1UserBinding=true";
         Task<HttpResponseMessage> response = httpClient.GetAsync(url);
         if (response.Result.IsSuccessStatusCode)
         {
             return await response.Result.Content.ReadAsStringAsync();
         }
         else
         {
             throw new Exception("Get Company List Failed");
         }
     }
 }

To allow end users to select a company of interest, we need to show the company list in the UI, with two
options:

• draw the company list in a C# Form
• draw the company list in an HTML page

To have a consistent look and feel with the authentication UI, the second option is used in this sample codes.
However, the first option is more straightforward. You can select one according to your own preferences.

6.4.8  Creating Choose Company WebView

Context

Likewise, we will create a web view to render the Choose Company page and allow users to select one
company. To achieve this, the interaction between the host environment and the web view is needed. This
means that you have to program across C# in the host environment and the JavaScript running in the web view
context.

Procedure

1. Prepare the Choose Company UI in a static HTML page.

A folder named static is created to hold the static resources. Inside the folder, the
file choose_company.html is for choosing a company. Accordingly, a relevant CSS file
choose_company.css is created to define the HTML style, so that it will have a consistent view. There are
some other static resources (for example, images, fonts, and so on) that are needed in order to render the
UI page.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

157

2. Create a web view to load the HTML page and post the company list to the UI page.

The class ChooseCompanyWebView defined in ChooseCompanyWebView.cs is for this purpose. How to
create the web view to render the HTML page is basically the same as how to create the authentication
web view. The difference is that the former is a local static file, while the latter is a remote URL. For details,
please see the function public async Task<ChooseCompanyInfo> ChooseAsync(). It will return the
selected company information.

A JavaScript string is passed to the web view context by calling
CoreWebView2.AddScriptToExecuteOnDocumentCreatedAsync. In the script, the company list is
assigned to the global window object in the JavaScript context.

The key code snippet is as follows:

 // Initialization for the web view.
await webView.EnsureCoreWebView2Async(null);
// A script to assign the current company list to the window object.
string script = string.Format("window.companyList = '{0}';",
              Convert.ToBase64String(Encoding.UTF8.GetBytes(companyList)));
// Pass the script to the web view to show the company list.
await webView.CoreWebView2.AddScriptToExecuteOnDocumentCreatedAsync(script);
// Show the HTML page with company list.
webView.CoreWebView2.Navigate(_htmlFile);

3. Retrieve the company list upon loading the HTML document.

To interact with the host environment, the file choose_company.js is created and referenced in the
choose_company.html. In this file, we implement the function window.onload, in which we can get the
company list, parse it and show it.

(function () {
    "use strict";
    window.onload = function () {
          // ...
        // Get the company list from host environment, parse it and show it.
        if (window.companyList) {
            let companyList = JSON.parse(atob(window.companyList));
            show_companyList(companyList);
        } else {
            alert("Company list not assigned");
        }
    };
})();

4. Change the window location on selecting one company.

The purpose of changing the windows location is to notify the host environment that the company
selection is done. The selected company will be set in the query parameters and returned to the C#
side.

(function () {
    "use strict";
    window.onload = function () {
        const company_db_select = document.querySelector('#select-company-
db');
        const company_name_select = document.querySelector('#select-company-
name');
        const company_id_select = document.querySelector('#select-company-
id');
        // ...
        // Put the selected company in the query paramaters and
        // change the window location to notify the host the company
selection is done.

158

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

        function chooseCompany() {
            let queryOptions = [
                `CompanySchemaName=${company_name_select.value}`,
                `CompanyID=${company_id_select.value}`,
                `DatabaseInstanceName=${company_db_select.value}`
            ];
            window.location = window.location + "?" + queryOptions.join('&');
        }
        // ...
    };
})();

5. React to a window location change.

The host environment will listen to the navigation event and close the web view once the location is
changed with query options. Upon analyzing the query options, the host will know which company is
selected. The key code snippet is from the function ChooseAsync() and is as follows:

webView.NavigationStarting += (s, e) =>
{
    // Terminate the navigation if one company is selected.
    Uri = new Uri(e.Uri);
    if(IsCompanySelected(uri))
    {
        var queryResult = HttpUtility.ParseQueryString(uri.Query);
        chooseCompanyInfo = new ChooseCompanyInfo();
        chooseCompanyInfo.CompanySchemaName =
queryResult.Get("CompanySchemaName");
        chooseCompanyInfo.CompanyID = queryResult.Get("CompanyID");
        chooseCompanyInfo.DatabaseInstanceName =
queryResult.Get("DatabaseInstanceName");
        e.Cancel = true;
        signal.Release();
        form.Close();
    }
};
// The selected company will be returned in the URI query string.
private bool IsCompanySelected(Uri uri)
{
    return !string.IsNullOrEmpty(uri.Query);
}

Simply consider that the company is selected as long as the navigation URI has query options.

// The selected company will be returned in the URI query string.
private bool IsCompanySelected(Uri uri)
{
    return !string.IsNullOrEmpty(uri.Query);
}

6.4.9  Choosing Company

With the choose company web view in place, we can create an instance of the web view and ask users to select
one company. This is done in the file Form.cs.

private async void button1_Click(object sender, EventArgs e)
{
    // ...
    var chooseCompanyWebView = new ChooseCompanyWebView(loginResult.AccessToken,
sldAddress);

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

159

    ChooseCompanyInfo = await chooseCompanyWebView.ChooseAsync();
    if (chooseCompanyInfo == null)
    {
        throw new Exception("Choose company failed");
    }
    // ....
}

Users can select one company from the list and get the company ID.

6.4.10  Connecting to Company

With the AccessToken and CompanyID, we can establish a connection to the company and access the
resources.

private async void button1_Click(object sender, EventArgs e)
{
    // ...
    SAPbobsCOM.Company oCompany = new SAPbobsCOM.Company();
    oCompany.AccessToken = loginResult.AccessToken;
    oCompany.CompanyId = chooseCompanyInfo.CompanyID;
    oCompany.Server = chooseCompanyInfo.DatabaseInstanceName;
    if (oCompany.Connect() != 0)
    {
        throw new Exception("Connection failed");
    }

    // Get the current company information
    SAPbobsCOM.CompanyInfo companyInfo =
oCompany.GetCompanyService().GetCompanyInfo();
    string message = string.Format("Company Name: {0}\nCompany Version: {1}",
                  companyInfo.CompanyName, companyInfo.Version);
    MessageBox.Show(message, "DIAPI OIDC Mode");
}

160

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

6.4.11  Refreshing Token

Refresh the access token in case it has expired. This is implemented by passing the RefreshToken to the
OIDC client method RefreshTokenAsync. Upon success, the refresh token, access token and ID token will be
updated simultaneously.

RefreshTokenResult = null;
if (loginResult.AccessTokenExpiration < DateTimeOffset.Now)
{
    refreshTokenResult = await
oidcClient.RefreshTokenAsync(loginResult.RefreshToken);
    if (refreshTokenResult.IsError)
    {
        throw new Exception(refreshTokenResult.ErrorDescription);
    }
    oCompany.AccessToken = refreshTokenResult.AccessToken;
}

6.4.12  OIDC Logout

After disconnecting from the company, to perform OIDC logout we need to pass the IdentityToken to the
OIDC client method LogoutAsync.

// Disconnect from the company
oCompany.Disconnect();
// OIDC Logout
LogoutRequest logoutRequest = new LogoutRequest();
logoutRequest.IdTokenHint = refreshTokenResult != null ?
refreshTokenResult.IdentityToken : loginResult.IdentityToken;
LogoutResult logoutResult = await oidcClient.LogoutAsync(logoutRequest);
if (logoutResult.IsError)
{
    MessageBox.Show(logoutResult.ErrorDescription, "OIDC logout error");
}

6.5  Walkthrough for Web Apps

In this section, we will demonstrate how a Node.js web app can sign in users by using the authorization code
flow. The code sample also demonstrates how to get an access token to call the Service Layer APIs. You can
download the complete source code package here.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

161

6.5.1  Prerequisites

You have installed the following software components:

• SAP Business One Server Tools
• Node JS

6.5.2  Dependencies

• express

A minimal and flexible Node.js web application framework that provides a robust set of features for web
and mobile applications.

• openid-client

A server-side OpenID Relying Party (RP, Client) implementation for Node.js runtime, supports passport.

6.5.3  Creating Web App

In this sample, we must first use express to create a web application with the following basic functionalities:

• Work on a HTTPS endpoint.
• Be able to handle a JSON request.
• Enable a session between server and client, and the session has a timeout.
• Redirect to the login page upon visiting it.

Below is the key code snippet from the backend. You can check the details in server.js.

const express = require("express");
const session = require("express-session");
const bodyParser = require("body-parser");
const https = require("https");
const fs = require("fs");
const privateKey = fs.readFileSync("cert/server.key", "utf8");
const certificate = fs.readFileSync("cert/server.crt", "utf8");
const credentials = { key: privateKey, cert: certificate };
// Implement the app router
const router = express.Router();
router.get(["/*"], (req, res, next) => {
    next();
});
router.get(["/"], (req, res, next) => {
  res.redirect("/login.html");
  }
);
// Configure the web app with some middleware
const app = express();
const timeout = 60000*60 //60 minutes
app.use(session({ secret: "keyboard cat", cookie: { maxAge: timeout, sameSite:
"none", secure: true } }));
app.use(bodyParser.urlencoded({ extended: true }));
app.use(bodyParser.json());

162

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

app.use("/", router);
app.use(["/static/", "/"], express.static("static"));
// Start the web server
const httpsServer = https.createServer(credentials, app);
const port = process.env.PORT || "8000";
httpsServer.listen(port, () => {
  console.log(`Listening to requests on https://localhost:${port}`);
});

Build and run with the following command:

npm install
npm start

Now the app is listening on 8000. You can access it using the URL: https://localhost:8000.

Based on this app, we will incrementally enhance it to support the OIDC mechanism.

6.5.4  Registering Web App

Procedure

1. Log on to the SAP Business One Extension Single Sign-On Manager, go to Extensions and choose the

Register button to start the registration wizard.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

163

2.

In the Client Information step, we will use WebApp1 for the name of the client, and choose Web App for the
client type.

3.

In the Redirect URIs step, enter your website URI. Please note that wildcard URIs are allowed.

4. Choose Review and Finish in the wizard.

5. Copy the client ID, client secret and redirect URI, and save them in your app.

164

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

6.5.5  OIDC Login

Context

Unlike the desktop app, we can directly use the browser along with the OIDC client library to accomplish the
OIDC login flow. In the login page, click the Sign in button to start the OIDC login interactively. Behind the
scenes, the following operations occur:

Procedure

1. Get the SLD address.

In the productive environment, you can get the SLD address from some configuration. In this sample
codes, for the sake of simplicity, we directly hardcode it.

2. Get the SAP Business One Authentication Server discovery endpoint.

SLD provides APIs to get the endpoint. For the API references, please see GetOpenIDConnectProvider
[page 197].

In this sample codes, a method getDiscoveryUri is defined in server.js for this purpose.

async function getDiscoveryUri() {
  const config = {
    headers: { Accept: "application/json" },
    httpsAgent: new https.Agent({ rejectUnauthorized: false }),
  };
  const response = await axios.get(
      sld_url + "/sld/sld0100.svc/GetOpenIDConnectProvider",
      config
  );
  return response?.data?.d?.GetOpenIDConnectProvider?.DiscoveryUri;
}

3. Create the OIDC client with your configurations once you have the discovery URI.

const { Issuer, custom } = require("openid-client");
let b1Issuer, client;
getDiscoveryUri().then(function(discoveryUri){
  console.log(discoveryUri);
  return Issuer.discover(discoveryUri);
}).then(function (issuer) {
  b1Issuer = issuer;
  client = new b1Issuer.Client({
    client_id: client_id,
    client_secret: client_secret,
    redirect_uris: [redirect_uri],
    post_logout_redirect_uris: [logout_redirect_uri],
    response_types: ["code"],
  });
}).catch(function(e){
  console.error(e);
  process.exit(1);
});

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

165

4. Start the OIDC login by using the OIDC client library when users click the Sign in button.

router.get(["/login"], (req, res, next) => {
  res.redirect(
    client.authorizationUrl({
      scope: "openid",
      redirect_uri: redirect_uri,
      response_type: "code",
      state: home_url,
    })
  );
});

5. Redirect to the redirect URI /callback and send the authorization code to the authentication server to

get tokens.

router.get("/callback", (req, res) => {
  const params = client.callbackParams(req);
  client
    .callback(client_callback_url, params, { state: params.state })
    .then(function (tokenSet) {
      req.session.tokenSet = tokenSet;
      // ...
        // to redirect to the choose company page
    });
});

In this step, we have finished the entire OIDC authentication flow and have the following tokens for
subsequent OIDC scenarios:

• AccessToken
• IdentityToken
• RefreshToken
• AccessTokenExpiration

6. After authentication, users need to be directed to the Choose Company page to select a company. As such,

we have a redirect operation after the token is retrieved from the authentication server.

// ...
// to redirect to the choose company page
res.redirect(`/static/choose_company.html?return_to=${params.state}`);

Upon loading the choose_company.html, the return_to parameter is retained in the frontend and will
be used for further navigation.

7. Redirect to the authentication server if the current session is not authenticated or has expired.

const router = express.Router();
router.get(["/*"], (req, res, next) => {
  if (req.url) {
    if(req.url.startsWith("/") || req.url.startsWith("/static") ||
req.url.startsWith("/callback") || req.url.startsWith("/index.html")){
      next();
      return;
    }
  }
  if (!isAuthorized(req)) {
    res.redirect(
      client.authorizationUrl({
        scope: "openid",
        redirect_uri: client_callback_url,
        response_type: "code",

166

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

        state: req.url,
      })
    );
  }
  else {
    next();
  }
});

8. Build and run. After you press Sign in, the following authentication pages pop up.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

167

6.5.6  Retrieving Company List

SLD provides an API to get the current user information, including the relevant company list. For the API
references, please see CurrentUserInfo [page 197].

In the sample codes, a method getCompanyList is defined in server.js for this purpose. The access token
is set in the request header to invoke the SLD API.

 async function getCompanyList(accessToken) {
  const config = {
    headers: { Authorization: "Bearer " + accessToken },
    httpsAgent: new https.Agent({ rejectUnauthorized: false }),
  };
  let response = await axios.get(
    sld_url + "/CurrentUserInfo?IncludeB1UserBinding=true",
    config);
  return response.data;
}
router.get("/get_companies", async (req, res) => {
  try{
    let ret = await getCompanyList(req.session.tokenSet.access_token);
    let currentUserInfo = ret?.d?.CurrentUserInfo;
    req.session.currentUserInfo = currentUserInfo;
    res.status(200).send(currentUserInfo);
  }catch(e){
    res.status(500).type("application/json").send({ message: "internal server
error" });
  }
});

6.5.7  Choosing Company

Upon selecting one company, the UI is redirected to the home page or another page where the user was, or
where the authentication was initiated.

168

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

In the backend, we have a function to handle the choose company logic.

router.post("/choose_company", (req, res) => {
  req.session.companySchemaName = req.body?.companySchemaName;
  let companies = req.session.currentUserInfo.B1UserBindings.results || [];
  for (let company of companies) {
    if (company.CompanySchemaName === req.session.companySchemaName) {
      req.session.companyID = company.CompanyID;
      break;
    }
  }
  res.status(200).json({ companyID: req.session.companyID });
});

In the frontend, it will navigate to the return_to page upon success. For more details, please see
choose_company.js.

// Save the return_to state on loading the choose company page,
// and use it when users select one company.
const return_to = urlParams.get("return_to");
function chooseCompany(whichCompany) {
  // ...
  fetch("/choose_company", {
    method: "POST",
    headers: {
      "Content-Type": "application/json;charset=utf-8",
    },
    body: JSON.stringify({ companySchemaName: whichCompany }),
  })
    .then(() => {
      if (return_to) {
        window.location.href = return_to;
      }
    })
    .catch((e) => alert("Choose Company error."));
  // ...
}

6.5.8  Accessing the Service Layer

On the home page, press Get BP or Get Item or Get Order to access the Service Layer.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

169

In the backend, it will send the company ID and access token to the Service Layer to get entities.

async function getEntities(req) {
  let url = sl_url + `/${req.query.entity}?$top=1`;
  let config = {
    headers: {
      Authorization: "Bearer " + req.session.tokenSet.access_token,
      "x-b1-companyid": req.session.companyID,
    },
    httpsAgent: new https.Agent({ rejectUnauthorized: false }),
  };
  let response = {};
  try {
    response = await axios.get(url, config);
  } catch (error) {
    console.error(error.toJSON());
    response = error.response;
  }
  return response;
}
router.get("/get_entities", async (req, res) => {
  let response = await getEntities(req);
  if (response.status == 401) {
    // Handle the access token expired case.
    let ret = await refreshToken(req);
    if (ret) {
      response = await getEntities(req);
    } else {
      // Handle the refresh token expired case.
      req.session.destroy();
      return res.clearCookie("connect.sid").status(401).json({
        message: "refresh token expired, please login again.",
      });
    }
  }
  res.status(response.status).send(response.data);
});

170

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

6.5.9  Refreshing a Token

Refresh the access token in case it has expired. This is implemented by passing RefreshToken to the
OIDC client method Refresh. Upon success, the refresh token, access token and ID token are updated
simultaneously.

async function refreshToken(req) {
  let ret = true;
  try {
    const tokenSet = await client.refresh(req.session.tokenSet.refresh_token);
    console.log("refreshed and validated tokens:", tokenSet);
    req.session.tokenSet = tokenSet;
  } catch (e) {
    console.error("refresh token error:", e);
    ret = false;
  }
  return ret;
}

6.5.10  OIDC Logout

Click the button Sign out to start the OIDC logout. Upon success, it will go back to the login page.

router.post("/logout", (req, res) => {
    let idToken = req.session.tokenSet.id_token;
    req.session.destroy(() => {
      let url = client.endSessionUrl({
        id_token_hint: idToken,
      });
      res.clearCookie("connect.sid");
      console.log("logout url:", url);
      res.redirect(url);
    });
});

6.5.11  OIDC Back-Channel Logout

OIDC back-channel logout is a mechanism designed to ensure that when users log out from an identity
provider (IdP), they also log out from all associated relying parties (RPs) or applications.

How back-channel logout works:

1. User initiates logout: The user initiates an OIDC logout.

2.

IDP sends logout token: The IdP generates a logout token and sends it to all registered RPs who share the
same user’s session at the IdP through a direct back-channel request.

3. RP processes logout: Each RP receives the logout token, validates it, and terminates the user session in the

browser.

4. Confirmation to IdP: The RP may send a confirmation back to the IdP, acknowledging the successful

logout.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

171

To implement back-channel logout, proceed with the following steps:

1. Configure the back-channel logout URL in the Web App registration.

 Note

The OIDC back-channel logout URI endpoint needs to be accessible over the internet in order for
identity providers (IdPs) to access it.

2. Specify the name of the session store.

const sessionStore = new session.MemoryStore();
app.use(session({  store: sessionStore, secret: "keyboard cat", cookie:
{ maxAge: timeout, sameSite: "none", secure: true } }));

3. Retrieve the session identifier (sid) from the access token and store it in the sessionStore. Use

the jsonwebtoken library to decode the token. For library details, visit: https://github.com/auth0/node-
jsonwebtoken

.

const jwt = require('jsonwebtoken');
...
const decoded = jwt.decode(tokenSet.access_token);
req.session.sid = decoded.sid;

4. Add a new route to receive back-channel logout tokens. Validate the logout token and delete sessions with

the same sid.

router.post("/backchannel-logout", (req, res) => {
  try{
    const logoutToken = req.body.logout_token;
    let decoded = jwt.decode(logoutToken, {complete: true});
    decoded = jwt.verify(logoutToken, publicKeys.get(decoded.header.kid),
{ algorithms: ['RS256'] });
    if(!decoded.iss || decoded.iss != b1Issuer.issuer)

172

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

    {
      res.status(400).send(`Wrong issuer`);
    }
    else if (decoded.sid) {
        sessionStore.all((err, sessions) => {
          Object.entries(sessions).forEach(([sessionId, sessionData]) => {
            if (sessionData.sid === decoded.sid) {
              sessionStore.destroy(sessionId);
            }
          });
        });
      res.setHeader("Cache-Control","no-store")
      res.sendStatus(200);
    }
  }catch (error){
    res.status(400).send(`Error:  ${error.message}`);
  }
});

The publicKeys map stores signature keys in PEM format. It is generated from the JSON Web Key Set by
constructing the jwks_uri URI. Use the signature key with the same key identifier (kid) as the logout token
to verify the token.

async function getJWKs(url) {
  const config = {
    headers: { Accept: "application/json" },
    httpsAgent: new https.Agent({ rejectUnauthorized: false }),
  };
  const response = await axios.get(
    url,
    config
  );
  return response?.data?.keys;
}
getJWKs(b1Issuer.jwks_uri).then(function (JWKs) {
  for (const JWK of JWKs) {
    if(JWK.use == "sig")
      publicKeys.set(JWK.kid ,jwkToPem(JWK));
  }
});

To demonstrate how back-channel logout works, access the SAP Business One, Web client and the Web App
sample in the browser:

1. Register the Web App in the Extension SSO Manager and set the back-channel logout URL.

Configure the settings correctly and start the Web App.

2. Log in to the Web App.

3. Access the SAP Business One, Web client.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

173

4. Sign out of the SAP Business One, Web client.

5. Reload the Web App and notice that you are automatically logged out.

6.6  Walkthrough for Single Page Apps

In this section, we will demonstrate how a single page app can sign in users by using the authorization code
flow. The code sample also demonstrates how to get an access token to call the Service Layer APIs. You can
download the complete source code package here.

6.6.1  Prerequisites

You have installed the following software components:

• SAP Business One Server Tools

174

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

• Node JS

6.6.2  Dependencies

• express

A minimal and flexible Node.js web application framework that provides a robust set of features for web
and mobile applications.

• oidc-client-ts

A library that provides OIDC and OAuth2 protocol support for browser-based JavaScript applications.

6.6.3  Creating Single Page App

In this sample, we must first use express to create a server with the following basic functionalities:

• Work on an HTTPS endpoint.
• Redirect to the login page upon visiting it.

Below is the key code snippet. You can check the details in server.js.

const express = require("express");
const https = require('https');
const fs = require('fs');
const path = require('path');
const options = {
    key: fs.readFileSync('cert/server.key'),
    cert: fs.readFileSync('cert/server.crt')
  };
const app = express();
//setup static folder
app.use(express.static('static'));
app.get("*", (request, response) => {
    response.sendFile(path.join(__dirname, '/static/index.html'));
});
const httpsServer = https.createServer(options, app);
httpsServer.listen("3300", () => {
  console.log(`Listening to requests on https://localhost:3300`);
});

Build and run with the following command:

npm install
npm start

Now the app is listening on 3300. You can access it using the URL: https://localhost:3300.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

175

6.6.4  Registering Single Page App

Procedure

1. Log on to the SAP Business One Extension Single Sign-On Manager, go to Extensions and choose the

Register button to start the registration wizard.

2.

In the Client Information step, we will use SinglePageApp1 for the name of the client, and choose Single
Page App for the client type.

3.

In the Redirect URIs step, enter your website URI. For example, https://localhost:3300/*. Please
note that wildcard URIs are allowed.

4. Choose Review in the wizard and then submit.

5. Copy the client ID, and save it in your app.

6.6.5  OIDC Login

Context

Similar to the web app, we can directly use the browser, together with the OIDC client library, to accomplish the
OIDC login flow. The default page is the OIDC authentication login page.

176

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

Procedure

1. Get the SLD address.

In the productive environment, you can get the SLD address from some configuration. In this sample code,
for the sake of simplicity, we directly hardcoded it.

let sldAddress = 'https://sld_address:40000/sld/sld0100.svc';

2. Get the SAP Business One Authentication Server discovery endpoint.

SLD provides APIs to get the endpoint. For the API references, please see GetOpenIDConnectProvider
[page 197].

In this sample code, a method getAuthorityEndpoint is defined in client-manager.js for this
purpose.

 getAuthorityEndpoint = () => {
     let settings = {
         type: 'GET',
         dataType: 'json',
         timeout: 15000,
         url: this.openIdConnectProviderUrl
     }
     return new Promise((resolve, reject) => {
         $.ajax(settings)
             .done(function (data) {
                 let authEndpoint =
data.d.GetOpenIDConnectProvider.DiscoveryUri
                 if (authEndpoint) {
                     resolve(authEndpoint);
                 } else {
                     reject(new Error('The DiscoveryUri does not set!'));
                 }
             })
             .fail(function (jqXHR, errorStatus) {
                 if (errorStatus == "timeout") {
                     reject(new Error("Sorry, request time out!"));
                 } else {
                     reject(jqXHR);
                 }
             });
     })
 }

3. Create a new class named OidcClientManager which is a wrapper of the oidc-client.

class OidcClientManager{
  constructor(clientSettings, openIdConnectProviderEndpoint = '',
userInfoEndpoint = '')
  {
   ...
  }

}

In the constructor function, only the first parameter is mandatory.

In the OidcClientManager.init function, we create the Oidc.UserManager object to redirect to the
OIDC login page once you have the discovery URI.

init = () => {
     return new Promise((resolve, reject) => {

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

177

         return this.getAuthorityEndpoint().then(data => {
             this.clientSettings.authority = data;
             this.clientSettings.metadataUrl = data;
             this.userManager = new oidc.UserManager(this.clientSettings);
             this.userManager.signinRedirectCallback().then(user => {
                 window.history.replaceState(null, window.document.title, '
');
                 resolve(user);
             }).catch(err => {
                 if (err.message === "No state in response" || err.message
=== "No matching state found in storage")
                     this.startSigninMainWindow().then(() => {
                         resolve();
                     }).catch(err => {
                         reject(err);
                     })
                 else
                     reject(this.formatOidcErr(err));
             })
         }).catch(err => { reject(err) })
     })
 }

4. After the successful authorization, the tokens are stored in the UserManager. You get tokens as below.

getUser = () => {
     return new Promise((resolve, reject) => {
         this.getUserManager().then(userManager => {
             userManager.getUser().then(data => {
                 resolve(data);
             }).catch(err => {
                 reject(err);
             });
         }).catch(err => {
             reject(err);
         });
     })
 }
 getAccessToken = async () => {
     try {
         let user = await this.getUser();
         if (this.validateToken(user['access_token'], 30)) {
             return Promise.resolve(user['access_token']);
         } else if (this.validateToken(user['refresh_token'], 10)) {
             user = await this.refreshToken();
             return Promise.resolve(user['access_token']);
         } else {
             return Promise.reject(new Error("login_required"));
         }
     } catch (error) {
         if (error.message === "refresh_token_error")
             return Promise.reject(new Error("login_required"));
         else
             return Promise.reject(error);
     }
 }

In this step, we have finished the entire OIDC authentication flow and have the following tokens for
subsequent OIDC scenarios:

• AccessToken
• RefreshToken

5. After authentication, we get the binding companies and set these data to bind-company list.

ClientManager.getBindingCompaniesInfo()

178

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

.then(bindCompanyListUI)
.catch(err=>{
  alert("get binding user info failed: " + err);
});

6. Build and run. The following authentication pages pop up.

6.6.6  Retrieving Company List

SLD provides an API to get the current user information, including the relevant company list. For the API
references, please see CurrentUserInfo [page 197].

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

179

In the sample codes, a method getBindingCompaniesInfo is defined in client-manager.js for this
purpose. The access token is set in the request header, as seen from the function ajaxHelper, to invoke the
SLD API. The ajaxHelper is a wrapper of $.ajax(), which already includes the authorization header and
refreshes the token mechanism. The ajax setting has a default value with a default method of GET and a data
type of JSON. You can configure your own settings passed in.

getBindingCompaniesInfo = () => {
        return new Promise((resolve, reject) => {
            this.ajaxHelper(this.userInfoUrl+'?
IncludeB1UserBinding=true').then(data => {
                resolve(data);
            }).catch(err => {
                reject(err);
            });
        })
    }
ajaxHelper = async (url, settings) => {
            ......
            let accessToken = await this.getAccessToken();
            let targetSettings = Object.assign({}, DEFAULT_SETTINGS, settings);
            ......
    }

6.6.7  Choosing Company

Upon selecting one company, the UI is redirected to the home page, or another page where the user was, or
where the authentication was initiated.

You can use the following sample code to choose a company:

companyID = sessionStorage.getItem("companyID");
if(companyID){
  chooseCompanyForm(companyID);

180

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

}}

6.6.8  Accessing the Service Layer

On the home page, press Get BP, Get Item or Get Order to access the Service Layer.

 Note

• You need to enable CORS during the configuration of Service Layer. For more information, see Working

with SAP Business One Service Layer on the SAP Help Portal.

• As of SAP Business One 10.0 FP 2602, audience validation is enabled by default in Service Layer for
Single Page Apps as a security enhancement. If you use an access token to access Service Layer,
ensure that the audience claim in the access token includes the Service Layer client ID as one of the
audience values. Otherwise, you encounter a 401 no authorization error.
To resolve this issue, you can add the Service Layer client ID in the Keycloak client configuration. For
more information, see Configuring Audience in Keycloak [page 182].
However, if you want to disable audience validation for testing or other development purposes, you
can set the EnableAudienceValidation to false in the Service Layer configuration file b1s.conf.
After you modify the file, restart the Service Layer service. Audience validation is then no longer
performed.

In the frontend, it will send the company ID and access token to the Service Layer to get the entities.

function getEntities(name){
  var settings = {
    headers: {
      "x-b1-companyid":sessionStorage.getItem("companyID"),
    }
  };
  ClientManager.ajaxHelper(slBaseUrl+name+'?$top=1', settings)

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

181

  .then(data=>{
    alert(JSON.stringify(data))
  })
  .catch(data=>{
    alert(JSON.stringify(data))
  });
}

6.6.9  Refreshing a Token

Refresh the access token in case it has expired. This is implemented by passing RefreshToken to the OIDC
client method refreshToken. Upon success, the refresh token, access token, and ID token are updated
simultaneously.

refreshToken = () => {
        return new Promise((resolve, reject) => {
            this.getUser().then(user => {
                if (!user) {
                    return reject(new Error("login_required"));
                }
                this.userManager._useRefreshToken({ refresh_token:
user.refresh_token }).then((resp) => {
                    if (resp) {
                        resolve(resp);
                    } else {
                        reject(new Error("refresh_token_error"));
                    }
                }).catch(err => {
                    if (err.message === "invalid_grant")
                        reject(new Error("refresh_token_error"));
                    else
                        reject(err);
                })
            }).catch(err => {
                reject(err);
            })
        });
    }

6.6.10  OIDC Logout

Click the Sign out button to start the OIDC logout. Upon success, the login page is displayed.

ClientManager.startSignoutRedirect();

6.6.11  Configuring Audience in Keycloak

Perform the following steps to configure the audience in Keycloak for a Single Page App that has already been
registered to Keycloak through the SAP Business One Extension Single Sign-On Manager.

182

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

 Note

This is a workaround for audience configuration for versions before SAP Business One 10.0 FP 2608.

1. Log in to the Keycloak admin console with the admin account.

2. Navigate to the Clients section and select the client representing your application. For example, the client

ID starts with b1-ext-singlepage-3bf8c5ac.

3. Go to the Client Scopes tab and click the scope relevant to your client ID in the Assigned client scope. For

example, the client scope starts with b1-ext-singlepage-3bf8c5ac.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

183

4. Configure a new mapper for the audience.

184

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

5.

In Add mapper, give the mapper a name (for example, my_audience_mapper) and select the Service
Layer client ID (for example, b1-B1ServiceLayers-1222-main) from the Included Client Audience list.

6. Save the changes.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

185

6.7  Walkthrough for Daemon Service

We use C# as the programming language to illustrate how to authenticate a partner daemon service step-by-
step. In the sample code, we first retrieve the access token from the SAP Business One Authentication Service
with the client ID and client credentials in the configuration step. We then request the binding companies from
SLD userinfo endpoint. Lastly, we access the Service Layer API using the access token and the company ID
with the identity of the technical user.

 Note

We currently don't support accessing the DI API using the access token and the company ID with the
identity of the Daemon Service technical user.

You can download the complete source code package here.

6.7.1  Prerequisites

You have installed the following software components:

• Visual Studio 2022 or higher
• .Net 6.0 or higher

6.7.2  Dependencies

• Microsoft.IdentityModel.Tokens

The library provides support for SecurityTokens and Cryptographic operations (Signing, Verifying
Signatures, and Encryption).

• Microsoft.IdentityModel.JsonWebTokens

The library provides support for creating, serializing and validating JSON Web Tokens.

• Newtonsoft.Json

Json.NET is a popular high-performance JSON framework for .NET.

186

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

6.7.3  Creating a Daemon Service

Procedure

1. Create an ASP.NET Core Empty app.

2. Select .NET 6.0.

You can change it by opening the property page once the project is created.

3. Open your project file in an editor and then add the following third-party package references in a group.

<ItemGroup>
   <PackageReference Include="Microsoft.IdentityModel.JsonWebTokens"
Version="7.6.3" />
   <PackageReference Include="Microsoft.IdentityModel.Tokens"
Version="7.6.3" />
   <PackageReference Include="Newtonsoft.Json" Version="13.0.3" />
</ItemGroup>

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

187

As an alternative, you can also manage the packages with the NuGet Package Manager, from which you can
browse and install packages like below:

6.7.4  Registering the Daemon Service

Procedure

1. Log on to the SAP Business One Extension Single Sign-On Manager, go to Extensions and choose the

Register button to start the registration wizard.

2.

In the Client Information step, specify the name of the client, and choose Daemon Service for the client
type.

188

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

 Note

• You can create a technical user in the SAP Business One client from  Administration Setup

General Users . The username should begin with b1ext_.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

189

• You can enable the OAuth client as a technical user in multiple service units and companies in the
dropdown box. If you select "Enabled All Companies under <IP Address>", that means the existing
and future companies are both enabled automatically under the IP address.

• We highly recommend utilizing Signed JWT authentication, which is more secure than client secret
authentication. In the sample code, we focus on demonstrating how Signed JWT authentication
works, and the client secret authentication is briefly introduced.

3. Since this app is not related to the front-end, in the Redirect URIs step, you can edit the HTTP redirect URI,

for example, https://localhost, or leave it empty.

190

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

4. Choose Review in the wizard.

 Note

If you encounter a warning as shown below, please confirm that the technical user exists.

Only submit when there are no warnings.

5. Copy the client ID and credentials, and save them as ClientId and PrivateKey in config.json.

{
"PrivateKey": "<the credentials>",

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

191

"ClientId": "b1-ext-xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
}

6.7.5  Getting an Access Token

Procedure

1. Set SLDAddress in the config.json file.

{
"SLDAddress": "https://XXXX:40000"
}

You can modify the values according to your SLD environment.

Don't forget to copy the config.json file to the folder where the binary exe file is located. Our sample
codes reads JSON from the directory where the exe file is located by default.

string configurationText = System.IO.File.ReadAllText("config.json");
configuration =
JsonConvert.DeserializeObject<Configuration>(configurationText);

2. Get the token endpoint URL.

According to your provided SLDAddress, in the GetTokenEndpointURL function, we must first obtain the
DiscoveryUri by accessing GetOpenIDConnectProvider, and then obtaining the token_endpoint.

 client.BaseAddress = new Uri(configuration.SLDAddress + "/sld/sld0100.svc/
GetOpenIDConnectProvider?$format=json");
 client.DefaultRequestHeaders.Clear();
 HttpResponseMessage response = client.GetAsync("").Result;
 if (response.IsSuccessStatusCode)
 {
     string responseBody = response.Content.ReadAsStringAsync().Result;
     if(responseBody != null)
     {
         JObject? obj = (JObject)JsonConvert.DeserializeObject(responseBody);
         string discoveryUri = obj["d"]["GetOpenIDConnectProvider"]
["DiscoveryUri"].ToString();
         HttpClient clientBak = new();
         clientBak.BaseAddress = new Uri(discoveryUri);
         clientBak.DefaultRequestHeaders.Clear();
         HttpResponseMessage responseBak = clientBak.GetAsync("").Result;
         responseBody = responseBak.Content.ReadAsStringAsync().Result;
         if (responseBak.IsSuccessStatusCode)
         {
             OpenIDConfiguration? openidConfig =
JsonConvert.DeserializeObject<OpenIDConfiguration>(responseBody);
             if (openidConfig is not null)
             {
                 return openidConfig.TokenEndpoint;
             }
         }
     }
 }

192

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

3. Get RSA private key.

In the GetRSASecurityKey function, we use RSA.ImportPkcs8PrivateKey to import the private key
from the PrivateKey field in the config.json file.

private static RsaSecurityKey GetRSASecurityKey()
 {
     //Get RSA privateKey
     var privateKeyBytes = Convert.FromBase64String(configuration.PrivateKey);
     var rsa = RSA.Create();
     rsa.ImportPkcs8PrivateKey(privateKeyBytes, out _);
     return new RsaSecurityKey(rsa);
 }

4. Generate the JWT as the client_assertion.

In the GetAccessToken function, we must first create the JsonWebToken by the
Microsoft.IdentityModel.JsonWebTokens library.

 // Get jwt
 var handler = new JsonWebTokenHandler();
 var descriptor = new SecurityTokenDescriptor
 {
     Subject = new ClaimsIdentity(new[]
     {
         new Claim(JwtRegisteredClaimNames.Sub, configuration.ClientId),
         new Claim(JwtRegisteredClaimNames.Jti, Guid.NewGuid().ToString())
     }),
     Issuer = configuration.ClientId,
     Audience = configuration.TokenEndpointURL,
     NotBefore = DateTime.UtcNow.AddMinutes(-120),
     Expires = DateTime.UtcNow.AddMinutes(120),
     SigningCredentials = new SigningCredentials(securityKey,
SecurityAlgorithms.RsaSha256)
 };
 string clientAssertion =  handler.CreateToken(descriptor);

For detailed usage of this library, please refer to Microsoft official document

.

5. Get an access token by clientid and clientassertion.

With client_assertion, the request should be as follows:

HttpClient client = new();
client.BaseAddress = new Uri(configuration.TokenEndpointURL);
client.DefaultRequestHeaders.Clear();
client.DefaultRequestHeaders.Accept.Add(MediaTypeWithQualityHeaderValue.Parse(
"application/json"));
string stringContent =
$"grant_type=client_credentials&scope=openid&client_id={configuration.ClientId
}"
         + $"&client_assertion_type="+
System.Web.HttpUtility.UrlEncode("urn:ietf:params:oauth:client-assertion-
type:jwt-bearer") +$"&client_assertion={clientAssertion}";

If the request is successful, the following values will be returned, which are defined in Tokens.cs.

• access_token
• expires_in
• refresh_expires_in
• token_type
• id_token

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

193

• not-before-policy
• scope

 Note

If you select Client Secret as the Credential Type when you register the oAuth client, you will directly
receive the Client ID and Client Secret from the Extension SSO Manager.

In this case, you don't need to generate the Json Web Token as shown above. The stringContent
should be as follows.

string stringContent =
$"grant_type=client_credentials&scope=openid&client_id={ClientId}&client_se
cret={ClientSecret}";

It may seem simpler, however if the application processes sensitive data, we highly recommend that
you utilize the Signed JWT authentication.

6.7.6  Getting a Company ID

The System Landscape Directory (SLD) provides an API to get the current user information, including the
relevant company list. For the API reference, please see CurrentUserInfo [page 197].

In the sample code, we default to using the first company ID in the list. A method GetFirstCompanyId is
defined for this purpose. You can also choose another company ID based on your specific situation. The access
token is set in the request header to invoke the SLD API.

private static string GetFirstCompanyId()
{
  //...
  HttpClient client = new();
  client.BaseAddress = new Uri(configuration.CurrentUserInfoURL+
"&$format=json");
  client.DefaultRequestHeaders.Clear();
  client.DefaultRequestHeaders.Add("Authorization", $"Bearer {accesstoken}");
  HttpResponseMessage response = client.GetAsync("").Result;
  //...
}

194

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

When the token expires, it will call GetAccessToken again to obtain a new token.

if (response.StatusCode == HttpStatusCode.Unauthorized)
{
   //if accesstoken expired, try twice
   accesstoken = GetAccessToken();
   client.DefaultRequestHeaders.Remove("Authorization");
   client.DefaultRequestHeaders.Add("Authorization", $"Bearer {accesstoken}");
   response = client.GetAsync("").Result;
}
if(!response.IsSuccessStatusCode)
{
   throw new InvalidDataException("Get company id failed");
}

6.7.7  Accessing the Service Layer

We can use the obtained access token and company id to access the Service Layer. In config.json, we define
the Service Layer URL.

{
"ServiceLayerBaseURL": "https://XXXX:50000"
}

In method GetCurrentUserInfoBySL, we demonstrate obtaining user information by accessing the Service
Layer API UsersService_GetCurrentUser. The access token and company ID are set in the request
headers to invoke the Service Layer API.

client.BaseAddress = new Uri(configuration.ServiceLayerBaseURL + "/b1s/v2/
UsersService_GetCurrentUser");
client.DefaultRequestHeaders.Clear();
client.DefaultRequestHeaders.Add("Authorization", $"Bearer {accesstoken}");
client.DefaultRequestHeaders.Add("X-b1-companyid", companyid);
StringContent content = new("", Encoding.UTF8, "application/json");
HttpResponseMessage response = client.PostAsync("", content).Result;

You can also access other APIs, such as getting items. A method GetItemsBySL is defined for this purpose.

 Note

You should first grant permissions to the corresponding SAP Business One technical user in the SAP

Business One client. In our sample code, grant Inventory permission to b1ext_dsuser in  Administration

 System Initialization

 Authorizations  form.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

195

HttpClient client = new();
client.BaseAddress = new Uri(configuration.ServiceLayerBaseURL+ "/b1s/v2/Items?
$top=3");
client.DefaultRequestHeaders.Clear();
client.DefaultRequestHeaders.Add("Authorization", $"Bearer {accesstoken}");
client.DefaultRequestHeaders.Add("X-b1-companyid", companyid);
HttpResponseMessage response = client.GetAsync("").Result;

When the token expires, it will call GetAccessToken again to obtain a new token.

if (response.StatusCode == HttpStatusCode.Unauthorized)
{
   //if accesstoken expired, try twice
   accesstoken = GetAccessToken();
   client.DefaultRequestHeaders.Remove("Authorization");
   client.DefaultRequestHeaders.Add("Authorization", $"Bearer {accesstoken}");
   response = client.GetAsync("").Result;
}
if (!response.IsSuccessStatusCode)
{
   throw new InvalidDataException("Get items failed");
}

6.8  SLD API References

SAP Business One provides you with the SLD APIs used in the OIDC scenario.

196

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

6.8.1  GetOpenIDConnectProvider

Description

This API retrieves the discovery URL of the OpenID Connect Provider (powered by SAP Business One
authentication server). The application is expected to retrieve the metadata of the OpenID Connect provider,
including data such as the token endpoint, user endpoint, logout endpoint, and so on.

Usage

GET /sld/sld0100.svc/GetOpenIDConnectProvider
Accept: application/json

Upon success, it returns 200, with a JSON formatted body.

If it fails, it returns 4xx.

6.8.2  CurrentUserInfo

Description

This API retrieves the information of a given user who is presented by an access token.

Usage

GET /sld/sld0100.svc/CurrentUserInfo?IncludeB1UserBinding=true
Accept: application/json
Authorization: Bearer <your access token>

Upon success, it returns 200, with a JSON formatted body, including the user roles and the company
assignment of the user with detailed information.

If it fails, it returns 4xx. For example, a 401 indicating an error when processing a bearer token or user that was
not authenticated, or a session timeout.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

197

6.9  Connection References for Service Layer and DI API

The following table shows different connection methods via Service Layer (SL) or Data Interface (DI) API of
SAP Business One in the span of several feature packages.

Scenarios

Versions Prior to FP 2208

FP 2208

FP 2305 and Onwards

No IDP is activated (tradi-

Always connect via the SAP

tional SAP Business One

Business One user code and

• Register an extension
client ID in the SAP

• Register an extension
client ID in the SAP

user)

password

Business One Extension

Business One Extension

Single Sign-On Manager

Single Sign-On Manager

and connect with the ac-

and connect with the ac-

cess token

cess token

• Connect via the SAP

• Connect via the SAP

Business One user code

Business One user code

and password

and password

The Active Directory Domain

Always connect via the SAP

Services is activated

Business One user code and

• Register an extension
client ID in the SAP

• Register an extension
client ID in the SAP

password

The SAP Business One au-

Not applicable

thentication server is acti-

vated

Business One Extension

Business One Extension

Single Sign-On Manager

Single Sign-On Manager

and connect with the ac-

and connect with the ac-

cess token
• Enable the SAP

Business One authen-

cess token

• Connect via the Active
Directory Domain Serv-

tication server and

ices domain user code

connect via the SAP

and password

Business One authenti-

cation server user code

and password

• Register an extension
client ID in the SAP

• Register an extension
client ID in the SAP

Business One Extension

Business One Extension

Single Sign-On Manager

Single Sign-On Manager

and connect with the ac-

and connect with the ac-

cess token

cess token

• Connect via the SAP

• Connect via the SAP

Business One authenti-

Business One authenti-

cation server user code

cation server user code

and password

and password

198

PUBLIC

Identity and Authentication Management in SAP Business One
Extensions

Scenarios

Versions Prior to FP 2208

FP 2208

FP 2305 and Onwards

One or more external IDPs

Not applicable

are activated

• Register an extension
client ID in the SAP

• Register an extension
client ID in the SAP

Business One Extension

Business One Extension

Single Sign-On Manager

Single Sign-On Manager

and connect with the ac-

and connect with the ac-

cess token
• Enable the SAP

cess token

Business One authen-

tication server and

connect via the SAP

Business One authenti-

cation server user code

and password

6.10  Principal Propagation for SAP Business One

SAP Business One principal propagation is an authentication mechanism provided for the partner side-by-side
applications passing end user context into SAP Business One provided APIs. SAP Business One APIs will
authenticate the user context coming from the partner application and propagate the user identity information
into the SAP Business One application. With this capability, partner applications can seamlessly access SAP
Business One resources with end user identity and permission.

For more information, please refer to Principal Propagation for SAP Business One.

Identity and Authentication Management in SAP Business One
Extensions

PUBLIC

199

7

Limitations

The following list describes the limitations of IAM in SAP Business One for the current release.

• The remote support platform (RSP) for SAP Business One only supports the user account B1SiteUser and

does not support any other landscape administrator.

• The command mode of Data Transfer Workbench (DTW.exe -s -s XXX.xml) is supported except for specific

user types.
The following user types cannot work with generated XML files:
• Authentication service users that are enabled for two-factor authentication
• External IDP users
As a workaround, you can use the authentication service user type without two-factor authentication.
Alternatively, you can use a SAP Business One user if IAM is not enabled.
To work with the command mode of DTW, in step 7 of the Data Import Wizard, choose Save to save the
wizard settings to an XML file. Use the XML file in the command mode of DTW as a scheduled run.
In DTW version FP 2208, FP 2305, and SP 2308, you cannot save the wizard settings to an XML file. In DTW
version SP 2311, the limitation is fixed and you can save the wizard settings.

• If you activate an identity provider and log into SAP Business One with a bound user, the functionality of

setting a schedule for running a report in the Report Execution Scheduler window does not work , no matter
whether you enter the correct user credentials or not.

• When an identity provider is activated and the SAP Business One Microsoft 365 integration feature is being

used under the Workflow user account, the following operations are not supported:
• Sending emails directly for marketing documents
• Sending approval process notification via email
For more information about SAP Business One Microsoft 365 integration, see How to Work with SAP
Business One Microsoft 365 Integration.

200

PUBLIC

Identity and Authentication Management in SAP Business One
Limitations

Important Disclaimers and Legal Information

Hyperlinks

Some links are classified by an icon and/or a mouseover text. These links provide additional information.

About the icons:
• Links with the icon

: You are entering a Web site that is not hosted by SAP. By using such links, you agree (unless expressly stated otherwise in your

agreements with SAP) to this:
• The content of the linked-to site is not SAP documentation. You may not infer any product claims against SAP based on this information.
• SAP does not agree or disagree with the content on the linked-to site, nor does SAP warrant the availability and correctness. SAP shall not be liable for any

damages caused by the use of such content unless damages have been caused by SAP's gross negligence or willful misconduct.

• Links with the icon

: You are leaving the documentation for that particular SAP product or service and are entering an SAP-hosted Web site. By using

such links, you agree that (unless expressly stated otherwise in your agreements with SAP) you may not infer any product claims against SAP based on this

information.

Videos Hosted on External Platforms

Some videos may point to third-party video hosting platforms. SAP cannot guarantee the future availability of videos stored on these platforms. Furthermore, any
advertisements or other content hosted on these platforms (for example, suggested videos or by navigating to other videos hosted on the same site), are not within
the control or responsibility of SAP.

Beta and Other Experimental Features

Experimental features are not part of the officially delivered scope that SAP guarantees for future releases. This means that experimental features may be changed by

SAP at any time for any reason without notice. Experimental features are not for productive use. You may not demonstrate, test, examine, evaluate or otherwise use

the experimental features in a live operating environment or with data that has not been sufficiently backed up.

The purpose of experimental features is to get feedback early on, allowing customers and partners to influence the future product accordingly. By providing your

feedback (e.g. in the SAP Community), you accept that intellectual property rights of the contributions or derivative works shall remain the exclusive property of SAP.

Example Code

Any software coding and/or code snippets are examples. They are not for productive use. The example code is only intended to better explain and visualize the syntax
and phrasing rules. SAP does not warrant the correctness and completeness of the example code. SAP shall not be liable for errors or damages caused by the use of
example code unless damages have been caused by SAP's gross negligence or willful misconduct.

Bias-Free Language

SAP supports a culture of diversity and inclusion. Whenever possible, we use unbiased language in our documentation to refer to people of all cultures, ethnicities,
genders, and abilities.

Identity and Authentication Management in SAP Business One
Important Disclaimers and Legal Information

PUBLIC

201

www.sap.com/contactsap

© 2026 SAP SE or an SAP affiliate company. All rights reserved.

No part of this publication may be reproduced or transmitted in any form
or for any purpose without the express permission of SAP SE or an SAP
affiliate company. The information contained herein may be changed
without prior notice.

Some software products marketed by SAP SE and its distributors
contain proprietary software components of other software vendors.
National product specifications may vary.

These materials are provided by SAP SE or an SAP affiliate company for
informational purposes only, without representation or warranty of any
kind, and SAP or its affiliated companies shall not be liable for errors or
omissions with respect to the materials. The only warranties for SAP or
SAP affiliate company products and services are those that are set forth
in the express warranty statements accompanying such products and
services, if any. Nothing herein should be construed as constituting an
additional warranty.

SAP and other SAP products and services mentioned herein as well as
their respective logos are trademarks or registered trademarks of SAP
SE (or an SAP affiliate company) in Germany and other countries. All
other product and service names mentioned are the trademarks of their
respective companies.

Please see https://www.sap.com/about/legal/trademark.html for
additional trademark information and notices.

