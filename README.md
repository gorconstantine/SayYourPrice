<html>
<body>
<form action="https://postmail.invotes.com/send"  method="post" id="email_form">
<table cellpadding="1" width="100%" align="center"  cellspacing="2">

<tr>
  <td rowspan="3"><input type="image" width="250" height="250" src="https://cdn.home24.net/images/media/catalog/product/original/png/b/u/buerodrehstuhl-marilyn-kunstleder-schwarz-3325569.jpg" /></td>
  <td>For how much (in Euro) would you buy this product?</td>
  <td><input type="text" name="pricebuy" id="pricebuy"  size="30"></td>

<tr>
  <td>For how much (in Euro) should Home24 sell this product?</td>
  <td><input type="text" name="pricesell" id="pricesell" size="30"></td>
</tr>

<tr>
  <td>What is the maximum price for this product?</td>
  <td><input type="text" name="maxprice"  id="maxprice" size="30"></td>
</tr>
</tr>
<tr>
  <td colspan="4"><input type="submit" value="Submit" align="center"/></td>
</tr>
</table>

    <input type="hidden" name="access_token" value="myq6f8k53gjufqn5uv3w8s64" />
      <!-- return urls can be fully qualified -OR-
         start with / for root relative -OR-
         start with . for url relative --> 
    <input type="hidden" name="success_url" value=".?message=Email+Successfully+Sent%21&isError=0" />
    <input type="hidden" name="error_url" value=".?message=Email+could+not+be+sent.&isError=1" />
   

    <!-- set the reply-to address -->
    <!-- <input type="text" name="reply_to"
                placeholder="Your Email" /> -->

    <!-- to append extra fields, use the extra_ prefix.
        Entries will be appended to your message body. -->
    <!-- <input type="text" name="extra_phone_number"
                placeholder="Phone Number" /> -->

    <!-- to split your message into 160 chars
         for an sms gateway -->
    <!-- <input type="hidden"
                name="sms_format" value="true" /> -->
   
    <input id="submit_form" type="submit" value="Send" />
    <!-- not required, but we'd appreciate it if you'd link to us somewhere on your site -->
    <p>Powered by <a href="https://postmail.invotes.com" target="_blank">PostMail</a></p>
</form>
   
</body>  
<!-- optional, prevents the submit button from being pressed more than once -->
<script>
    var submitButton = document.getElementById("submit_form");
    var form = document.getElementById("email_form");
    form.addEventListener("submit", function (e) {
        setTimeout(function() {
            submitButton.value = "Sending...";
            submitButton.disabled = true;
        }, 1);
    });
</script> 


</html>
