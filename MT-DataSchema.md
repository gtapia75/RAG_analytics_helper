Event: Video 75% Complete
Description: This event is triggered when the video passes the 75% milestone of the total duration of the asset
Attributes:
  - video_session_id (text): Video session unique for each video
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_id (text): The ID of the video asset from the platform source
  - video_id (text): The ID of the video asset from the platform source

Event: Video View Ended
Description: This event is triggered when the video passes the 90% of the total duration of it
Attributes:
  - video_session_id (text): Video session unique for each video
  - max_playhead_position (decimal): The maximum playhead position for the video "session". Can be higher than the playhead_position in the Video View Ended event due to scrubbing.
  - video_id (text): The ID of the video asset from the platform source
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_completed (text): A true or false value representing whether a user's max_playhead_position ever reached 90% or more of the video_duration.

Event: Click - Event Calendar
Description: This event is triggered when the user clicks on any event available in the Event Calendar Component
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Join Newsletter
Description: This event is triggered when the user clicks on the Explore Offerings button
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Article Strip
Description: This event is triggered when the user clicks on the article strip component
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - River Card
Description: This event is triggered when the user clicks on any of the River Card elements
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Close Video Player
Description: This event is triggered when the user clicks on the X icon to close the video player
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Trending Pages
Description: This event is triggered when the user clicks on any of the elements available in the Trending Pages component
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Play Video
Description: This event is triggered when the user clicks on the play button in the player
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Video Playlist Card
Description: This event is triggered when the user clicks on any of the video options available in the video playlist
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Video View Started
Description: This event is triggered every time that a video start playing for the first time
Attributes:
  - video_session_id (text): Video session unique for each video
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_id (text): The ID of the video asset from the platform source
  - video_id (text): The ID of the video asset from the platform source

Event: Video Player Impression
Description: This Event is triggered when the player is loaded/viewed in the Page
Attributes:
  - video_session_id (text): Video session unique for each video
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_id (text): The ID of the video asset from the platform source
  - video_id (text): The ID of the video asset from the platform source

Event: Click - Video Player Fullscreen
Description: This event is triggered when the user clicks on the fullscreen button of the video player
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Video Ad Viewed
Description: This Event is triggered when an ad is played in the video player (Pre-roll, Mid-roll)
Attributes:
  - video_session_id (text): Video session unique for each video
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_id (text): The ID of the video asset from the platform source
  - video_id (text): The ID of the video asset from the platform source

Event: Click - DTC Widget Logo
Description: This event is triggered when the user clicks on the Motortrend logo available in the DTC Widget
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element


Event: Video 25% Complete
Description: This event is triggered when the video passes the 25% milestone of the total duration of the asset
Attributes:
  - video_session_id (text): Video session unique for each video
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_id (text): The ID of the video asset from the platform source
  - video_id (text): The ID of the video asset from the platform source
  - 
Event: Video 50% Complete
Description: This event is triggered when the video passes the 50% milestone of the total duration of the asset
Attributes:
  - video_session_id (text): Video session unique for each video
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_id (text): The ID of the video asset from the platform source
  - video_id (text): The ID of the video asset from the platform source
  - 

Event: Click - Text Insert
Description: This event is triggered when the user clicks on any of the text insert links available in the articles
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Video 100% Complete
Description: This event is triggered when the video passes the 100% milestone of the total duration of the asset
Attributes:
  - video_session_id (text): Video session unique for each video
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_id (text): The ID of the video asset from the platform source
  - video_id (text): The ID of the video asset from the platform source

Event: Click - DTC Widget Card
Description: This event is triggered when the user clicks on a card in the DTC widget
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Bright Edge
Description: This event is triggered when the user clicks on any element available in the Bright Edge component
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - See all Photos
Description: This event is triggered when the user clicks on the See all photos button available in the Articles to access it the photo gallery
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Return to Article
Description: This event is triggered when the user clicks on the icon to return from the Photo Gallery to the Article related
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Hero Card
Description: This Event is triggered when the user clicks on any element on the Hero card
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Mute Video
Description: This event is triggered when the user clicks on the Mute Button of the video player
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Share Social Media
Description: This Event is triggered when the user clicks on the share to Social Media icon (Facebook, X)
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - DTC Widget Banner
Description: This event is triggered when the user clicks on the DTC Widget Banner
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Global Footer
Description: This event is triggered when the user clicks on any of the footer options
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Film Strip Card
Description: Click event on Film strip
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: User Engagement Summary
Description: This event is triggered when: The user leaves a page, when the user change of the tab in the browser, after 5 minutes of inactivity or when the user closes the browser.
Attributes:
  - scroll_depth (decimal): The maximum vertical distance a user saw on a view. The minimum should always be the height of the screen.
  - view_height (decimal): The total loaded height of the view at the time the event fired.
  - ad_blocker_enabled (text): The number of ad impressions
  - scroll_percentage (decimal): The scroll percentage of a page as a decimal to two decimal places.

Event: Email Click
Description: This event is triggered when the user clicks on any of the elements in the email received
Attributes:
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - element_link (text): The destination URL (href) of the clicked element
  - email_subject (text): The titleor subject of the email

Event: Email Unsubscribe
Description: Event triggered when the user click on the unsubscribe for any of the newsletters
Attributes:
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - email_subject (text): The titleor subject of the email

Event: Ad Impression
Description: This event is triggered when an ad is loaded onto the page (viewed impression is a separate event)
Attributes:
  - ad_size (text): Size of the ad
  - ad_campaign_id (text): The ID of the campaign in GAM.
  - ad_slot_id (text): The ad slot ID from Google Ad Manager.

Event: Email Open
Description: This event is triggered when the user opens the mail received
Attributes:
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.

Event: Email Send
Description: This Event is triggered on the backend every time a new email is sent to the user
Attributes:
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - email_subject (text): The titleor subject of the email

Event: Email Delivery
Description: This event is triggered on the backend every time that an email is confirmed as delivery (not bounced)
Attributes:
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - email_subject (text): The title or subject of the email

Event: Email Bounce
Description: Email event triggered on the backend when the email service receive a notification of an email bounce
Attributes:
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.

Event: Click - Related Articles
Description: This event is triggered when the user clicks on any of the articles available in the Related Articles component
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - Unmute Video Player
Description: This event is triggered when the user clicks on the click to unmute button on the video player
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Click - You May Also Like
Description: Event triggered when user clicks on the You May Also Like cards
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element

Event: Viewed Page/Screen
Description: This is the standard page view event for any kind of pages available in the website (articles, buyers guide, car specs, etc). The content_* attributes are related to each type of content
Attributes:
  - content_article_type (String): The article type information
  - content_brand (String): The brand of the content: MotorTrend, Superstreet, HotRod, etc
  - content_category (String):The "Primary Channel" value in Sonic. And (Primary) category in Word Press.
  - content_creation_date (String): The date/time the content was created.
  - content_id (String): The ID for the content, comes from CMS
  - content_metatitle (String): Article metatitle
  - content_section (String): Based on the Primary Section the firse part before the /
  - content_title (String):The title of the content. This could be episode title, show title, article title, car name, etc. depending on the content type.
  - device_family (String): The name of the device family. Ex: Android TV, Fire TV, etc
  - device_screen_area (Number):The area of the device screen in pixels
  - device_screen_height (Number): The height of the device screen in pixels
  - device_user_agent (String): The user agent string of the browser. navigator.userAgent
  - page_id(String): The ID of a specific page view. Changes with each page reload.
  - view_domain (String): The domain of the page. Ex. "motortrend.com"
