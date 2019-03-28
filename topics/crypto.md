---
layout: topic
title: "Crypto"

level: 3

intro: Cryptography is a corner stone of a trusted web. Without it many services could not be offered reliably. While rust has a strong RNG, the main suite in use isn't pure rust but the (in)famous openssl.

suites:
 - openssl
 - libsodium-sys
 - gpgme
 - ring

rng:
 - rand
 - uuid

passwords:
  - bcrypt
  - djangohashers
  - pwhash

tls:
 - rustls
 - openssl
 - webpki

hashing:
 - fnv
 - twox-hash
 - md5
 - djangohashers
 - blake2-rfc
 - bcrypt
 - pwhash

algorithms:
 - secp256k1
 - twox-hash
 - blake2-rfc

tooling:
 - tempfile
 - cookie
 - frank_jwt

news_tag: crypto
---


<h2>Suites  {% include level.html level=2 %}</h2>

<p><em>While openssl is the most popular suite, rust-crypto remains the only memory-safe option.</em></p>

{% include packages.html packages=page.suites %}


<h2>Random Number Generators  {% include level.html level=0 %}</h2>

{% include packages.html packages=page.rng %}


<h2>Password  {% include level.html level=3 %}</h2>

{% include packages.html packages=page.passwords %}


<h2>TLS  {% include level.html level=3 %}</h2>

{% include packages.html packages=page.tls %}



<h2>Tooling  {% include level.html level=4 %}</h2>

<p><em>Tooling is great, just a little scarce...</em></p>

{% include packages.html packages=page.tooling %}


---

<h2>Also</h2>


<h3>Hashing  {% include level.html level=3 %}</h3>

{% include packages.html packages=page.hashing %}


<h3>Algorithms  {% include level.html level=3 %}</h3>

{% include packages.html packages=page.algorithms %}
