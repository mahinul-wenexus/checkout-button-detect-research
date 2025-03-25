# RESEARCH: automated checkout button detection 


* Most checkout button have attribute `name="checkout"`.
* Check for layout. Many checkout button tends to be in flex to have two button `view cart` & `checkout` in one line. in that case, look for parent element and then add button as adjacent element in parent
* Some `mini-cart` have only `view-cart` button. It doesn't have checkout button.
* If there is no selector with `name='checkout'` then search for form with `action='checkout'`. [sample data details: it had button with type='submit' and form with action='/checkout'. There was only one form in the whole DOM]
* There are buttons with `<a href="/checkout" class="btn btn--large btn--wide">Checkout</a>`


<br>
<br>

### Hidden Elements
> There are some hidden elements. Have to check if i. the element is display:none or not. ii. The element could be `behind` another element(this specific problem might cause issue if we try to add adjacent element to it).

