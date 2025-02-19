# PHP Website Brief

## Purpose
This document serves as a single source of truth for this project. All details concerning this project, from planning to deployment, are included in this brief. 

## Overview
This project will deliver a fully functional website that's built with Laravel, a PHP framework, plus HTML5, CSS3, and JavaScript. 

## Project Requirements
* Login/Logout for all users


* User Roles:
    * Admin - Has full access to everything in the website, plus full CRUD capabilities

    * Editor - Has access to all contributor content, with the ability to CRUD that content. The Editor 
      may also create, update, and delete content of their own creation. 

    * Contributor/Author - Has access to the page editor to create, publish, and update content. 
      Deletion of content has to be authorized by the Editor.

    * Subcriber - Only has access to the public-facing part of the website. All subscribers will receive emails
      and notifications when new content is published. Subscribers may opt out of subscriptions at any time. 


* Admin dashboard with views that communicate:
    * Overall site traffic
        * Number of unique visits per day
        * Average length of engagement
        * Number of bounces

    * Post engagement for all published posts and articles
        * Most visited post
        * Least visited post
        * Posts with no visits
        * Average engagement of all posts

    * User activity:
        * Editors - Track how much time editor spends in Editor role
        * Contributors - Track how much content each contributor publishes
        * Subscribers - Track total subscriptions, new subscriptions, active subscriptions, and cancelled subscriptions.

* Editor dashboard with views that communicate: 
    * Drafts that need editing
    * Contributors activity 
    * Activity on recently published posts
    * View of most read posts
    * View of least read posts
    * View of posts that haven't been visited at all


* Contributor dashboard with views that communicate:
    * Post engagement for posts written by the contributor
    * Posts that have been edited 
    * Posts that are ready for final edits
    * Most engaging posts
    * Least engaging posts
    * Posts that got no visits at all

    
* Admins, Editors, and Contributors 
    * Post Editor to create, save, draft, publish, and delete posts
    * Post editor will include: 
        * Rich text editor
        * Image placement
        * Banner image for post
        * Ability to add mulitple images to a single post


* Security
    * Website must use https at all times
    * Users must authenticate with verifiable email address
    * Include 2FA that allows:
        * Use of biometrics
        * Use of PIN
        * Use of a single, generated code that's emailed to the user
    * Require the use of secure passwords for all users, including the admin


## Constraints

* Database access 
    * Only the site admin or webmaster/server admin will have access to the database
    * No other users are allowed to access the database by any means

* User roles are to be configured such that they only have the minimum permissions needed to perform their roles

* No http - https only for the entire site

* Secure web forms to prevent code injection attacks and XSS (cross scripting) attacks
* Disallow weak passwords
* Published pages are to be static HTML with dynamic or interactive elements
* Disallow the use of special characters in post URLs (only common punctuation plus the hyphen and forward slash are allowed)
* Block non-subscribers from any activities or interactions outside of upvotes/downvotes for a post or sharing the post on their social media



    

