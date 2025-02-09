Event: Video 75% Complete
Description: This event is triggered when the video passes the 75% milestone of the total duration of the asset
Attributes:
  - video_session_id (text): Video session unique for each video
  - video_casted (text): A boolean representing whether the video is currently casted
  - video_duration (decimal): The duration of the video in seconds
  - video_title (text): The title of the video
  - video_source (text): The source of the video like "kaltura", "webiny", etc
  - video_id (text): The ID of the video asset from the platform source
  - video_publication_date (text): The publication date for the video in ISO standard format.
  - video_type (text): The type of video: long form, short form, fast tv, etc
  - playhead_position (decimal): The position of the playhead at the time the event occurred.
  - platform_name (text): The name of the platform

Event: Video View Ended
Description: This event is triggered when the video passes the 90% of the total duration of it
Attributes:
  - video_channel_name (text): The name of the FAST TV channel the video is being watched on.
  - video_session_id (text): Video session unique for each video
  - max_playhead_position (decimal): The maximum playhead position for the video "session". Can be higher than the playhead_position in the Video View Ended event due to scrubbing.
  - video_id (text): The ID of the video asset from the platform source
  - total_ads_capacity (decimal): The total potential number of ads that could have been viewed based on the ad serving rules.
  - total_ad_time (decimal): The total number of seconds spent watching ads.
  - total_watch_time (decimal): The total number of seconds a user spent actively watching the video content.
  - video_season_name (text): The name or number of the season if applicable; else "0"
  - video_duration (decimal): The duration of the video in seconds
  - video_casted (text): A boolean representing whether the video is currently casted
  - playhead_position (decimal): The position of the playhead at the time the event occurred.
  - video_type (text): The type of video: long form, short form, fast tv, etc
  - total_session_time (decimal): The total number of seconds a user spent on the same video including pause time and active watch time.
  - total_ads_viewed (decimal): The total number of ads viewed.
  - video_source (text): The source of the video like "kaltura", "webiny", etc
  - video_publication_date (text): The publication date for the video in ISO standard format.
  - video_title (text): The title of the video
  - video_show_name (text): The name of the show, if applicable.
  - video_episode_number (decimal): The number of the episode. (Will be "0" if not numbered).
  - video_completed (text): A true or false value representing whether a user's max_playhead_position ever reached 90% or more of the video_duration.
  - video_show_id (text): The ID of the show, if applicable.
  - platform_name (text): The name of the platform

Event: Click - Event Calendar
Description: This event is triggered when the user clicks on any event available in the Event Calendar Component
Attributes:
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_link (text): The destination URL (href) of the clicked element
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - platform_name (text): The name of the platform

Event: Click - Join Newsletter
Description: This event is triggered when the user clicks on the Explore Offerings button
Attributes:
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_link (text): The destination URL (href) of the clicked element
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Click - Article Strip
Description: This event is triggered when the user clicks on the article strip component
Attributes:
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_link (text): The destination URL (href) of the clicked element
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - platform_name (text): The name of the platform

Event: Click - River Card
Description: This event is triggered when the user clicks on any of the River Card elements
Attributes:
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_link (text): The destination URL (href) of the clicked element
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Click - Close Video Player
Description: This event is triggered when the user clicks on the X icon to close the video player
Attributes:
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - platform_name (text): The name of the platform

Event: Click - Trending Pages
Description: This event is triggered when the user clicks on any of the elements available in the Trending Pages component
Attributes:
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element
  - platform_name (text): The name of the platform
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_component (text): Used on widgets click events for YMAL and Trending

Event: Click - Play Video
Description: This event is triggered when the user clicks on the play button in the player
Attributes:
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Click - Video Playlist Card
Description: This event is triggered when the user clicks on any of the video options available in the video playlist
Attributes:
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Video View Started
Description: This event is triggered every time that a video start playing for the first time
Attributes:
  - video_id (text): The ID of the video asset from the platform source
  - playhead_position (decimal): The position of the playhead at the time the event occurred.
  - video_source (text): The source of the video like "kaltura", "webiny", etc
  - video_title (text): The title of the video
  - video_episode_number (decimal): The number of the episode. (Will be "0" if not numbered).
  - video_session_id (text): Video session unique for each video
  - video_season_name (text): The name or number of the season if applicable; else "0"
  - video_show_name (text): The name of the show, if applicable.
  - video_type (text): The type of video: long form, short form, fast tv, etc
  - video_channel_name (text): The name of the FAST TV channel the video is being watched on.
  - video_show_id (text): The ID of the show, if applicable.
  - video_casted (text): A boolean representing whether the video is currently casted
  - video_duration (decimal): The duration of the video in seconds
  - video_publication_date (text): The publication date for the video in ISO standard format.
  - platform_name (text): The name of the platform

Event: Video Player Impression
Description: This Event is triggered when the player is loaded/viewed in the Page
Attributes:
  - video_source (text): The source of the video like "kaltura", "webiny", etc
  - video_publication_date (text): The publication date for the video in ISO standard format.
  - video_id (text): The ID of the video asset from the platform source
  - video_title (text): The title of the video
  - video_duration (decimal): The duration of the video in seconds
  - video_season_name (text): The name or number of the season if applicable; else "0"
  - video_show_id (text): The ID of the show, if applicable.
  - video_episode_number (decimal): The number of the episode. (Will be "0" if not numbered).
  - video_session_id (text): Video session unique for each video
  - video_channel_name (text): The name of the FAST TV channel the video is being watched on.
  - video_show_name (text): The name of the show, if applicable.
  - video_type (text): The type of video: long form, short form, fast tv, etc
  - video_casted (text): A boolean representing whether the video is currently casted
  - platform_name (text): The name of the platform

Event: Click - Video Player Fullscreen
Description: This event is triggered when the user clicks on the fullscreen button of the video player
Attributes:
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Video Ad Viewed
Description: This Event is triggered when an ad is played in the video player (Pre-roll, Mid-roll)
Attributes:
  - video_casted (text): A boolean representing whether the video is currently casted
  - video_source (text): The source of the video like "kaltura", "webiny", etc
  - ad_duration (decimal): The duration of the ad viewed in seconds.
  - video_title (text): The title of the video
  - creative_id (text): The id of the creative for the ad.
  - video_type (text): The type of video: long form, short form, fast tv, etc
  - ad_id (text): The id for the ad itself.
  - video_duration (decimal): The duration of the video in seconds
  - video_id (text): The ID of the video asset from the platform source
  - playhead_position (decimal): The position of the playhead at the time the event occurred.
  - video_session_id (text): Video session unique for each video
  - video_publication_date (text): The publication date for the video in ISO standard format.
  - platform_name (text): The name of the platform

Event: Click - DTC Widget Logo
Description: This event is triggered when the user clicks on the Motortrend logo available in the DTC Widget
Attributes:
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_link (text): The destination URL (href) of the clicked element
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - platform_name (text): The name of the platform

Event: Video 25% Complete
Description: This event is triggered when the video passes the 25% milestone of the total duration of the asset
Attributes:
  - video_publication_date (text): The publication date for the video in ISO standard format.
  - video_casted (text): A boolean representing whether the video is currently casted
  - video_source (text): The source of the video like "kaltura", "webiny", etc
  - playhead_position (decimal): The position of the playhead at the time the event occurred.
  - video_duration (decimal): The duration of the video in seconds
  - video_id (text): The ID of the video asset from the platform source
  - video_session_id (text): Video session unique for each video
  - video_title (text): The title of the video
  - video_type (text): The type of video: long form, short form, fast tv, etc
  - platform_name (text): The name of the platform

Event: Video 50% Complete
Description: This event is triggered when the video passes the 50% milestone of the total duration of the asset
Attributes:
  - video_source (text): The source of the video like "kaltura", "webiny", etc
  - video_id (text): The ID of the video asset from the platform source
  - video_duration (decimal): The duration of the video in seconds
  - video_type (text): The type of video: long form, short form, fast tv, etc
  - video_title (text): The title of the video
  - video_publication_date (text): The publication date for the video in ISO standard format.
  - playhead_position (decimal): The position of the playhead at the time the event occurred.
  - video_session_id (text): Video session unique for each video
  - video_casted (text): A boolean representing whether the video is currently casted
  - platform_name (text): The name of the platform

Event: Click - Text Insert
Description: This event is triggered when the user clicks on any of the text insert links available in the articles
Attributes:
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_link (text): The destination URL (href) of the clicked element
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Video 100% Complete
Description: This event is triggered when the video passes the 100% milestone of the total duration of the asset
Attributes:
  - video_duration (decimal): The duration of the video in seconds
  - video_publication_date (text): The publication date for the video in ISO standard format.
  - video_session_id (text): Video session unique for each video
  - video_type (text): The type of video: long form, short form, fast tv, etc
  - video_source (text): The source of the video like "kaltura", "webiny", etc
  - video_casted (text): A boolean representing whether the video is currently casted
  - video_title (text): The title of the video
  - video_id (text): The ID of the video asset from the platform source
  - playhead_position (decimal): The position of the playhead at the time the event occurred.
  - platform_name (text): The name of the platform

Event: Click - DTC Widget Card
Description: This event is triggered when the user clicks on a card in the DTC widget
Attributes:
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_link (text): The destination URL (href) of the clicked element
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - platform_name (text): The name of the platform

Event: Click - Bright Edge
Description: This event is triggered when the user clicks on any element available in the Bright Edge component
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_link (text): The destination URL (href) of the clicked element
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - platform_name (text): The name of the platform

Event: Click - See all Photos
Description: This event is triggered when the user clicks on the See all photos button available in the Articles to access it the photo gallery
Attributes:
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_link (text): The destination URL (href) of the clicked element
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - platform_name (text): The name of the platform

Event: Click - Return to Article
Description: This event is triggered when the user clicks on the icon to return from the Photo Gallery to the Article related
Attributes:
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_link (text): The destination URL (href) of the clicked element
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - platform_name (text): The name of the platform
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.

Event: Click - Hero Card
Description: This Event is triggered when the user clicks on any element on the Hero card
Attributes:
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_link (text): The destination URL (href) of the clicked element
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Click - Mute Video
Description: This event is triggered when the user clicks on the Mute Button of the video player
Attributes:
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - platform_name (text): The name of the platform

Event: Click - Share Social Media
Description: This Event is triggered when the user clicks on the share to Social Media icon (Facebook, X)
Attributes:
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_link (text): The destination URL (href) of the clicked element
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Click - DTC Widget Banner
Description: This event is triggered when the user clicks on the DTC Widget Banner
Attributes:
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_link (text): The destination URL (href) of the clicked element
  - platform_name (text): The name of the platform

Event: Click - Global Footer
Description: This event is triggered when the user clicks on any of the footer options
Attributes:
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_link (text): The destination URL (href) of the clicked element
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Click - Film Strip Card
Description: Click event on Film strip
Attributes:
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_link (text): The destination URL (href) of the clicked element
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: User Engagement Summary
Description: This event is triggered when: The user leaves a page, when the user change of the tab in the browser, after 5 minutes of inactivity or when the user closes the browser.
Attributes:
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - content_sections_total (decimal): The number of page breaks of photos or any content "sections" on the page/screen
  - ads_rendered (decimal): The count of ads where the html content is written to the page successfully (Client)
  - inventory_widget_viewed (text): Whether or not the user viewed the car inventory widget
  - comments_posted (decimal): The total number of comments posted by the user on a particular article.
  - ads_responded_in_avg (integer): average time in ms of ad response time - request time
  - ads_requested (decimal): The count of ad requests page on the page (Client)
  - scroll_depth (decimal): The maximum vertical distance a user saw on a view. The minimum should always be the height of the screen.
  - content_sections_viewed_percent (decimal): The percentage of page breaks or photos or any content "sections" on the page/screen that the user has viewed.
  - ads_responded (integer): number of ads whose request was successful
  - ads_rendered_in_avg (integer): average time in ms of ad render time - response time
  - ads_gpt_loaded (boolean): boolean that defines whether the gpt sdk was loaded when ues fired
  - inventory_widget_type (text): The type of inventory widget present on the page if there is one. If this value is not set there is no widget present.
  - ads_loaded (decimal): The count of ads that rendered fully and can be viewed by a user if the ad scrolls into the viewport (Client)
  - ads_first_request_time (integer): time in ms of first ad request - page load time
  - ads_queue_empty (boolean): boolean that defines whether the gpt queue was ever populated by the time ues fired
  - view_height (decimal): The total loaded height of the view at the time the event fired.
  - ads_requested_in_avg (integer): This is the number of milliseconds for avg ad request time
  - content_sections_viewed (decimal): The number of page breaks or photos or any content "sections" on the page/screen that the user has viewed.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - ad_blocker_enabled (text): The number of ad impressions
  - scroll_percentage (decimal): The scroll percentage of a page as a decimal to two decimal places.
  - platform_name (text): The name of the platform
  - ads_impressed (decimal): The number of ad impressions
  - ads_impl_load_time (integer): Time that takes to load the impl script
  - ads_gpt_load_time (integer): time that takes to load the gpt script
  - ads_impl_loaded (boolean): boolean to identify if script impl loaded or not
  - ads_impl_status (text): Status returned in the network tab to load imp script
  - ads_gpt_status (text): Status returned in the network tab to load gpt script

Event: Email Click
Description: This event is triggered when the user clicks on any of the elements in the email received
Attributes:
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - content_type (text): The type of content being shown.
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - element_link (text): The destination URL (href) of the clicked element
  - email_subject (text): The titleor subject of the email
  - platform_name (text): The name of the platform

Event: Email Unsubscribe
Description: Event triggered when the user click on the unsubscribe for any of the newsletters
Attributes:
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - content_type (text): The type of content being shown.
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - email_subject (text): The titleor subject of the email
  - platform_name (text): The name of the platform

Event: Ad Impression
Description: This event is triggered when an ad is loaded onto the page (viewed impression is a separate event)
Attributes:
  - ad_size (text): Size of the ad
  - ad_campaign_id (text): The ID of the campaign in GAM.
  - ad_slot_id (text): The ad slot ID from Google Ad Manager.
  - ad_advertiser_id (text): The ID of the advertiser in GAM.
  - ad_line_item_id (text): The ID of the line item in GAM.
  - ad_creative_id (text): The ID of the creative of the ad in GAM.
  - ad_creative_template_id (text): The ID of the creative template in GAM.
  - ad_path (text): The ad targeting path from Google Ad Manager.
  - platform_name (text): The name of the platform
  - ad_back_fill (text): Wheter the ad is considered backfill (programmatic)
  - ad_refresh_type (text): Name of the refresh type (no_interaction, user_interaction, out_of_viewport, tab_switch)
  - ad_refreshed (text): Flag to identify if the ad_impression was due to a ad refresh action

Event: Email Open
Description: This event is triggered when the user opens the mail received
Attributes:
  - email_subject (text): The titleor subject of the email
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - content_type (text): The type of content being shown.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - platform_name (text): The name of the platform

Event: Email Send
Description: This Event is triggered on the backend every time a new email is sent to the user
Attributes:
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - content_type (text): The type of content being shown.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - email_subject (text): The titleor subject of the email
  - platform_name (text): The name of the platform

Event: Email Delivery
Description: This event is triggered on the backend every time that an email is confirmed as delivery (not bounced)
Attributes:
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - content_type (text): The type of content being shown.
  - platform_name (text): The name of the platform
  - email_subject (text): The titleor subject of the email

Event: Email Bounce
Description: Email event triggered on the backend when the email service receive a notification of an email bounce
Attributes:
  - email_subject (text): The titleor subject of the email
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - content_type (text): The type of content being shown.
  - email_list_name (text): The name of the email list like "MotorTrend Newsletter", "HotRod Newsletter" etc
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - platform_name (text): The name of the platform

Event: Click - Related Articles
Description: This event is triggered when the user clicks on any of the articles available in the Related Articles component
Attributes:
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - element_link (text): The destination URL (href) of the clicked element
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - platform_name (text): The name of the platform

Event: Click - Unmute Video Player
Description: This event is triggered when the user clicks on the click to unmute button on the video player
Attributes:
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - mp_event_name (text): This is used for creating the event names in the mParticle data plan instead of the name in Anamap
  - platform_name (text): The name of the platform

Event: Click - You May Also Like
Description: Event triggered when user clicks on the You May Also Like cards
Attributes:
  - element_content (text): The content of the element being clicked. For rail clicks this would be the show name. For CTAs it could be the button text.
  - element_link (text): The destination URL (href) of the clicked element
  - platform_name (text): The name of the platform
  - element_name (text): The name of the specific clickable element. This is more specific than event_name.
  - event_group (text): The more broad group of events this belongs with. For example login type buttons may belong to an Authentication event_group.
  - element_parent (text): The name of the parent container where the clicked element is located.
  - element_position (text): The position number of the element clicked. Ex: If the element parent is a rail then this will be the position number of the element inside the rail.
  - element_id (text): The NextWeb ID of the element. Used for the Click config file.
  - element_component (text): Used on widgets click events for YMAL and Trending
  - element_path (text): A Javascript selector path that can be used in document.querySelector to find the element on the page.
  - event_name (text): The more generic name of the event which can be triggered by multiple UI elements.

Event: Viewed Page/Screen
Description: This is the standard page view event for any kind of pages available in the website (articles, buyers guide, car specs, etc). The content_* attributes are related to each type of content
Attributes:
  - app_name (String): The name of the application or website like "nextweb"
  - car_bodystyle_list (String): Comma separated list with the different body style values selected in car finder page
  - car_data_array (String): An array of JSON objects representing all of the car data present on the page.
  - car_make (String): The make or brand of the car (parent to car model).
  - car_manufacturer (String): The manufacturer of the car (parent to car make).
  - car_model (String): The model of the car.
  - car_segment (String):The car body style such as SUV, Truck, Sedan, etc.
  - car_trim (String):The car trim such as the "LX" in Honda Civic LX.
  - car_year (String): The year of the car.
  - content_all_brands (String): All the brands related to the article
  - content_article_type (String): The article type information
  - content_brand (String): The brand of the content: MotorTrend, Superstreet, HotRod, etc
  - content_category (String):The "Primary Channel" value in Sonic. And (Primary) category in Word Press.
  - content_creation_date (String): The date/time the content was created.
  - content_duration (Number): The length of the content in seconds.
  - content_episode_number (Number): The number of the episode. (Will be "0" if not numbered).
  - content_exclude_sitemap (String): Flag to identify if the article is or not excluded from sitemap
  - content_id (String): The ID for the content, comes from CMS
  - content_images_array (String): Array with the url of all images
  - content_images_count (Number): Total number of images related to the article
  - content_is_stream (String): Whether the content is a live stream vs recorded video.
  - content_meta_description (String): Article metadescription
  - content_metatitle (String): Article metatitle
  - content_modification_date (String): The date/time the content was last modified.
  - content_object_id (String): Custom ID we generate to identify the content
  - content_parent (String): The name of the parent content like the show name. For articles this should be the Primary Vertical (which is the name of the magazine).
  - content_parent_id (String): The ID for the parent content (show ID).
  - content_parent_type (String): The content type of the parent content such as a Show or Magazine.
  - content_photographer_primary (String): The name of the primary photographer
  - content_photographer_secondary (String):The name of the secondary photographer
  - content_primary_section (String): Content Primary section
  - content_publication_date (String): The data/time the content was published.
  - content_save_date (String): Date-time when the action was saved (savedon)
  - content_season_name (String): The number or name (ex: "2022 Series") of the season. (Will be "0" if not available).
  - content_section (String): Based on the Primary Section the firse part before the /
  - content_slug (String): Article Slug
  - content_subsection (String): Based on the Primary Section the second part after the /
  - content_syndication (String): Flag to identify if the article is syndicated
  - content_tags (String): The keywords or tags list from the CMS/VMS.
  - content_tags_array (String): Array with the article tags
  - content_taxonomies_array (String): Array with the different articles taxonomies
  - content_title (String):The title of the content. This could be episode title, show title, article title, car name, etc. depending on the content type.
  - content_type (String): The type of content being shown.
  - content_version (String): The version/revision number for the content
  - content_videos_array (String): Array with the videos related to the article
  - content_videos_count (String): Total number of videos related to the article
  - content_writer_primary (String): The name of the primary writer
  - content_writer_secondary (String): The name of the secondary writer
  - content_year (String): The year of the magazine publication.
  - device_family (String): The name of the device family. Ex: Android TV, Fire TV, etc
  - device_model (String): The name of the device manufacturer and model name. Ex: Sony - ATSV458u
  - device_screen_area (Number):The area of the device screen in pixels
  - device_screen_height (Number): The height of the device screen in pixels
  - device_screen_width (Number): The width of the device screen in pixels
  - device_user_agent (String): The user agent string of the browser. navigator.userAgent
  - device_user_agent_bot (String): The type of bot/crawler identified by parsing the user agent string (e.g., googlebot or bingbot)
  - dq_modifications (String):An array listing where modifications have been made to the event by the Data Quality Pipeline
  - inventory_widget_present (String):Whether or not the car inventory widget is present on the page
  - magazine_year (String): The year of the magazine publication.
  - nitrous_version (String):Nitrous SDK Version
  - page_id(String): The ID of a specific page view. Changes with each page reload.
  - platform_name (String): The name of the platform
  - session_id (String): The ID of the session. Changes after 30 minutes of inactivity.
  - true_view (String): A boolean representing whether the page view is a true page view or not
  - view_canonical_path (String):The canonical path of the current page.
  - view_canonical_url (String): The full canonical URL of the page
  - view_count (Number): Each time a user views a page in a session this number increments. view_count = 1 represents the first page view in a session.
  - view_domain (String): The domain of the page. Ex. "motortrend.com"
  - view_group (String): The group of pages or screens that the view belongs to.
  - view_name (String): The name of the page or screen.
  - view_name_previous (String): The name of the previous page or screen.
  - view_path (String):The path of the page. Ex. "/reviews" as seen in the user's browser
  - view_sponsored (String): Flag to identify if the page is sponsored or not
  - view_state (String): The state of a page or screen if it has time limited versions like a countdown, live, and was-live version.
  - view_subdomain (String):The value of the subdomain
  - view_template (String): The template of the page like CTT, AMP, Article, etc. Applies to web.
  - view_url (String): The full URL of the page as seen in the browser of the user.
  - window_id (String): The ID of a specific tab or window. Unique to each tab or window the user has open.
