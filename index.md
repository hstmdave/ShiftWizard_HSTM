<html>
  <body>
    <script type='text/javascript'>
	  function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			        window.addEventListener("onEmbeddedMessagingReady", () => {
            embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
                "PreChat_URL": window.location.origin
            });
        });

			embeddedservice_bootstrap.init(
				'00D7X000001PMnZ',
				'ShiftWizard_Messaging',
				'https://healthstream--hstm.sandbox.my.site.com/ESWShiftWizardMessaging1729107285626',
				{
					scrt2URL: 'https://healthstream--hstm.sandbox.my.salesforce-scrt.com'
				}
			);
		  } catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		  }
	  };
    </script>
    <script type='text/javascript' src='https://healthstream--hstm.sandbox.my.site.com/ESWShiftWizardMessaging1729107285626/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  </body>
</html>
