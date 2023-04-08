# Wordpress-Functions

## 1) Custom Message on Menu Page
```
<div id="message" class="updated notice notice-success is-dismissible" style="display:none"><p>Order updated.</p><button type="button" class="notice-dismiss"><span class="screen-reader-text">Dismiss this notice.</span></button></div>
<div id="message-error" class="error notice notice-error is-dismissible" style="display:none"><p>Error Occured. Try again.</p><button type="button" class="notice-dismiss"><span class="screen-reader-text">Dismiss this notice.</span></button></div>
```

## Tips:

Use this in success
```
jQuery("html, body").animate({ scrollTop: 0 }, "slow");
jQuery(".notice-success").show();
```
Use this in Error
```
jQuery("html, body").animate({ scrollTop: 0 }, "slow");
jQuery(".notice-error").show(); 
```
