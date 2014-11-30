# PHPCI plugin for Redmine integration

This PHPCI plugin allows to update the Redmine issues with build results.

## Configuration Options

* **enabled** - Required - The plugin is enabled or disabled (example, `enabled: true`).
* **status** - Redmine issue will change status to this status (example, `status: 4`).
* **prev_status** - Current redmine issue's status (example, `prev_status: 2`).
* **percent** - Redmine issue will change `done_ratio` to *percent* value (example, `percent: 80`).
* **lang** - Redmine issue's notes language. Can be `en` or `ru` (example, `lang: en`).
* **issue_regexp** - Mask for issue id searching in branch string (example, `issue_regexp: "/task-(\d+)/"`).
 
## Build Settings

* **redmine** - All child properties are required
  * **server** - Redmine server base URL (example, `server: http://redmine.example.com`)
  * **api_key** - Redmine API key (example, `api_key: 3hfsdyt3fsd87xuv23jhsd`)
