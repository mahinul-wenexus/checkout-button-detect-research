# RESEARCH: automated checkout button detection 


* Most checkout button have attribute `name="checkout"`.
* Check for layout. Many checkout button tends to be in flex to have two button `view cart` & `checkout` in one line. in that case, look for parent element and then add button as adjacent element in parent
