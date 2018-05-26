Path for all the conf files:
etc/asterisk

extensions.conf, sip.conf, pjsip.conf has to be updated per the scripts in the repository

Any VOIP softphone application has to be used to make a call for the extension specified in extension.conf

username and password in the VOIP application has to be configured accordingly.

If the VOIP SoftPhone application is not able to communicate to the asteriskNow one possible error could be 
that both of them are trying to talk on the same Ports. Hence in the VOIP softphone application change the
port Number to 5061 (instead of 5060)

Domain in the VOIP Softphone application has to be the IP address of the machine on which
asterisk service is configured

After all the above is configured, one can make a call from the application to the extension mentioned in
extension.conf and one should find output in the asterisk console.
