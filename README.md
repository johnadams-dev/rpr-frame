# rpr-frame

RPR's AVM widget for Adams Cameron, served on its own subdomain,
https://rpr.johnadams.org/rpr-frame.html?q=<address>.

The Market Update report (johnadams.org/market-update.html, Workshop repo)
frames this page. It lives on a separate origin so RPR's script can run
unsandboxed (RPR checks the Referer, which a fully sandboxed frame doesn't
send) without access to johnadams.org's stored Workshop sign-in.

RPR's widget token allows `*.johnadams.org`. Display only: Workshop never
reads, stores or calculates with RPR's figure.
