# Git Pull

Receives GitHub "Post Receive Hook" messages and conducts a 'git pull' in the configured repository.

Helpful for when you have a non-technical person helping with the code or theme, but aren't familiar with git-pulling to the staging server.

## Directions

Install and enable the module, then go to 'admin/config/delvelopment/git_pull' to set your Git path and Repository path.

Next, go to GitHub and configure '<siteURL>/github/update' as your WebHook URL, under Service Hooks in the repository admin.  Replace <siteURL> above with your site's URL. 

When new code is pushed, drupal will receive the WebHook request, and conduct the git pull as configured. You should see entries in the Recent Log indicating the success of the pull.
