
<script type='text/javascript'>
	  function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			embeddedservice_bootstrap.settings.chatButtonPosition = "1%, 1%"; // Setting chat button position, measured from bottom right

			window.addEventListener("onEmbeddedMessagingReady", () => {
				embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({
					"PreChat_URL": window.location.origin
				});
			});

			embeddedservice_bootstrap.init(
				'00DWL000003W4Bd',
				'Streamy_ShiftWizard',
				'https://healthstream--hstm.sandbox.my.site.com/ESWStreamyShiftWizard1737139032082',
				{
					scrt2URL: 'https://healthstream--hstm.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://healthstream--hstm.sandbox.my.site.com/ESWStreamyShiftWizard1737139032082/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>


