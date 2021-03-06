<h1>NoCA Traffic Encryption</h1>
<p>I wanted a free, secure method of encrypting web traffic, and after reading about some of the under-handed methods used by the powers that be to acquire private keys from Certificate Authorities, I decided to make NoCA. NoCA is intended to bypass CAs, and allow a server administrator to create their own private/public key pair to encrypt all responses sent from the server, so that the client only recieves encrypted data, and an extension (Chrome, Firefox) would intercept the incoming responses, decrypt their bodies, then pass it on to the browser. The extension would also intercept every outgoing request, and encrypt the request bodies.</p>
<p>As an end result, this is going to be open source, so that there is no centralized authority which could be compromised, thereby forgoing the need for a CA, which is often the weakest link in the web security pipeline when trying to protect privacy.</p>

<h3>Possible Technologies</h3>
<ul>
<li><a href="https://www.npmjs.com/package/node-cryptojs-aes">node-cryptojs</a></li>
</ul>