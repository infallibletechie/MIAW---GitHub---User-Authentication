<html>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

       window.addEventListener("onEmbeddedMessagingReady", () => {
        	console.log(
        		"onEmbeddedMessagingReady event"
        	);
        	embeddedservice_bootstrap.userVerificationAPI.setIdentityToken({
        		identityTokenType: "JWT",
        		identityToken: "eyJraWQiOiIxMjM0NSIsImFsZyI6IlJTMjU2In0.eyJpc3MiOiJ0ZXN0SXNzdWVyIiwic3ViIjoidXNlcjEiLCJleHAiOjE3MTY0MDMwNTgsImlhdCI6MTcxNjM5NzA1OH0.PSiGljFWi90DAcXg6yIH1fbxxKWsSzxfADo0hoxINN-NhR7ogeok8PSWHgnU9-3iYc4y9iJuNSoVR3cUyrlZPgnF_P9JFauLBgkMyqpX9jyIBVQycuyyDYRwa2Qltz09Omjgj8kNLaghyXiKnS4jlON7DhsXnuxfbn7Ca1FU6gPUVuvs63MNNDNn2i5q2HFN0I-KdvQ4xz9QZDrN6mvAYthMmhbd3i6vOUdsGP5yx0IFByq0BcAiwhc_7ZkRVtYb1S6U22PNwDJ5SQrSWd3YonY-QaN6_4iAy_FscgR1pv5z35WTax-uOIqCeU_C-c98DawMu6jWsiBCXdWkiR01_g",
        	});
      });

			embeddedservice_bootstrap.init(
				'00D8Z000000sp44',
				'MIAW_GitHub_User_Authentication',
				'https://infallibletechiemiaw.my.site.com/ESWMIAWGitHubUserAuthe1716397926217',
				{
					scrt2URL: 'https://infallibletechiemiaw.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://infallibletechiemiaw.my.site.com/ESWMIAWGitHubUserAuthe1716397926217/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>  
</html>
