<!--
This file is auto-generated and will be re-generated every time the docs are updated.
To modify it, go to its source at https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/create_app_on_managed_play_store.rb
-->

# create_app_on_managed_play_store


Create Managed Google Play Apps




> Create new apps on Managed Google Play.


create_app_on_managed_play_store ||
---|---
Supported platforms | android
Author | @janpio



## 1 Example

```ruby
create_app_on_managed_play_store(
  json_key: 'path/to/you/json/key/file',
  developer_account_id: 'developer_account_id', # obtained using the `get_managed_play_store_publishing_rights` action (or looking at the Play Console url)
  app_title: 'Your app title',
  language: 'en_US', # primary app language in BCP 47 format
  apk: '/files/app-release.apk'
)
```





## Parameters

Key | Description | Default
----|-------------|--------
  `json_key` | The path to a file containing service account JSON, used to authenticate with Google | [*](#parameters-legend-dynamic)
  `json_key_data` | The raw service account JSON data used to authenticate with Google | [*](#parameters-legend-dynamic)
  `developer_account_id` | The ID of your Google Play Console account. Can be obtained from the URL when you log in (`https://play.google.com/apps/publish/?account=...` or when you 'Obtain private app publishing rights' (https://developers.google.com/android/work/play/custom-app-api/get-started#retrieve_the_developer_account_id) | [*](#parameters-legend-dynamic)
  `apk` | Path to the APK file to upload | [*](#parameters-legend-dynamic)
  `app_title` | App Title | 
  `language` | Default app language (e.g. 'en_US') | `en_US`
  `root_url` | Root URL for the Google Play API. The provided URL will be used for API calls in place of https://www.googleapis.com/ | 
  `timeout` | Timeout for read, open, and send (in seconds) | `300`

<em id="parameters-legend-dynamic">* = default value is dependent on the user's system</em>


<hr />
To show the documentation in your terminal, run
```no-highlight
fastlane action create_app_on_managed_play_store
```

<a href="https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/create_app_on_managed_play_store.rb" target="_blank">View source code</a>

<hr />

<a href="/actions/"><b>Back to actions</b></a>
