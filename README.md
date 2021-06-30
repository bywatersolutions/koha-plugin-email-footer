# Email Footer plugin for Koha

This plugin, once installed and configured, will automatically add a footer to every outgoing email sent from Koha to patrons.

# Downloading

From the [release page](https://github.com/bywatersolutions/koha-plugin-email-footer/releases) you can download the latest release in `kpz` format.

# Installation

This plugin requires no special installation. Simply download the kpz file from the releases page, then upload it to Koha from Administration / Plugins.

# Configuration

Notices are configured from koha-conf.xml, inside the `config` block. For example:
```xml
 <email_footers>
    <footer type="text">
You are receiving this email because you opted in through your agreement with the library.
For more information on library notifications, please contact us at &lt;phone number&gt;.
    </footer>
    <footer type="html">
You are receiving this email because you opted in through your agreement with the library.
For more information on library notifications, please contact us at &lt;phone number&gt;.
    </footer>
    <footer lang="fr-FR" type="text">
You are receiving this email because you opted in through your agreement with the library.
Pour plus d'informations sur les notifications de la bibliothèque, veuillez nous contacter au &lt;phone number&gt;.
    </footer>
    <footer lang="fr-FR" type="html">
Vous recevez cet e-mail car vous vous êtes inscrit via votre accord avec la bibliothèque.
Pour plus d'informations sur les notifications de la bibliothèque, veuillez nous contacter au &lt;phone number&gt;.
    </footer>
 </email_footers>
```
