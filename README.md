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
Use this for hide the message
```
jQuery(".notice-dismiss").click(function(){
jQuery(".notice-success").hide();
jQuery(".notice-error").hide();
 ```

## 2) Wordpress Mail

```
$headers[] = 'From: Amit Singh < amit@singh.com >';
$headers[] .= "Content-type: text/html";
	$to = $email;
	$subject = "Registration Confirmation ";
  
	$sent = wp_mail($to, $subject, $message,$headers );
```
