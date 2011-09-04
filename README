# gpg-web #

The goal of this project is to provide a specification (and implementation) for
authenticating and encrypting web requests (HTTP) using GPG in the browser.

## Motivation ##

Every modern browser has support for encryption and authentication via SSL,
so why bother re-solving the problem?
 * Because we can. GPG is a great, and under-used bit of software. I wanted
   to flex my coding muscles, and this is a problem I've been thinking about
   for a while.
 * Cut out CAs. In most cases, it's easier and probably more secure to use an
   authentication certificate issues by a CA for use over SSL. I have no way
   of adding most web servers to my web of trust in a sensible way, and I can
   probably trust that Verisign and Co. know whether or not I should accept a
   certificate better than I do. However, there are plenty of cases when one
   might not want to trust a CA certificate (recent breaches of security
   including the Dutch DigiNotar signing certificate being a case in point).
   Alternatively, you might prefer to be able to issue and use your own
   certificates, which can be reasonably verified by a web of trust within your
   own organisation, or you might even have legitimate reasons not to trust the
   standard CAs (for example, do we really trust that Verisign wouldn't issue
   the US government a certificate for wikileaks.org?)

## Background ##

This is not the first time anyone has had a go at implementing GPG
authentication in the browser. FireGPG was a browser plugin for verifying and
performing encrypt/decrypt operations on text in the browser, and this protocol
is inspired by gpgAuth. I chose not to fork gpgAuth, as I felt the spec was
unclear - I would have to have gleaned it from the implementation examples.
There may well be similarities to that project found here, and credit should
be given where credit is due - I think the gpgAuth project is a noble effort.
