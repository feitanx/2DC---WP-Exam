Since can’t access the backend, I will disable all plugins directly through the database which I have access. I will also deactivate themes by renaming theme folder.
Then I will enable debugging on wp-config.php:

    define('WP_DEBUG', true);
    define('WP_DEBUG_LOG', true);
    define('WP_DEBUG_DISPLAY', false);

This will log errors to a debug.log file located in wp-content/debug.log. I will  check this file to see the specific error and identify the plugin or theme causing the issue.

Once I identify the issue, I will remove the faulty plugin or theme by deleting or renaming its folder.

Then re-enable each plugin one by one in the active_plugins database option or by renaming their folders to verify which one is causing the problem.
