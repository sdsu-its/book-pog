# Logging into Blackboard

As of January 5th, most users will login to Blackboard via SDSUid. Some users with GUI accounts \(some staff members, ITS staff, clicker users, CES students, etc\) will still need to login with a username and password, which can be accomplished via the [Speakeasy method](#speakeasy-method) listed below.

## SSO Login Issues

There are a few common issues associated with login in via SDSUid \(SAML SSO\), with the associated solution listed below. There are also macros in [Desk](/ops/fs/desk.md) for all of these common responses, sometimes with a bit more detail.

### Session Expired

There are situations in which the SSO session will expire, but the user will remain logged in to the Office Portal \(portal.office.com\), because they have elected to stay signed in. This presents an issue when the user attempts to login to Blackboard, as their session is expired, but they will not be prompted to login via the Office365 Portal, as they are still signed in there. To fix this problem, have the user complete the following:  
1. Visit [portal.office.com](https://portal.office.com)  
2. Click on your name in the upper right hand corner and select the "Sign out" option.  
\(It might take a moment to fully sign out\)  
3. Go back to blackboard.sdsu.edu and login using your SDSUid.

To prevent this form occurring in the future, you can advice the user to choose "no" when prompted if they would like to stay signed in after logging into the Office365 Portal. This will result in the user being prompted to login when they try and access a service which uses AAD \(Azure Active Directory, what drives the Office365 Portal\), and their session is expired.

**Macro Name:** BB - SSO Session Expired

### Clear Session

If their session is still valid, which is indicated by the absence of the Session Expired Verbiage on the Error Page presented by Blackboard, we can try clearing the user's browser session. This varies from browser to browser, and is listed for each common browser in the [Reference Section](/ref/clear_session.md).

**Macro Name:** BB - Clear Session

## Speakeasy Method

The new SDSUid login is only for users who previously used their RedID to login to Blackboard. So as not to confuse them, we have hidden the login box for those using GUI accounts.

To reveal these login box, visit the Blackboard homepage. Here, you will notice that the name "San Diego State University" appears twice. Click on the "y" at the end of the word "University" in the second appearance of the name. An "Administrative Login" box and "Password" box should appear at the bottom of the home page. Use these boxes to enter your GUI credentials.

![](/assets/bb-hidden-login.png)

**Macro Name:** BB - GUI Login
