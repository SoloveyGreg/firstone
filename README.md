# firstone
Just the 1-st time 

<!-- main_header -->
<div class="alert alert-info GeneralAffiliateLink">
	{widget id="generalAffiliateLink"}
<br><a href="https://anothersite.com/#a_aid={$refid}" target="_blank" style="position:relative;left:158px;">https://anothersite.com/#a_aid={$refid}</a>



How to add another one?
Create a copy of your active theme if you haven't done one yet, and then search for the file main_header.tpl in which you should find the part with {widget id="generalAffiliateLink"}.
Have a look at Configuration->Tracking settings to see what linking method you are using and also look in Configuration->URL parameter names to get the correct parameter for affiliate ID. Or have a look at an existing General Affiliate Link in some affiliate panel to know how you should create another one.
Generally speaking to add a different URL to the existing one you would need to add the following code right to the {widget id="generalAffiliateLink"}, the example shows an Anchor link with a_aid as affiliate parameter name:
<br><a href="https://anothersite.com/#a_aid={$refid}" target="_blank" style="position:relative;left:158px;">https://anothersite.com/#a_aid={$refid}</a>
Save the changes and set your theme as default. The above code is just an example code without any description for the link and of course you can customize it anyway you want. In the code above the {$refid} will be automatically replaced with the affiliate's referral id when an affiliate is logged in his panel.
