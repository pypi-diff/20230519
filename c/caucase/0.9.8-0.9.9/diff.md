# Comparing `tmp/caucase-0.9.8.tar.gz` & `tmp/caucase-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/caucase-0.9.8.tar", last modified: Mon Jun 29 03:27:25 2020, max compression
+gzip compressed data, was "caucase-0.9.9.tar", last modified: Tue Mar  2 01:12:20 2021, max compression
```

## Comparing `caucase-0.9.8.tar` & `caucase-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2020-06-29 03:27:25.000000 caucase-0.9.8/
--rw-r--r--   0 vincent   (1000) vincent   (1000)    22754 2020-06-29 03:27:25.000000 caucase-0.9.8/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)    68611 2020-06-29 03:25:54.000000 caucase-0.9.8/versioneer.py
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase.egg-info/
--rw-r--r--   0 vincent   (1000) vincent   (1000)      263 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase.egg-info/entry_points.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)      561 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase.egg-info/SOURCES.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase.egg-info/dependency_links.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)    22754 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase.egg-info/PKG-INFO
--rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2020-06-04 09:18:23.000000 caucase-0.9.8/caucase.egg-info/zip-safe
--rw-r--r--   0 vincent   (1000) vincent   (1000)       56 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase.egg-info/requires.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)        8 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase.egg-info/top_level.txt
--rw-r--r--   0 vincent   (1000) vincent   (1000)     2665 2020-06-29 03:25:54.000000 caucase-0.9.8/setup.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    36166 2020-06-29 03:25:54.000000 caucase-0.9.8/COPYING
--rw-r--r--   0 vincent   (1000) vincent   (1000)       86 2020-06-29 03:25:54.000000 caucase-0.9.8/MANIFEST.in
--rw-r--r--   0 vincent   (1000) vincent   (1000)     4402 2020-06-29 03:25:54.000000 caucase-0.9.8/CHANGES.txt
-drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase/
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1088 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/version.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    33243 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/cli.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     4868 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/http_wsgibase.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    98741 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/test.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    33707 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/ca.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1795 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/exceptions.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    37443 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/http.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     1193 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/__init__.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)     3944 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/http_wsgirequesthandler.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    17904 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/storage.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)      497 2020-06-29 03:27:25.000000 caucase-0.9.8/caucase/_version.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    34313 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/wsgi.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    19746 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/utils.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)    11313 2020-06-29 03:25:54.000000 caucase-0.9.8/caucase/client.py
--rw-r--r--   0 vincent   (1000) vincent   (1000)      200 2020-06-29 03:27:25.000000 caucase-0.9.8/setup.cfg
--rw-r--r--   0 vincent   (1000) vincent   (1000)    13941 2020-06-29 03:25:54.000000 caucase-0.9.8/README.rst
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2021-03-02 01:12:20.850977 caucase-0.9.9/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     4903 2021-03-02 01:11:06.000000 caucase-0.9.9/CHANGES.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    36166 2020-06-27 13:16:31.000000 caucase-0.9.9/COPYING
+-rw-r--r--   0 vincent   (1000) vincent   (1000)       86 2018-09-12 01:24:25.000000 caucase-0.9.9/MANIFEST.in
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    25836 2021-03-02 01:12:20.850977 caucase-0.9.9/PKG-INFO
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    16138 2021-02-15 06:40:46.000000 caucase-0.9.9/README.rst
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2021-03-02 01:12:20.850977 caucase-0.9.9/caucase/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1193 2020-06-27 13:20:56.000000 caucase-0.9.9/caucase/__init__.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      497 2021-03-02 01:12:20.850977 caucase-0.9.9/caucase/_version.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    35938 2021-02-15 06:40:46.000000 caucase-0.9.9/caucase/ca.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    34369 2021-02-15 06:38:04.000000 caucase-0.9.9/caucase/cli.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    12737 2021-02-15 06:38:09.000000 caucase-0.9.9/caucase/client.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1795 2020-06-27 13:20:56.000000 caucase-0.9.9/caucase/exceptions.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    38383 2021-02-15 06:38:04.000000 caucase-0.9.9/caucase/http.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     4868 2021-02-01 03:13:24.000000 caucase-0.9.9/caucase/http_wsgibase.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     3944 2018-07-21 12:51:41.000000 caucase-0.9.9/caucase/http_wsgirequesthandler.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    19158 2021-02-15 06:38:04.000000 caucase-0.9.9/caucase/storage.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)   116563 2021-02-22 05:05:04.000000 caucase-0.9.9/caucase/test.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    21691 2021-02-15 06:38:04.000000 caucase-0.9.9/caucase/utils.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     1088 2020-06-27 13:16:31.000000 caucase-0.9.9/caucase/version.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    35786 2021-02-22 01:15:25.000000 caucase-0.9.9/caucase/wsgi.py
+drwxr-xr-x   0 vincent   (1000) vincent   (1000)        0 2021-03-02 01:12:20.850977 caucase-0.9.9/caucase.egg-info/
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    25836 2021-03-02 01:12:20.000000 caucase-0.9.9/caucase.egg-info/PKG-INFO
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      561 2021-03-02 01:12:20.000000 caucase-0.9.9/caucase.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2021-03-02 01:12:20.000000 caucase-0.9.9/caucase.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      263 2021-03-02 01:12:20.000000 caucase-0.9.9/caucase.egg-info/entry_points.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)       56 2021-03-02 01:12:20.000000 caucase-0.9.9/caucase.egg-info/requires.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)        8 2021-03-02 01:12:20.000000 caucase-0.9.9/caucase.egg-info/top_level.txt
+-rw-r--r--   0 vincent   (1000) vincent   (1000)        1 2020-06-27 13:26:41.000000 caucase-0.9.9/caucase.egg-info/zip-safe
+-rw-r--r--   0 vincent   (1000) vincent   (1000)      200 2021-03-02 01:12:20.850977 caucase-0.9.9/setup.cfg
+-rw-r--r--   0 vincent   (1000) vincent   (1000)     2665 2021-02-15 06:38:04.000000 caucase-0.9.9/setup.py
+-rw-r--r--   0 vincent   (1000) vincent   (1000)    68611 2018-09-12 01:24:25.000000 caucase-0.9.9/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `caucase-0.9.8/PKG-INFO` & `caucase-0.9.9/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,474 +1,396 @@
-Metadata-Version: 1.1
-Name: caucase
-Version: 0.9.8
-Summary: Certificate Authority.
-Home-page: https://lab.nexedi.com/nexedi/caucase
-Author: Vincent Pelletier
-Author-email: vincent@nexedi.com
-License: GPLv3+ with wide exception for FOSS
-Description: ..  Note to the editor: beware of implicit inline
-            targets aliasing, keep global title different from all commands
-        
-        =============================================================================
-        caucase - Certificate Authority for Users, Certificate Authority for SErvices
-        =============================================================================
-        
-        Overview
-        ========
-        
-        The goal of caucase is to automate certificate issuance and renewal without
-        constraining how the certificate will be used.
-        
-        For example, there is no assumption that the certificate will be used to
-        secure HTTP, nor to serve anything at all: you may need certificates to
-        authenticate users, or sign your mails, or secure an SQL server socket.
-        
-        As an unfortunate consequence, it is not possible for caucase to automatically
-        validate a signing request content against a service (ex: as one could check
-        the certificate for an HTTPS service was requested by someone with the ability
-        to make it serve a special file).
-        
-        This also means that, while caucase imposes RFC-recommended constraints on many
-        certificate fields and extensions to be worthy of trust, it imposes no
-        constraint at all on subject and alternate subject certificate fields.
-        
-        To still allow certificates to be used, caucase uses itself to authenticate
-        users (humans or otherwise) who implement the validation procedure: they tell
-        caucase what certificates to emit. Once done, any certificate can be
-        prolonged at a simple request of the key holder while the to-renew
-        certificate is still valid (not expired, not revoked).
-        
-        Bootstrapping the system (creating the first service certificate for
-        `caucased`_ to operate on HTTPS, and creating the first user certificate to
-        control further certificate issuance) works by caucase automatically signing a
-        set number of certificates upon submission.
-        
-        Vocabulary
-        ==========
-        
-        Caucase manipulates the following asymmetric cryptography concepts.
-        
-        - Key pair: A private key and corresponding public key. The public key can be
-          derived from the private key, but not the other way around. As a consequence,
-          the private key is itself considered to be a key pair.
-        
-        - Certificate: A certificate is the assurante, by a certificate authority,
-          that a given public key and set of attributes belong to an authorised entity.
-          Abbreviated cert or crt. A certificate is by definition signed by a CA.
-        
-        - Certificate Authority: An entry, arbitrarily trusted (but worthy of trust by
-          its actions and decision) which can issue certificates. Abbreviated CA.
-        
-        - Certificate signing request: A document produced by an entity desiring to get
-          certified, which they send to a certificate authority. The certificate signing
-          request contains the public key and desired set of attributes that the CA
-          should pronounce itself on. The CA has all liberty to issue a different set
-          of attributes, or to not issue a certificate.
-        
-        - Certificate revocation list: Lists the certificates which were issued by a CA
-          but which should not be trusted anymore. This can happen for a variety of
-          reasons: the private key was compromised, or its owning entity should not be
-          trusted anymore (ex: entity's permission to access to protected service was
-          revoked).
-        
-        - PEM: A serialisation mechanism commonly used for various cryptographic data
-          pieces. It relies on base64 so it is 7-bits-safe (unlike DER), and is very
-          commonly supported. Caucase exclusively uses PEM format.
-        
-        Validity period
-        ===============
-        
-        Cryptographic keys wear out as are used and as they age.
-        
-        Of course, they do not bit-rot nor become thinner with use. But each time one
-        uses a key and each minute an attacker had access to a public key, fractions
-        of the private key bits are inevitably leaked, weakening it overall.
-        
-        So keys must be renewed periodically to preserve intended security level. So
-        there is a limited life span to each certificate, including the ones emitted by
-        caucase.
-        
-        The unit duration for caucase-emitted certificates is the "normal" certificate
-        life span. It default to 93 days from the moment the certificate was signed,
-        or about 3 months.
-        
-        Then the CA certificate has a default life span of 4 "normal" certificate
-        validity periods. As CA renewal happens in caucase without x509-level cross
-        signing (by decision, to avoid relying on intermediate CA support on
-        certificate presenter side and instead rely on more widespread
-        multi-CA-certificate support on verifier side), there is a hard lower bound of
-        3 validity periods, under which the CA certificate cannot be reliably renewed
-        without risking certificate validation issues for emitted "normal"
-        certificates. CA certificate renewal is composed of 2 phases:
-        
-        - Passive distribution phase: current CA certificate has a remaining life span
-          of less than 2 "normal" certificate life spans: a new CA certificate is
-          generated and distributed on-demand (on "normal" certificate renewal and
-          issuance, on CRL retrieval with caucase tools...), but not used to sign
-          anything.
-        - Active use phase: new CA certificate is valid for more than one "normal"
-          certificate life span. This means that all existing certificates which are
-          still in active use had to be renewed at least once since the new CA
-          certificate exists. This means all the certificate holders had the
-          opportunity to learn about the new CA certificate. So the new CA certificate
-          starts being used to sign new certificates, and the old CA certificate falls
-          out of use as its signed "normal" certificates expire.
-        
-        By default, all caucase tools will generate a new private key unrelated to the
-        previous one on each certificate renewal.
-        
-        Lastly, there is another limited validity period, although not for the same
-        reasons: the list of revoked certificates also has a maximum life span. In
-        caucase, the CRL is re-generated whenever it is requested and:
-        
-        - there is no previous CRL
-        - previous CRL expired
-        - any revocation happened since previous CRL was created
-        
-        Commands
-        ========
-        
-        Caucase provides several commands to work with certificates.
-        
-        caucase
-        +++++++
-        
-        Reference caucase "one-shot" client.
-        
-        This command is intended to be used for isolated actions:
-        
-        - listing and signing pending certificate signature requests
-        
-        - revoking certificates
-        
-        It is also able to submit certificate signing requests, retrieve signed
-        certificates, requesting certificate renewals and updating both
-        CA certificates and revocation lists, but you may be interested in using
-        `caucase-updater`_ for this instead.
-        
-        caucase-updater
-        +++++++++++++++
-        
-        Reference caucase certificate renewal daemon.
-        
-        Monitors a key pair, corresponding CA certificate and CRL, and renew them
-        before expiration.
-        
-        When the key-pair lacks a signed certificate, issues a pre-existing CSR to
-        caucase server and waits for the certificate to be issued.
-        
-        caucase-probe
-        +++++++++++++
-        
-        Caucase server availability tester.
-        
-        Performs minimal checks to verify a caucase server is available at given URL.
-        
-        caucase-rerequest
-        +++++++++++++++++
-        
-        Utility allowing to re-issue a CSR using a locally-generated private key.
-        
-        Intended to be used in conjunction with `caucase-updater`_ when user cannot
-        generate the CSR on the system where the certificate is desired (ex: automated
-        HTTPS server deployment), where user is not the intended audience for
-        caucase-produced certificate:
-        
-        - User generates a CSR on their own system, and signs it with any key (it will
-          not be needed later
-        - User sends the CSR to the system where the certificate is desired
-        - User gets caucase-rerequest to run on this CSR, producing a new private key
-          and a CSR similar to issued one, but signed with this new private key
-        - From then on, caucase-updater can take over
-        
-        This way, no private key left their original system, and user could still
-        freely customise certificate extensions.
-        
-        caucase-key-id
-        ++++++++++++++
-        
-        Utility displaying the identifier of given key, or the identifier of keys
-        involved in given backup file.
-        
-        Allows identifying users which hold a private key candidate for restoring a
-        caucased backup (see `Restoration procedure`_).
-        
-        caucased
-        ++++++++
-        
-        Reference caucase server daemon.
-        
-        This daemon provides access to both CAU and CAS services over both HTTP and
-        HTTPS.
-        
-        It handles its own certificate issuance and renewal, so there is no need to use
-        `caucase-updater`_ for this service.
-        
-        CORS
-        ----
-        
-        caucased implements CORS protection: when receiving a cross-origin request,
-        it will respond with 401 Unauthorized, with the WWW-Authenticate header set to
-        a custom scheme ("cors") with an "url" parameter containing an URI template
-        with one variable field: "return" (more on it later).
-        
-        Upon receiving this response, the application is expected to render the URL
-        template and redirect the user to resulting URL. There, the user will be
-        informed of the cross-origin access attempt, and offered the choice to grant or
-        deny access to given origin.
-        
-        Once their decision is made, their browser will receive a cookie remembering
-        this decision, and they will be redirected to the URL received in the "return"
-        field received upon above-described redirection.
-        
-        Then, the application should retry the original request, which will be
-        accompanied by that cookie.
-        
-        Backups
-        -------
-        
-        Loosing the CA private key prevents issuing any new certificate trusted by
-        services which trusted the CA. Also, it prevents issuing any new CRL.
-        Recovering from such total loss requires starting a new CA and rolling it out
-        to all services which used the previous one. This is very time-costly.
-        
-        So backups are required.
-        
-        On the other hand, if someone gets their hand on the CA private key, they can
-        issue certificates for themselves, allowing them to authenticate with services
-        trusting the CA managed by caucase - including caucased itself if they issue a
-        user certificate: they can then revoke existing certificates and cause a lot of
-        damage.
-        
-        So backups cannot happen in clear text, they must be encrypted.
-        
-        But the danger of encrypted backups is that by definition they become worthless
-        if they cannot be decrypted. So as many (trusted) entities as possible should
-        be granted the ability to decrypt the backups.
-        
-        The solution proposed by caucased is to encrypt produced backups in a way which
-        allows any of the caucase users to decrypt the archive.
-        
-        As these users are already entrusted with issuing certificates, this puts
-        only a little more power in their hands than they already have. The little
-        extra power they get is that by having unrestricted access to the CA private
-        key they can issue certificates bypassing all caucase restrictions. The
-        proposed parade is to only make the backups available to a limited subset of
-        caucase users when there is an actual disaster, and otherwise keep it out of
-        their reach. This mechanism is not handled by caucase.
-        
-        As there are few trusted users, caucase can keep their still-valid certificates
-        in its database for the duration of their validity with minimal size cost.
-        
-        Backup procedure
-        ----------------
-        
-        Backups happen periodically as long as caucased is running. See
-        `--backup-period` and `--backup-directory`.
-        
-        As discussed above, produced files should be kept out of reach of caucase
-        users until a disaster happens.
-        
-        Restoration procedure
-        ---------------------
-        
-        See `caucased-manage --restore-backup`.
-        
-        To restore, one of the trusted users must voluntarily compromise their own
-        private key, providing it to the administrator in charge of the restoration
-        procedure. Restoration procedure will hence immediately revoke their
-        certificate. They must also provide a CSR generated with a different private
-        key, so that caucase can provide them with a new certificate, so they keep
-        their access only via different credentials.
-        
-        - admin identifies the list of keys which can decipher a backup, and broadcasts
-          that list to key holders
-        
-        - key holders manifest themselves
-        
-        - admin picks a key holder, requests them to provide their existing private key
-          and to generate a new key and accompanying CSR
-        
-        - key holder provide requested items
-        
-        - admin initiates restoration with `--restore-backup` and provides key holder
-          with replacement certificate
-        
-        - admin starts caucased, service is back online.
-        
-        Backup file format
-        ------------------
-        
-        - 64bits: 'caucase\0' magic string
-        
-        - 32bits LE: header length
-        
-        - header: json-encoded header (see below)
-        
-        - encrypted byte stream (aka payload)
-        
-        Header schema (inspired from s/mime, but s/mime tools available do not
-        support at least iterative production or iterative generation)::
-        
-          {
-            "description": "Caucase backup header",
-            "required": ["algorithm", "key_list"],
-            "properties": {
-              "cipher": {
-                "description": "Symetric ciher used for payload",
-                "required": ["name"],
-                "properties": {
-                  "name":
-                    "enum": ["aes256_cbc_pkcs7_hmac_10M_sha256"],
-                    "type": "string"
-                  },
-                  "parameter": {
-                    "description": "Name-dependend clear cipher parameter (ex: IV)",
-                    "type": "string"
-                  }
+..  Note to the editor: beware of implicit inline
+    targets aliasing, keep global title different from all commands
+
+=============================================================================
+caucase - Certificate Authority for Users, Certificate Authority for SErvices
+=============================================================================
+
+Overview
+========
+
+The goal of caucase is to automate certificate issuance and renewal without
+constraining how the certificate will be used.
+
+For example, there is no assumption that the certificate will be used to
+secure HTTP, nor to serve anything at all: you may need certificates to
+authenticate users, or sign your mails, or secure an SQL server socket.
+
+As an unfortunate consequence, it is not possible for caucase to automatically
+validate a signing request content against a service (ex: as one could check
+the certificate for an HTTPS service was requested by someone with the ability
+to make it serve a special file).
+
+This also means that, while caucase imposes RFC-recommended constraints on many
+certificate fields and extensions to be worthy of trust, it imposes no
+constraint at all on subject and alternate subject certificate fields.
+
+To still allow certificates to be used, caucase uses itself to authenticate
+users (humans or otherwise) who implement the validation procedure: they tell
+caucase what certificates to emit. Once done, any certificate can be
+prolonged at a simple request of the key holder while the to-renew
+certificate is still valid (not expired, not revoked).
+
+Bootstrapping the system (creating the first service certificate for
+`caucased`_ to operate on HTTPS, and creating the first user certificate to
+control further certificate issuance) works by caucase automatically signing a
+set number of certificates upon submission.
+
+Vocabulary
+==========
+
+Caucase manipulates the following asymmetric cryptography concepts.
+
+- Key pair: A private key and corresponding public key. The public key can be
+  derived from the private key, but not the other way around. As a consequence,
+  the private key is itself considered to be a key pair.
+
+- Certificate: A certificate is the assurante, by a certificate authority,
+  that a given public key and set of attributes belong to an authorised entity.
+  Abbreviated cert or crt. A certificate is by definition signed by a CA.
+
+- Certificate Authority: An entry, arbitrarily trusted (but worthy of trust by
+  its actions and decision) which can issue certificates. Abbreviated CA.
+
+- Certificate signing request: A document produced by an entity desiring to get
+  certified, which they send to a certificate authority. The certificate signing
+  request contains the public key and desired set of attributes that the CA
+  should pronounce itself on. The CA has all liberty to issue a different set
+  of attributes, or to not issue a certificate.
+
+- Certificate revocation list: Lists the certificates which were issued by a CA
+  but which should not be trusted anymore. This can happen for a variety of
+  reasons: the private key was compromised, or its owning entity should not be
+  trusted anymore (ex: entity's permission to access to protected service was
+  revoked).
+
+- PEM: A serialisation mechanism commonly used for various cryptographic data
+  pieces. It relies on base64 so it is 7-bits-safe (unlike DER), and is very
+  commonly supported. Caucase exclusively uses PEM format.
+
+Validity period
+===============
+
+Cryptographic keys wear out as are used and as they age.
+
+Of course, they do not bit-rot nor become thinner with use. But each time one
+uses a key and each minute an attacker had access to a public key, fractions
+of the private key bits are inevitably leaked, weakening it overall.
+
+So keys must be renewed periodically to preserve intended security level. So
+there is a limited life span to each certificate, including the ones emitted by
+caucase.
+
+The unit duration for caucase-emitted certificates is the "normal" certificate
+life span. It default to 93 days from the moment the certificate was signed,
+or about 3 months.
+
+Then the CA certificate has a default life span of 4 "normal" certificate
+validity periods. As CA renewal happens in caucase without x509-level cross
+signing (by decision, to avoid relying on intermediate CA support on
+certificate presenter side and instead rely on more widespread
+multi-CA-certificate support on verifier side), there is a hard lower bound of
+3 validity periods, under which the CA certificate cannot be reliably renewed
+without risking certificate validation issues for emitted "normal"
+certificates. CA certificate renewal is composed of 2 phases:
+
+- Passive distribution phase: current CA certificate has a remaining life span
+  of less than 2 "normal" certificate life spans: a new CA certificate is
+  generated and distributed on-demand (on "normal" certificate renewal and
+  issuance, on CRL retrieval with caucase tools...), but not used to sign
+  anything.
+- Active use phase: new CA certificate is valid for more than one "normal"
+  certificate life span. This means that all existing certificates which are
+  still in active use had to be renewed at least once since the new CA
+  certificate exists. This means all the certificate holders had the
+  opportunity to learn about the new CA certificate. So the new CA certificate
+  starts being used to sign new certificates, and the old CA certificate falls
+  out of use as its signed "normal" certificates expire.
+
+By default, all caucase tools will generate a new private key unrelated to the
+previous one on each certificate renewal.
+
+Lastly, there is another limited validity period, although not for the same
+reasons: the list of revoked certificates also has a maximum life span. In
+caucase, the CRL is re-generated whenever it is requested and:
+
+- there is no previous CRL
+- previous CRL expired
+- any revocation happened since previous CRL was created
+
+Here is an illustration of the certificate and CA certificate renewal process::
+
+  Time from first caucased start:
+    +--------+--------+--------+--------+--------+--------+--------+-->
+  Certificate 1 validity:      |                 |                 |
+    |[cert 1v1]  [cert 1v3]  [cert 1v5]  [cert 1v7]  [cert 1v9]  [ce...
+    |      [cert 1v2]  [cert 1v4]  [cert 1v6]  [cert 1v8]  [cert 1vA]
+  Certificate 2 validity:      |                 |                 |
+    |    [cert 2v1]  [cert 2v3]| [cert 2v5]  [cert 2v7]  [cert 2v9]|
+    |          [cert 2v2]  [cert 2v4]  [cert 2v6]| [cert 2v8]  [cert...
+  CA certificates validity:    |                 |                 |
+    [ca v1                     |        ]        |                 |
+    |                 [ca v2   |                 |        ]        |
+    |                          |        [ca v3   |                 |...
+    |                          |                 |        [ca v4   |...
+  CRL validity for CA1:        |                 |                 |
+    [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ][ ][  ]        |                 |
+  CRL validity for CA2:        |                 |                 |
+    |                 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ][ ][  ]        |
+  CRL validity for CA3:        |                 |                 |
+    |                          |        [ ][ ][ ][ ][ ][ ][ ][ ][ ][...
+  CA renewal phase:            |                 |                 |
+    |none             |passive |active  |passive |active  |passive |...
+  Active CA:                   |                 |                 |
+    [ca v1                    ][ca v2           ][ca v3            |...
+  Trust anchor:                |                 |                 |
+    [ca v1                     |       ][ca v2   |       ][ca v3   |...
+
+Legend::
+
+  +--------+ : One certificate validity period (default: 93 days)
+
+Points of interest:
+
+- this illustration assumes no revocation happen
+- there usually are 2 simultaneously-valid CA certificates
+- there usually are 2 simultaneously-valid CRLs overall, one per CA certificate
+- the first ``cert 1`` signed by CA v2 is ``cert 1v6``
+- the first ``cert 2`` signed by CA v2 is ``cert 1v5``
+
+Commands
+========
+
+Caucase provides several commands to work with certificates.
+
+caucase
++++++++
+
+Reference caucase "one-shot" client.
+
+This command is intended to be used for isolated actions:
+
+- listing and signing pending certificate signature requests
+
+- revoking certificates
+
+It is also able to submit certificate signing requests, retrieve signed
+certificates, requesting certificate renewals and updating both
+CA certificates and revocation lists, but you may be interested in using
+`caucase-updater`_ for this instead.
+
+caucase-updater
++++++++++++++++
+
+Reference caucase certificate renewal daemon.
+
+Monitors a key pair, corresponding CA certificate and CRL, and renew them
+before expiration.
+
+When the key-pair lacks a signed certificate, issues a pre-existing CSR to
+caucase server and waits for the certificate to be issued.
+
+caucase-probe
++++++++++++++
+
+Caucase server availability tester.
+
+Performs minimal checks to verify a caucase server is available at given URL.
+
+caucase-rerequest
++++++++++++++++++
+
+Utility allowing to re-issue a CSR using a locally-generated private key.
+
+Intended to be used in conjunction with `caucase-updater`_ when user cannot
+generate the CSR on the system where the certificate is desired (ex: automated
+HTTPS server deployment), where user is not the intended audience for
+caucase-produced certificate:
+
+- User generates a CSR on their own system, and signs it with any key (it will
+  not be needed later
+- User sends the CSR to the system where the certificate is desired
+- User gets caucase-rerequest to run on this CSR, producing a new private key
+  and a CSR similar to issued one, but signed with this new private key
+- From then on, caucase-updater can take over
+
+This way, no private key left their original system, and user could still
+freely customise certificate extensions.
+
+caucase-key-id
+++++++++++++++
+
+Utility displaying the identifier of given key, or the identifier of keys
+involved in given backup file.
+
+Allows identifying users which hold a private key candidate for restoring a
+caucased backup (see `Restoration procedure`_).
+
+caucased
+++++++++
+
+Reference caucase server daemon.
+
+This daemon provides access to both CAU and CAS services over both HTTP and
+HTTPS.
+
+It handles its own certificate issuance and renewal, so there is no need to use
+`caucase-updater`_ for this service.
+
+CORS
+----
+
+caucased implements CORS protection: when receiving a cross-origin request,
+it will respond with 401 Unauthorized, with the WWW-Authenticate header set to
+a custom scheme ("cors") with an "url" parameter containing an URI template
+with one variable field: "return" (more on it later).
+
+Upon receiving this response, the application is expected to render the URL
+template and redirect the user to resulting URL. There, the user will be
+informed of the cross-origin access attempt, and offered the choice to grant or
+deny access to given origin.
+
+Once their decision is made, their browser will receive a cookie remembering
+this decision, and they will be redirected to the URL received in the "return"
+field received upon above-described redirection.
+
+Then, the application should retry the original request, which will be
+accompanied by that cookie.
+
+Backups
+-------
+
+Loosing the CA private key prevents issuing any new certificate trusted by
+services which trusted the CA. Also, it prevents issuing any new CRL.
+Recovering from such total loss requires starting a new CA and rolling it out
+to all services which used the previous one. This is very time-costly.
+
+So backups are required.
+
+On the other hand, if someone gets their hand on the CA private key, they can
+issue certificates for themselves, allowing them to authenticate with services
+trusting the CA managed by caucase - including caucased itself if they issue a
+user certificate: they can then revoke existing certificates and cause a lot of
+damage.
+
+So backups cannot happen in clear text, they must be encrypted.
+
+But the danger of encrypted backups is that by definition they become worthless
+if they cannot be decrypted. So as many (trusted) entities as possible should
+be granted the ability to decrypt the backups.
+
+The solution proposed by caucased is to encrypt produced backups in a way which
+allows any of the caucase users to decrypt the archive.
+
+As these users are already entrusted with issuing certificates, this puts
+only a little more power in their hands than they already have. The little
+extra power they get is that by having unrestricted access to the CA private
+key they can issue certificates bypassing all caucase restrictions. The
+proposed parade is to only make the backups available to a limited subset of
+caucase users when there is an actual disaster, and otherwise keep it out of
+their reach. This mechanism is not handled by caucase.
+
+As there are few trusted users, caucase can keep their still-valid certificates
+in its database for the duration of their validity with minimal size cost.
+
+Backup procedure
+----------------
+
+Backups happen periodically as long as caucased is running. See
+`--backup-period` and `--backup-directory`.
+
+As discussed above, produced files should be kept out of reach of caucase
+users until a disaster happens.
+
+Restoration procedure
+---------------------
+
+See `caucased-manage --restore-backup`.
+
+To restore, one of the trusted users must voluntarily compromise their own
+private key, providing it to the administrator in charge of the restoration
+procedure. Restoration procedure will hence immediately revoke their
+certificate. They must also provide a CSR generated with a different private
+key, so that caucase can provide them with a new certificate, so they keep
+their access only via different credentials.
+
+- admin identifies the list of keys which can decipher a backup, and broadcasts
+  that list to key holders
+
+- key holders manifest themselves
+
+- admin picks a key holder, requests them to provide their existing private key
+  and to generate a new key and accompanying CSR
+
+- key holder provide requested items
+
+- admin initiates restoration with `--restore-backup` and provides key holder
+  with replacement certificate
+
+- admin starts caucased, service is back online.
+
+Backup file format
+------------------
+
+- 64bits: 'caucase\0' magic string
+
+- 32bits LE: header length
+
+- header: json-encoded header (see below)
+
+- encrypted byte stream (aka payload)
+
+Header schema (inspired from s/mime, but s/mime tools available do not
+support at least iterative production or iterative generation)::
+
+  {
+    "description": "Caucase backup header",
+    "required": ["algorithm", "key_list"],
+    "properties": {
+      "cipher": {
+        "description": "Symetric ciher used for payload",
+        "required": ["name"],
+        "properties": {
+          "name":
+            "enum": ["aes256_cbc_pkcs7_hmac_10M_sha256"],
+            "type": "string"
+          },
+          "parameter": {
+            "description": "Name-dependend clear cipher parameter (ex: IV)",
+            "type": "string"
+          }
+        }
+        "type": "object"
+      },
+      "key_list": {
+        "description": "Content key, encrypted with public keys",
+        "minItems": 1,
+        "items": {
+          "required": ["id", "cipher", "key"],
+          "properties": {
+            "id": {
+              "description": "Hex-encoded sha1 hash of the public key",
+              "type": "string"
+            },
+            "cipher": {
+              "description": "Asymetric cipher used for symetric key",
+              "required": ["name"],
+              "properties": {
+                "name": {
+                  "enum": ["rsa_oaep_sha1_mgf1_sha1"],
+                  "type": "string"
                 }
-                "type": "object"
               },
-              "key_list": {
-                "description": "Content key, encrypted with public keys",
-                "minItems": 1,
-                "items": {
-                  "required": ["id", "cipher", "key"],
-                  "properties": {
-                    "id": {
-                      "description": "Hex-encoded sha1 hash of the public key",
-                      "type": "string"
-                    },
-                    "cipher": {
-                      "description": "Asymetric cipher used for symetric key",
-                      "required": ["name"],
-                      "properties": {
-                        "name": {
-                          "enum": ["rsa_oaep_sha1_mgf1_sha1"],
-                          "type": "string"
-                        }
-                      },
-                      "type": "object"
-                    }
-                    "key": {
-                      "description": "Hex-encoded encrypted concatenation of signing and symetric encryption keys",
-                      "type": "string"
-                    }
-                  },
-                  "type": "object"
-                },
-                "type": "array"
-              }
-            },
-            "type": "object"
-          }
-        
-        0.9.8 (2020-06-29)
-        ==================
-        * Add support for python3.
-        * Add support for one-CA-cert-per-file layout. For services which do not support loading multiple CA certificates from a single file.
-        * Fix caucase.sh authenticated usage (was broken by 0.9.4 "Make caucased https CA certificate safer").
-        * Avoid busy-loop in caucase-updater when it thinks a renewal is due but caucased does not offer a newer version.
-        * Fix tests timeouts on slower machined. Anything faster than a Raspberry Pi 1 should now pass.
-        
-        0.9.7 (2020-06-04)
-        ==================
-        * Fix CRL renewal:
-          * teach caucased to renew CRLs ahead of their expirations.
-          * make caucase-updater check CRL expiration date.
-        * Grant extra permissions in license.
-        
-        0.9.6 (2019-05-27)
-        ==================
-        * Do not use a 128bits OID arc for caucase internal use, as it is not widely supported.
-        * Assorted CLI usability improvements.
-        
-        0.9.5 (2019-01-24)
-        ==================
-        * Add --version support.
-        * Logging is reworked to reduce verbosity (especially in tests).
-        * Fix caucased sometimes crashing when renewing its https certificate.
-        * Make caucased logs more apache-like.
-        * Make caucased responses more standard-compliant ("Allow" header in 405 response and "Date" header in all responses).
-        * Fix unintended dependency on system timezone.
-        
-        0.9.4 (2018-11-14)
-        ==================
-        * Improved documentation.
-        * Tentative web-friendliness (not used in real life yet, so practicality is still uncertain):
-          * Make caucased https CA certificate safer for adding in a trust store (ex: browser) by constraining the certificates it can sign.
-          * cookie-based CORS access control with crude UI.
-          * API is self-documenting using application/hal+json format.
-        * Tentative python3 friendliness, there may still be file IO encoding issues.
-        
-        0.9.3 (2018-09-21)
-        ==================
-        * Add support for listening to multiple specific addresses in caucased.
-        * shell implementation does not rely on an external file anymore.
-        * Do not start listening on https port before wrapping sockets with an ssl context
-        * Make caucase-updater usable by anonymous services (ex: they only need to connect to a caucase-certified service, without authenticating themselves using caucase)
-        * Use stricter file permissions for caucased sqlite database.
-        * Include caucase version in user agent header.
-        * Make caucased logging format more similar to apache's default.
-        * Fix caucased https certificate renewal. Fixes a crash which happens every 2 months.
-        * Make caucase-updater retry on network errors. Fixes crashes on transient network error.
-        
-        0.9.2 (2017-11-03)
-        ==================
-        * Add support for migrating an existing CA to caucase: import CA cert and CRLs.
-        * Require CRL signature checks (bumps cryptography module version requirements).
-        * Provide CRL distribution point extension in CA certificates.
-        * Play nicer with http:
-          * Catch more errors to provide nice status codes
-          * Add support for "Transfer-Encoding: chunked"
-          * Add support for "Expect: 100-continue"
-        * Produce TLS-compliant certificates (domain name must be in an alternative name extension, subject is not enough).
-        * Reduce speed requirements in tests.
-        * Add shell implementation of "caucase" command.
-        * Certificate renewal bypasses pending CSR limits.
-        * caucase-manage: new command for offline database maintenance.
-        
-        0.9.1 (2017-09-21)
-        ==================
-        * Documentation improvements
-        * Packaging improvements
-        
-        0.9.0 (2017-08-02)
-        ==================
-        * implement the "cau" half of "caucase"
-        * massive rework: removal of flask dependency, removal of HTML UI, rework of
-          the REST API, rework of the CLI tools, rework of the WGSI application,
-          incomatible redesign of the database.
-        
-        0.1.4 (2017-07-21)
-        ==================
-        * caucase web parameter 'auto-sign-csr-amount' can be used to set how many csr must be signed automatically.
-        
-        0.1.3 (2017-06-30)
-        ==================
-        
-        * add support for backup caucase database to cli
-        * serial is a random unique formatted hexadecimal number get from the csr_id
-        * allow to set custom subject (X509Name) when signing a certificate
-        * add new cliweb command which when required will download/update crl file from caucase web
-        
-        0.1.2 (2017-05-12)
-        ==================
-        * cliweb: renew now takes threshold option to check if renew is required and optional on-renew script to run after certificate renewal
-        
-        0.1.1 (2017-04-27)
-        ==================
-        
-         * initial implementation of certificate authority
-        
-        
-Keywords: certificate authority
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Topic :: Security :: Cryptography
-Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+              "type": "object"
+            }
+            "key": {
+              "description": "Hex-encoded encrypted concatenation of signing and symetric encryption keys",
+              "type": "string"
+            }
+          },
+          "type": "object"
+        },
+        "type": "array"
+      }
+    },
+    "type": "object"
+  }
```

### Comparing `caucase-0.9.8/versioneer.py` & `caucase-0.9.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `caucase-0.9.8/caucase.egg-info/SOURCES.txt` & `caucase-0.9.9/caucase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caucase-0.9.8/caucase.egg-info/PKG-INFO` & `caucase-0.9.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: caucase
-Version: 0.9.8
+Version: 0.9.9
 Summary: Certificate Authority.
 Home-page: https://lab.nexedi.com/nexedi/caucase
 Author: Vincent Pelletier
 Author-email: vincent@nexedi.com
 License: GPLv3+ with wide exception for FOSS
 Description: ..  Note to the editor: beware of implicit inline
             targets aliasing, keep global title different from all commands
@@ -121,14 +121,54 @@
         reasons: the list of revoked certificates also has a maximum life span. In
         caucase, the CRL is re-generated whenever it is requested and:
         
         - there is no previous CRL
         - previous CRL expired
         - any revocation happened since previous CRL was created
         
+        Here is an illustration of the certificate and CA certificate renewal process::
+        
+          Time from first caucased start:
+            +--------+--------+--------+--------+--------+--------+--------+-->
+          Certificate 1 validity:      |                 |                 |
+            |[cert 1v1]  [cert 1v3]  [cert 1v5]  [cert 1v7]  [cert 1v9]  [ce...
+            |      [cert 1v2]  [cert 1v4]  [cert 1v6]  [cert 1v8]  [cert 1vA]
+          Certificate 2 validity:      |                 |                 |
+            |    [cert 2v1]  [cert 2v3]| [cert 2v5]  [cert 2v7]  [cert 2v9]|
+            |          [cert 2v2]  [cert 2v4]  [cert 2v6]| [cert 2v8]  [cert...
+          CA certificates validity:    |                 |                 |
+            [ca v1                     |        ]        |                 |
+            |                 [ca v2   |                 |        ]        |
+            |                          |        [ca v3   |                 |...
+            |                          |                 |        [ca v4   |...
+          CRL validity for CA1:        |                 |                 |
+            [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ][ ][  ]        |                 |
+          CRL validity for CA2:        |                 |                 |
+            |                 [ ][ ][ ][ ][ ][ ][ ][ ][ ][ ][ ][  ]        |
+          CRL validity for CA3:        |                 |                 |
+            |                          |        [ ][ ][ ][ ][ ][ ][ ][ ][ ][...
+          CA renewal phase:            |                 |                 |
+            |none             |passive |active  |passive |active  |passive |...
+          Active CA:                   |                 |                 |
+            [ca v1                    ][ca v2           ][ca v3            |...
+          Trust anchor:                |                 |                 |
+            [ca v1                     |       ][ca v2   |       ][ca v3   |...
+        
+        Legend::
+        
+          +--------+ : One certificate validity period (default: 93 days)
+        
+        Points of interest:
+        
+        - this illustration assumes no revocation happen
+        - there usually are 2 simultaneously-valid CA certificates
+        - there usually are 2 simultaneously-valid CRLs overall, one per CA certificate
+        - the first ``cert 1`` signed by CA v2 is ``cert 1v6``
+        - the first ``cert 2`` signed by CA v2 is ``cert 1v5``
+        
         Commands
         ========
         
         Caucase provides several commands to work with certificates.
         
         caucase
         +++++++
@@ -359,14 +399,22 @@
                 },
                 "type": "array"
               }
             },
             "type": "object"
           }
         
+        0.9.9 (2021-03-02)
+        ==================
+        * Add AuthorityKeyIdentifier extension in CRLs.
+        * Accept user certificates signed by non-current CA.
+        * Name CA certificates after their AuthorityKeyIdentifier keyid extension instead of their serial.
+        * Produce one CRL per CA certificate, as some ssl-using services fail when there is no CRL signed by the same CA as the certificate being validated.
+        * Fix trust anchor distribution during CA renewal period: the correct trust anchor is the oldest still-valid CA.
+        
         0.9.8 (2020-06-29)
         ==================
         * Add support for python3.
         * Add support for one-CA-cert-per-file layout. For services which do not support loading multiple CA certificates from a single file.
         * Fix caucase.sh authenticated usage (was broken by 0.9.4 "Make caucased https CA certificate safer").
         * Avoid busy-loop in caucase-updater when it thinks a renewal is due but caucased does not offer a newer version.
         * Fix tests timeouts on slower machined. Anything faster than a Raspberry Pi 1 should now pass.
```

### Comparing `caucase-0.9.8/setup.py` & `caucase-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
   keywords='certificate authority',
   url='https://lab.nexedi.com/nexedi/caucase',
   license='GPLv3+ with wide exception for FOSS',
   packages=find_packages(),
   install_requires=[
     'cryptography>=2.2.1', # everything x509 except...
     'pyOpenSSL>=18.0.0', # ...certificate chain validation
-    'pem>=17.1.0', # Parse PEM files
+    'pem>=18.2.0', # Parse PEM files
     'PyJWT', # CORS token signature
   ],
   zip_safe=True,
   entry_points={
     'console_scripts': [
       'caucase = caucase.cli:main',
       'caucase-probe = caucase.cli:probe',
```

### Comparing `caucase-0.9.8/COPYING` & `caucase-0.9.9/COPYING`

 * *Files identical despite different names*

### Comparing `caucase-0.9.8/CHANGES.txt` & `caucase-0.9.9/CHANGES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+0.9.9 (2021-03-02)
+==================
+* Add AuthorityKeyIdentifier extension in CRLs.
+* Accept user certificates signed by non-current CA.
+* Name CA certificates after their AuthorityKeyIdentifier keyid extension instead of their serial.
+* Produce one CRL per CA certificate, as some ssl-using services fail when there is no CRL signed by the same CA as the certificate being validated.
+* Fix trust anchor distribution during CA renewal period: the correct trust anchor is the oldest still-valid CA.
+
 0.9.8 (2020-06-29)
 ==================
 * Add support for python3.
 * Add support for one-CA-cert-per-file layout. For services which do not support loading multiple CA certificates from a single file.
 * Fix caucase.sh authenticated usage (was broken by 0.9.4 "Make caucased https CA certificate safer").
 * Avoid busy-loop in caucase-updater when it thinks a renewal is due but caucased does not offer a newer version.
 * Fix tests timeouts on slower machined. Anything faster than a Raspberry Pi 1 should now pass.
```

### Comparing `caucase-0.9.8/caucase/version.py` & `caucase-0.9.9/caucase/version.py`

 * *Files identical despite different names*

### Comparing `caucase-0.9.8/caucase/cli.py` & `caucase-0.9.9/caucase/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -399,21 +399,35 @@
     'each containing a single PEM-encoded certificate. '
     'default: %(default)s',
   )
   parser.add_argument(
     '--crl',
     default='cas.crl.pem',
     metavar='CRL_PATH',
-    help='Services certificate revocation list location. default: %(default)s',
+    help='Services certificate revocation list location. '
+    'May be an existing directory or file, or non-existing. '
+    'If non-existing and given path has an extension, a file will be created, '
+    'otherwise a directory will be. '
+    'When it is a file, it may contain multiple PEM-encoded concatenated '
+    'CRLs. When it is a directory, it may contain multiple files, each '
+    'containing a single PEM-encoded CRL. '
+    'default: %(default)s',
   )
   parser.add_argument(
     '--user-crl',
     default='cau.crl.pem',
     metavar='CRL_PATH',
-    help='Users certificate revocation list location. default: %(default)s',
+    help='Users certificate revocation list location. '
+    'May be an existing directory or file, or non-existing. '
+    'If non-existing and given path has an extension, a file will be created, '
+    'otherwise a directory will be. '
+    'When it is a file, it may contain multiple PEM-encoded concatenated '
+    'CRLs. When it is a directory, it may contain multiple files, each '
+    'containing a single PEM-encoded CRL. '
+    'default: %(default)s',
   )
   parser.add_argument(
     '--threshold',
     default=31,
     type=float,
     help='The remaining certificate validity period, in days, under '
     'which a renew is desired. default: %(default)s',
@@ -810,14 +824,20 @@
     'Will be maintained up-to-date.',
   )
   parser.add_argument(
     '--crl',
     required=True,
     metavar='CRT_PATH',
     help='Path of your certificate revocation list for MODE. '
+    'May be an existing directory or file, or non-existing. '
+    'If non-existing and given path has an extension, a file will be created, '
+    'otherwise a directory will be. '
+    'When it is a file, it may contain multiple PEM-encoded concatenated '
+    'CRLs. When it is a directory, it may contain multiple files, each '
+    'containing a single PEM-encoded CRL. '
     'Will be maintained up-to-date.'
   )
   args = parser.parse_args(argv)
   try:
     cas_url = args.ca_url + '/cas'
     ca_url = {
       MODE_SERVICE: cas_url,
@@ -885,19 +905,19 @@
       ca_crt_list = [
         utils.load_ca_certificate(x)
         for x in utils.getCertList(args.ca)
       ]
       if RetryingCaucaseClient.updateCRLFile(ca_url, args.crl, ca_crt_list):
         print('Got new CRL')
         updated = True
-      with open(args.crl, 'rb') as crl_file:
+      for crl_pem in utils.getCRLList(args.crl):
         next_deadline = min(
           next_deadline,
           utils.load_crl(
-            crl_file.read(),
+            crl_pem,
             ca_crt_list,
           ).next_update - crl_threshold,
         )
       if args.crt:
         crt_pem, key_pem, key_path = utils.getKeyPair(args.crt, args.key)
         crt = utils.load_certificate(crt_pem, ca_crt_list, None)
         if crt.not_valid_after - threshold <= now:
```

### Comparing `caucase-0.9.8/caucase/http_wsgibase.py` & `caucase-0.9.9/caucase/http_wsgibase.py`

 * *Files identical despite different names*

### Comparing `caucase-0.9.8/caucase/test.py` & `caucase-0.9.9/caucase/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import HTMLParser
 import httplib
 from io import BytesIO, StringIO
 import ipaddress
 import json
 import os
 import random
+import re
 import shutil
 import socket
 import sqlite3
 import ssl
 import subprocess
 import sys
 import tarfile
@@ -51,18 +52,18 @@
 import threading
 import time
 import unittest
 from urllib import quote, urlencode
 import urlparse
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives import serialization, hashes
 from caucase import cli
 import caucase.ca
-from caucase.ca import Extension
+from caucase.ca import Extension, CertificateAuthority
 from caucase.client import CaucaseError, CaucaseClient
 from caucase.exceptions import CertificateVerificationError
 # Do not import caucase.http into this namespace: 2to3 will import standard
 # http module, which will then be masqued by caucase's http submodule.
 import caucase.http
 from caucase import utils
 from caucase import exceptions
@@ -157,21 +158,20 @@
 
   def makefile(self, mode, _):
     """
     Fake splitting the socket.
     """
     return self._rfile if 'r' in mode else self._wfile
 
-  # pylint: disable=unused-argument
   def sendall(self, data, flags=None): # pragma: no cover
     """
     Redirect sendall.
     """
+    _ = flags # Silence pylint
     self._wfile.write(data)
-  # pylint: enable=unused-argument
 
 class NoCloseFileProxy(object):
   """
   Intercept .close() calls, for example to allow reading StringIO content
   despite attempted closure.
   """
   def __init__(self, real_file):
@@ -332,31 +332,27 @@
     tests will need to interact with it.
     """
     global _clean_caucased_snapshot # pylint: disable=global-statement
     self._data_dir = data_dir = tempfile.mkdtemp(prefix='caucase_test_')
 
     self._client_dir = client_dir = os.path.join(data_dir, 'client')
     os.mkdir(client_dir)
-    # pylint: disable=bad-whitespace
     self._client_ca_crt      = os.path.join(client_dir, 'cas.crt.pem')
     self._client_ca_dir      = os.path.join(client_dir, 'cas_crt')
     self._client_user_ca_crt = os.path.join(client_dir, 'cau.crt.pem')
     self._client_crl         = os.path.join(client_dir, 'cas.crl.pem')
     self._client_user_crl    = os.path.join(client_dir, 'cau.crl.pem')
-    # pylint: enable=bad-whitespace
 
     self._server_event = threading.Event()
     self._server_dir = server_dir = os.path.join(data_dir, 'server')
     os.mkdir(server_dir)
-    # pylint: disable=bad-whitespace
     self._server_db          = os.path.join(server_dir, 'caucase.sqlite')
     self._server_key         = os.path.join(server_dir, 'server.key.pem')
     self._server_backup_path = os.path.join(server_dir, 'backup')
     self._server_cors_store  = os.path.join(server_dir, 'cors.key')
-    # pylint: enable=bad-whitespace
     # Using a BytesIO for caucased output here, because stdout/stderr do not
     # necessarily have a known encoding, for example when output is a pipe
     # (to a file, ...). caucased must deal with this.
     self.caucase_test_output = BytesIO()
     os.mkdir(self._server_backup_path)
 
     self._server_netloc = netloc = os.getenv(
@@ -443,25 +439,23 @@
             ca=True,
             path_length=0,
           ),
           critical=True, # "MUST mark the extension as critical"
         ),
         Extension(
           x509.KeyUsage(
-            # pylint: disable=bad-whitespace
             digital_signature =False,
             content_commitment=False,
             key_encipherment  =False,
             data_encipherment =False,
             key_agreement     =False,
             key_cert_sign     =True,
             crl_sign          =True,
             encipher_only     =False,
             decipher_only     =False,
-            # pylint: enable=bad-whitespace
           ),
           critical=True, # "SHOULD mark this extension critical"
         ),
       ] + list(extension_list),
     ).sign(
       private_key=private_key,
       algorithm=hashes.SHA256(),
@@ -495,41 +489,80 @@
       not_valid_before=not_before,
       not_valid_after=not_after,
       serial_number=x509.random_serial_number(),
       public_key=crt_key.public_key(),
       extensions=[
         Extension(
           x509.KeyUsage(
-            # pylint: disable=bad-whitespace
             digital_signature =True,
             content_commitment=False,
             key_encipherment  =True,
             data_encipherment =False,
             key_agreement     =False,
             key_cert_sign     =False,
             crl_sign          =False,
             encipher_only     =False,
             decipher_only     =False,
-            # pylint: enable=bad-whitespace
           ),
           critical=True,
         ),
       ] + list(extension_list),
     ).sign(
       private_key=ca_key,
       algorithm=hashes.SHA256(),
       backend=_cryptography_backend,
     )
 
-  def _getClientCRL(self):
-    with open(self._client_crl, 'rb') as crl_pem_file:
-      return x509.load_pem_x509_crl(
-        crl_pem_file.read(),
-        _cryptography_backend
-      )
+  @staticmethod
+  def _getCRL(
+    ca_key,
+    ca_crt,
+    crl_number=1,
+    revoked_serial_list=(),
+    last_update=None,
+    next_update=None,
+  ):
+    if last_update is None: # pragma: no cover
+      last_update = datetime.datetime.utcnow()
+    if next_update is None: # pragma: no cover
+      next_update = last_update + datetime.timedelta(5, 0)
+    return x509.CertificateRevocationListBuilder(
+      issuer_name=ca_crt.issuer,
+      last_update=last_update,
+      next_update=next_update,
+      extensions=[
+        Extension(
+          x509.CRLNumber(crl_number),
+          critical=False,
+        ),
+        Extension(
+          ca_crt.extensions.get_extension_for_class(
+            x509.AuthorityKeyIdentifier,
+          ).value,
+          critical=False,
+        ),
+      ],
+      revoked_certificates=[
+        x509.RevokedCertificateBuilder(
+          serial_number=x['serial'],
+          revocation_date=utils.timestamp2datetime(x['revocation_date']),
+        ).build(_cryptography_backend) # pragma: no cover
+        for x in revoked_serial_list
+      ],
+    ).sign(
+      private_key=ca_key,
+      algorithm=hashes.SHA256(),
+      backend=_cryptography_backend,
+    )
+
+  def _getClientCRLList(self):
+    return [
+      x509.load_pem_x509_crl(x, _cryptography_backend)
+      for x in utils.getCRLList(self._client_crl)
+    ]
 
   def _skipIfOpenSSLDoesNotSupportIPContraints(self):
     ca_key, ca_crt = self._getCAKeyPair(
       extension_list=[
         Extension(
           x509.NameConstraints(
             permitted_subtrees=[
@@ -546,15 +579,15 @@
       ca_crt=ca_crt,
     )
     try:
       # pylint: disable=protected-access
       utils._verifyCertificateChain(
         cert=crt,
         trusted_cert_list=[ca_crt],
-        crl=None,
+        crl_list=None,
       )
       # pylint: enable=protected-access
     except CertificateVerificationError: # pragma: no cover
       raise unittest.SkipTest('OpenSSL versoin does not support IP constraints')
 
   def _restoreServer(
     self,
@@ -1133,31 +1166,41 @@
       '--get-crt', csr_id, key_path,
     ).splitlines()
     self.assertRaises(TypeError, utils.getCert, key_path)
     self.assertEqual([
       csr_id + ' not found - maybe CSR was rejected ?'
     ], out)
 
+    # The server is able to regenerate the same CRL after a restart
+    reference_crl_list = self._getClientCRLList()
+    assert reference_crl_list # Sanity check
+    os.unlink(self._client_crl)
+    self._stopServer()
+    self._startServer()
+    self._runClient()
+    self.assertEqual(self._getClientCRLList(), reference_crl_list)
+
     # Renewing CRL
     self._stopServer()
-    reference_crl = self._getClientCRL()
+    reference_crl, = self._getClientCRLList()
     now = datetime.datetime.utcnow()
     # x509 certificates have second-level accuracy
     now = now.replace(microsecond=0)
     # Sanity check: pre-existing CRL creation should be strictly in the past
     self.assertLess(reference_crl.last_update, now)
-    # Store a dummy, already expired CRL, just to force a new one to be
-    # generated on next server start.
+    # Bump last_update in the past by a bit over half the CRL lifetime.
     SQLite3Storage(
       self._server_db,
       table_prefix='cas',
-    ).storeCertificateRevocationList('', 0)
+    ).storeCRLLastUpdate(
+      last_update=utils.datetime2timestamp(now - datetime.timedelta(16)),
+    )
     self._startServer()
     self._runClient()
-    new_crl = self._getClientCRL()
+    new_crl, = self._getClientCRLList()
     # May be equal due to lack of timestamp accuracy.
     self.assertLessEqual(now, new_crl.last_update)
 
   def testBadCSR(self):
     """
     Submitting an invalid CSR.
 
@@ -1167,14 +1210,52 @@
     try:
       client.createCertificateSigningRequest('Not actually a CSR')
     except CaucaseError as e:
       self.assertEqual(e.args[0], 400, e)
     else: # pragma: no cover
       raise AssertionError('Did not raise CaucaseError(400, ...)')
 
+  def testGetSingleCRL(self):
+    """
+    Retrieve an individual CRL.
+
+    Requires bypassing cli, as it only updates all CRLs.
+    """
+    self._runClient()
+    ca_crt_pem, = utils.getCertList(self._client_ca_crt)
+    ca_crt = utils.load_ca_certificate(ca_crt_pem)
+    ca_key_identifier = utils.getAuthorityKeyIdentifier(ca_crt)
+    user_key_path = self._createFirstUser()
+    service_key = self._createAndApproveCertificate(
+      user_key_path,
+      'service',
+    )
+    distribution_point, = utils.load_certificate(
+      utils.getCert(service_key),
+      [
+        utils.load_ca_certificate(x)
+        for x in utils.getCertList(self._client_ca_crt)
+      ],
+      None,
+    ).extensions.get_extension_for_class(
+      x509.CRLDistributionPoints,
+    ).value
+    crl_uri, = distribution_point.full_name
+    self.assertRegexpMatches(
+      crl_uri.value,
+      u'/cas/crl/%i$' % (ca_key_identifier, ),
+    )
+    reference_client_crl_pem, = utils.getCRLList(self._client_crl)
+    self.assertEqual(
+      CaucaseClient(
+        self._caucase_url + '/cas',
+      ).getCertificateRevocationList(ca_key_identifier),
+      reference_client_crl_pem,
+    )
+
   def testUpdateUser(self):
     """
     Verify that CAU certificate and revocation list are created when the
     (rarely needed) --update-user option is given.
     """
     self.assertFalse(os.path.exists(self._client_ca_crt))
     self.assertFalse(os.path.exists(self._client_crl))
@@ -1301,38 +1382,34 @@
         )
         self.assertEqual(
           extension.value,
           expected_value,
         )
         self.assertTrue(extension.critical)
     requested_key_usage = x509.KeyUsage(
-      # pylint: disable=bad-whitespace
       digital_signature =True,
       content_commitment=True,
       key_encipherment  =True,
       data_encipherment =True,
       key_agreement     =True,
       key_cert_sign     =True,
       crl_sign          =True,
       encipher_only     =True,
       decipher_only     =False,
-      # pylint: enable=bad-whitespace
     )
     expected_key_usage = x509.KeyUsage(
-      # pylint: disable=bad-whitespace
       digital_signature =True,
       content_commitment=True,
       key_encipherment  =True,
       data_encipherment =True,
       key_agreement     =True,
       key_cert_sign     =False,
       crl_sign          =False,
       encipher_only     =True,
       decipher_only     =False,
-      # pylint: enable=bad-whitespace
     )
     requested_extended_usage = x509.ExtendedKeyUsage([
       x509.oid.ExtendedKeyUsageOID.OCSP_SIGNING,
       x509.oid.ExtendedKeyUsageOID.CLIENT_AUTH,
     ])
     expected_extended_usage = x509.ExtendedKeyUsage([
       x509.oid.ExtendedKeyUsageOID.CLIENT_AUTH,
@@ -1470,41 +1547,84 @@
       '--get-crt', csr_id, key_path2,
     )
     checkCRT(key_path2)
 
   def testCACertRenewal(self):
     """
     Exercise CA certificate rollout procedure.
+    Also, check CaucaseClient.updateCAFile and CaucaseClient.updateCRLFile.
     """
+    def _checkUserAccess(user):
+      self._runClient(
+        '--user-key', user,
+        '--list-csr', # Whatever restricted operation
+      )
     user_key_path = self._createFirstUser()
-    cau_crt, = [
+    cau_ca_list = [
       utils.load_ca_certificate(x)
       for x in utils.getCertList(self._client_user_ca_crt)
     ]
+    cau_crt, = cau_ca_list
+    caucase_url = self._caucase_url + '/cau'
+    updateCAFile = lambda: CaucaseClient.updateCAFile(
+      url=caucase_url,
+      ca_crt_path=self._client_user_ca_crt,
+    )
+    updateCRLFile = lambda: CaucaseClient.updateCRLFile(
+      url=caucase_url,
+      crl_path=self._client_user_crl,
+      ca_list=cau_ca_list,
+    )
+    self._runClient('--update-user')
+    # CA & CRL were freshly updated, they should not need any update
+    self.assertFalse(updateCAFile())
+    self.assertFalse(updateCRLFile())
+    os.unlink(self._client_user_ca_crt)
+    os.unlink(self._client_user_crl)
+    # CA & CRL were emptied, they need update
+    self.assertTrue(updateCAFile())
+    self.assertTrue(updateCRLFile())
+    # And there is no need for further updates
+    self.assertFalse(updateCAFile())
+    self.assertFalse(updateCRLFile())
     self._stopServer()
-    # CA expires in 100 days: longer than one certificate life,
+    # CA expires in 100 days: longer than one certificate life (93 days),
     # but shorter than two. A new CA must be generated and distributed,
     # but not used for new signatures yet.
-    new_cau_crt_pem = self._setCACertificateRemainingLifeTime(
+    # As we will use this crt as trust anchor, we must make the client believe
+    # it knew it all along.
+    old_cau_pem = self._setCACertificateRemainingLifeTime(
       'user',
       cau_crt.serial_number,
       datetime.timedelta(100, 0),
     )
-    # As we will use this crt as trust anchor, we must make the client believe
-    # it knew it all along.
-    with open(self._client_user_ca_crt, 'wb') as client_user_ca_crt_file:
-      client_user_ca_crt_file.write(new_cau_crt_pem)
+    utils.saveCertList(self._client_user_ca_crt, [old_cau_pem])
     self._startServer(timeout=20)
-    new_user_key = self._createAndApproveCertificate(
+    # There is a new CA (and its CRL), update is needed.
+    self.assertTrue(updateCAFile())
+    # Load the new CA so CRL validation succeeds
+    cau_ca_list = [
+      utils.load_ca_certificate(x)
+      for x in utils.getCertList(self._client_user_ca_crt)
+    ]
+    self.assertTrue(updateCRLFile())
+    # And there is no need for further updates
+    self.assertFalse(updateCAFile())
+    self.assertFalse(updateCRLFile())
+    user1_key = self._createAndApproveCertificate(
+      user_key_path,
+      'user',
+    )
+    user2_key = self._createAndApproveCertificate(
       user_key_path,
       'user',
     )
     # Must not raise: we are signed with the "old" ca.
     utils.load_certificate(
-      utils.getCert(new_user_key),
+      utils.getCert(user2_key),
       [cau_crt],
       None,
     )
     # We must now know the new CA
     cau_crt_list = [
       utils.load_ca_certificate(x)
       for x in utils.getCertList(self._client_user_ca_crt)
@@ -1512,40 +1632,186 @@
     new_cau_crt, = [
       x for x in cau_crt_list
       if x.serial_number != cau_crt.serial_number
     ]
     self._stopServer()
     # New CA now exists for 100 days: longer than one certificate life.
     # It may (must) be used for new signatures.
-    self._setCACertificateRemainingLifeTime(
+    new_cau_pem = self._setCACertificateRemainingLifeTime(
       'user',
       new_cau_crt.serial_number,
       new_cau_crt.not_valid_after - new_cau_crt.not_valid_before -
       datetime.timedelta(100, 0),
     )
+    utils.saveCertList(
+      self._client_user_ca_crt,
+      [old_cau_pem, new_cau_pem],
+    )
     self._startServer()
+    # New certificate is signed by the new CA.
+    # Also, checks that user_key_path, which was signed by the old CA, is still
+    # accepted.
+    user3_key = self._createAndApproveCertificate(
+      user_key_path,
+      'user',
+    )
+    self.assertRaises(
+      exceptions.CertificateVerificationError,
+      utils.load_certificate,
+      utils.getCert(user3_key),
+      [cau_crt],
+      None,
+    )
+    utils.load_certificate(
+      utils.getCert(user3_key),
+      cau_crt_list,
+      None,
+    )
+    # Renewing a certificate gets one signed by the new CA
     self._runClient(
       '--mode', 'user',
       # 100 days is longer than certificate life, so it will be immediately
       # renewed.
       '--threshold', '100',
-      '--renew-crt', new_user_key, '',
+      '--renew-crt', user2_key, '',
     )
     self.assertRaises(
       exceptions.CertificateVerificationError,
       utils.load_certificate,
-      utils.getCert(new_user_key),
+      utils.getCert(user2_key),
       [cau_crt],
       None,
     )
     utils.load_certificate(
-      utils.getCert(new_user_key),
+      utils.getCert(user2_key),
       cau_crt_list,
       None,
     )
+    # This user certificate is accepted too.
+    _checkUserAccess(user2_key)
+    # Revoking a certificate signed by the old CA works.
+    _checkUserAccess(user1_key)
+    self._runClient(
+      '--mode', 'user',
+      '--revoke-crt', user1_key, '',
+    )
+    self.assertRaises(CaucaseError, _checkUserAccess, user1_key)
+    # Revoking a certificate signed by the new CA works.
+    _checkUserAccess(user2_key)
+    self._runClient(
+      '--mode', 'user',
+      '--revoke-crt', user2_key, '',
+      '--update-user',
+    )
+    # The CRLs maintained by the client have been refreshed to include the
+    # latest revocation, and all CRLs contain it.
+    expected_serial_set = {
+      utils.load_certificate(
+        utils.getCert(x),
+        cau_ca_list,
+        None,
+      ).serial_number
+      for x in (user1_key, user2_key)
+    }
+    # Test sanity check
+    assert len(expected_serial_set) == 2, expected_serial_set
+    crl_pem_a, crl_pem_b = utils.getCRLList(self._client_user_crl)
+    self.assertItemsEqual(
+      expected_serial_set,
+      [x.serial_number for x in utils.load_crl(crl_pem_a, cau_ca_list)],
+    )
+    self.assertItemsEqual(
+      expected_serial_set,
+      [x.serial_number for x in utils.load_crl(crl_pem_b, cau_ca_list)],
+    )
+    self.assertRaises(CaucaseError, _checkUserAccess, user2_key)
+    # A client without established trust anchor gets all still-valid CA
+    # certificates, not just the active one, so they can check still-valid
+    # certificates issued on the CA being retired.
+    os.unlink(self._client_user_ca_crt)
+    self._runClient('--mode', 'user')
+    self.assertItemsEqual(
+      [old_cau_pem, new_cau_pem],
+      utils.getCertList(self._client_user_ca_crt),
+    )
+    # The old CA is now fully expired
+    self._stopServer()
+    old_cau_pem = self._setCACertificateRemainingLifeTime(
+      'user',
+      cau_crt.serial_number,
+      datetime.timedelta(-1, 0),
+    )
+    utils.saveCertList(
+      self._client_user_ca_crt,
+      [old_cau_pem, new_cau_pem],
+    )
+    self._startServer()
+    # Non-renewed user certificate is rejected
+    self.assertRaises(CaucaseError, _checkUserAccess, user_key_path)
+    # Revoked and non-renewed user certificate is rejected
+    self.assertRaises(CaucaseError, _checkUserAccess, user1_key)
+    # Revoked and renewed user certificate is rejected
+    self.assertRaises(CaucaseError, _checkUserAccess, user2_key)
+    # Renewed and non-revoked user certificate is accepted
+    _checkUserAccess(user3_key)
+    # A client without established trust anchor only gets valid CA certs.
+    os.unlink(self._client_user_ca_crt)
+    self._runClient('--mode', 'user')
+    self.assertItemsEqual(
+      [new_cau_pem],
+      utils.getCertList(self._client_user_ca_crt),
+    )
+
+  def testCaucasedCRLRenewal(self):
+    """
+    Renew a CRL which has reached its renewal time.
+    """
+    self._stopServer()
+    cau = CertificateAuthority(
+      storage=SQLite3Storage(
+        db_path=self._server_db,
+        table_prefix='cas',
+      ),
+    )
+    # Fill the cache
+    reference_crl_pem_dict = cau.getCertificateRevocationListDict()
+    # Artificially expire all cached CRLs
+    # pylint: disable=protected-access
+    crl_pem_dict = cau._current_crl_dict
+    # pylint: enable=protected-access
+    for (
+      authority_key_identifier,
+      (crl_pem, _),
+    ) in crl_pem_dict.items():
+      crl_pem_dict[authority_key_identifier] = (
+        crl_pem,
+        datetime.datetime.utcnow() - datetime.timedelta(0, 1),
+      )
+    cau_ca_list = cau.getCACertificateList()
+    new_crl_pem_dict = cau.getCertificateRevocationListDict()
+    self.assertTrue(reference_crl_pem_dict)
+    self.assertItemsEqual(reference_crl_pem_dict, new_crl_pem_dict)
+    for (
+      authority_key_identifier,
+      reference_crl_pem,
+    ) in reference_crl_pem_dict.iteritems():
+      self.assertEqual(
+        utils.load_crl(
+          new_crl_pem_dict[authority_key_identifier],
+          cau_ca_list,
+        ).extensions.get_extension_for_class(
+          x509.CRLNumber,
+        ).value.crl_number,
+        utils.load_crl(
+          reference_crl_pem,
+          cau_ca_list,
+        ).extensions.get_extension_for_class(
+          x509.CRLNumber,
+        ).value.crl_number + 1,
+      )
 
   def testCaucasedCertRenewal(self):
     """
     Exercise caucased internal certificate renewal procedure.
     """
     user_key_path = self._createFirstUser()
     self._stopServer()
@@ -1572,15 +1838,15 @@
     ).cursor().execute(
       'SELECT key FROM http_casca',
     ).fetchall()
 
     self._stopServer()
     crt_pem, key_pem, ca_crt_pem = utils.getCertKeyAndCACert(
       self._server_key,
-      crl=None,
+      crl_list=None,
     )
     with open(self._server_key, 'wb') as server_key_file:
       server_key_file.write(key_pem)
       server_key_file.write(utils.dump_certificate(
         self._setCertificateRemainingLifeTime(
           key=utils.load_privatekey(utils.toBytes(http_cas_key)),
           crt=utils.load_certificate(
@@ -1637,46 +1903,49 @@
     """
     Test wsgi class reaction to malformed requests.
 
     For tests which are not accessible through the client module (as it tries
     to only produce valid requests).
     """
     self._runClient('--mode', 'user', '--update-user')
-    cau_list = [
+    cau_crt, = [
       utils.load_ca_certificate(x)
       for x in utils.getCertList(self._client_user_ca_crt)
     ]
-    with open(self._client_user_crl, 'rb') as client_user_crl_file:
-      cau_crl = client_user_crl_file.read()
+    cau_crl, = utils.getCRLList(self._client_user_crl)
+    ca_key_id = utils.getAuthorityKeyIdentifier(
+      utils.load_crl(cau_crl, [cau_crt]),
+    )
+    cau_crl_dict = {ca_key_id: cau_crl}
     class DummyCAU(object):
       """
       Mock CAU.
       """
       digest_list = ['sha256']
 
       @staticmethod
       def getCACertificateList():
         """
         Return cau ca list.
         """
-        return cau_list
+        return [cau_crt]
 
       @staticmethod
       def getCACertificate():
         """
         Return a dummy string as CA certificate
         """
         return b'notreallyPEM'
 
       @staticmethod
-      def getCertificateRevocationList():
+      def getCertificateRevocationListDict():
         """
         Return cau crl.
         """
-        return cau_crl
+        return cau_crl_dict
 
       @staticmethod
       def appendCertificateSigningRequest(_):
         """
         Raise to exercise the "unexpected exception" code path in WSGI.
         """
         raise ValueError('Some generic exception')
@@ -1797,16 +2066,27 @@
           u"method": u"DELETE",
           u"templated": True,
           u"title": u"Reject a pending certificate signing request.",
         },
       },
       u"_links": {
         u"getCertificateRevocationList": {
+          u"href": HATEOAS_HTTP_PREFIX + u"/cau/crl/{+authority_key_id}",
+          u"templated": True,
+          u"title": (
+            u"Retrieve latest certificate revocation list for given "
+            u"decimal representation of the authority identifier."
+          ),
+        },
+        u"getCertificateRevocationListList": {
           u"href": HATEOAS_HTTP_PREFIX + u"/cau/crl",
-          u"title": u"Retrieve latest certificate revocation list.",
+          u"title": (
+            u"Retrieve latest certificate revocation list for all valid "
+            u"authorities."
+          ),
         },
         u"getCACertificate": {
           u"href": HATEOAS_HTTP_PREFIX + u"/cau/crt/ca.crt.pem",
           u"title": u"Retrieve current CA certificate.",
         },
         u"self": {
           u"href": HATEOAS_HTTP_PREFIX + u"/cau",
@@ -1844,17 +2124,42 @@
     })[0], 404)
     self.assertEqual(request({
       'PATH_INFO': '/cau/does_not_exist',
       'REQUEST_METHOD': 'GET',
     })[0], 404)
 
     self.assertEqual(request({
+      'PATH_INFO': '/cau/crl/abc',
+      'REQUEST_METHOD': 'GET',
+    })[0], 404)
+    self.assertEqual(request({
       'PATH_INFO': '/cau/crl/123',
       'REQUEST_METHOD': 'GET',
     })[0], 404)
+    self.assertEqual(request({
+      'PATH_INFO': '/cau/crl/12/3',
+      'REQUEST_METHOD': 'GET',
+    })[0], 404)
+    status, _, header_dict, body = request({
+      'PATH_INFO': '/cau/crl/%i' % (ca_key_id, ),
+      'REQUEST_METHOD': 'GET',
+    })
+    self.assertEqual(status, 200)
+    self.assertEqual(header_dict.get('Content-Type'), 'application/pkix-crl')
+    self.assertEqual(body, cau_crl)
+    status, _, header_dict, body = request({
+      'PATH_INFO': '/cau/crl',
+      'REQUEST_METHOD': 'GET',
+    })
+    self.assertEqual(status, 200)
+    self.assertEqual(header_dict.get('Content-Type'), 'application/pkix-crl')
+    self.assertEqual(body, '\n'.join(
+      x.decode('ascii')
+      for x in cau_crl_dict.itervalues()
+    ).encode('utf-8'))
 
     min_date = int(time.time())
     status, _, header_dict, _ = request({
       'PATH_INFO': '/cau/crl',
       'REQUEST_METHOD': 'PUT',
     })
     max_date = int(time.time())
@@ -1936,14 +2241,20 @@
       'CONTENT_LENGTH': str(wsgi.MAX_BODY_LENGTH + 1),
       'wsgi.input': BytesIO(),
     })[0], 413)
     self.assertEqual(request({
       'PATH_INFO': '/cau/crt/renew',
       'REQUEST_METHOD': 'PUT',
       'CONTENT_TYPE': 'application/json',
+      'wsgi.input': BytesIO(b'"' + b'a' * (wsgi.MAX_BODY_LENGTH + 1)),
+    })[0], 413)
+    self.assertEqual(request({
+      'PATH_INFO': '/cau/crt/renew',
+      'REQUEST_METHOD': 'PUT',
+      'CONTENT_TYPE': 'application/json',
       'wsgi.input': BytesIO(b'{'),
     })[0], 400)
     self.assertEqual(request({
       'PATH_INFO': '/cau/crt/revoke',
       'REQUEST_METHOD': 'PUT',
       'CONTENT_TYPE': 'application/json',
       'wsgi.input': BytesIO(b'{"digest": null}'),
@@ -2370,36 +2681,40 @@
         raise
 
     after_restore = list(SQLite3Storage(
       self._server_db,
       table_prefix='cau',
     ).dumpIterator())
 
-    CRL_INSERT = b'INSERT INTO "caucrl" '
+    CRL_NUMBER_INSERT = b'INSERT INTO "caucounter" VALUES(\'crl_number\','
     CRT_INSERT = b'INSERT INTO "caucrt" '
     REV_INSERT = b'INSERT INTO "caurevoked" '
     def filterBackup(backup, expect_rev):
       """
       Remove all lines which are know to differ between original batabase and
       post-restoration database, so the rest (which must be the majority of the
       database) can be tested to be equal.
       """
       rev_found = not expect_rev
       new_backup = []
       crt_list = []
+      crl_number_found = False
       for row in backup:
-        if row.startswith(CRL_INSERT):
+        if row.startswith(CRL_NUMBER_INSERT):
+          assert not crl_number_found
+          crl_number_found = True
           continue
         if row.startswith(CRT_INSERT):
           crt_list.append(row)
           continue
         if row.startswith(REV_INSERT): # pragma: no cover
           assert not rev_found, 'Unexpected revocation found'
           continue
         new_backup.append(row)
+      assert crl_number_found
       return new_backup, crt_list
 
     before_backup, before_crt_list = filterBackup(
       before_backup,
       False,
     )
     after_restore, after_crt_list = filterBackup(
@@ -2534,15 +2849,15 @@
       'service',
     )
     # ...and revoke it
     # Note: Fetches CRL right after revoking certificate
     self._runClient(
       '--revoke-crt', service_key, service_key,
     )
-    self._runClient()
+    crl, = self._getClientCRLList()
     getBytePass_orig = caucase.http.getBytePass
     try:
       caucase.http.getBytePass = lambda x: b'test'
       self.assertFalse(os.path.exists(exported_ca), exported_ca)
       caucase.http.manage(
         argv=(
           '--db', self._server_db,
@@ -2563,14 +2878,20 @@
         ),
         stdout=stdout,
       )
       self.assertTrue(os.path.exists(server_db2), server_db2)
       self.assertEqual(
         [
           'Imported 1 CA certificates',
+          'Set CRL number to %i and last update to %s' % (
+            crl.extensions.get_extension_for_class(
+              x509.CRLNumber,
+            ).value.crl_number,
+            crl.last_update.isoformat(' '),
+          ),
           'Revoked 1 certificates (1 were already revoked)',
         ],
         stdout.getvalue().decode('ascii').splitlines(),
       )
     finally:
       caucase.http.getBytePass = getBytePass_orig
 
@@ -2875,15 +3196,16 @@
       updater_event.set()
       # Wait for it to call "until()" again
       until_updater.wait()
       # It must have retrieved the certificate now.
       self.assertTrue(os.path.exists(re_crt_path))
 
       # Next wakeup should be 7 days before CRL expiration (default delay)
-      crl_renewal = self._getClientCRL().next_update - datetime.timedelta(7, 0)
+      crl, = self._getClientCRLList()
+      crl_renewal = crl.next_update - datetime.timedelta(7, 0)
       # Give +/-5 seconds of leeway.
       crl_tolerance = datetime.timedelta(0, 5)
       self.assertGreater(
         until_updater.deadline, crl_renewal - crl_tolerance,
       )
       self.assertLess(
         until_updater.deadline, crl_renewal + crl_tolerance,
@@ -2902,60 +3224,89 @@
       ca_crt = utils.load_ca_certificate(ca_file.read())
     self.assertEqual(client_ca_crt, ca_crt)
 
   def testCAFilesystemStorage(self):
     """
     Test CA certificate storage in filesystem.
     """
+    def _listCAFiles():
+      return [
+        x
+        for x in os.listdir(self._client_ca_dir)
+        if x.endswith('.ca.pem')
+      ]
     # Loading from non-existsent files
     self.assertFalse(os.path.exists(self._client_ca_dir))
     self.assertEqual(utils.getCertList(self._client_ca_dir), [])
     self.assertFalse(os.path.exists(self._client_ca_crt))
     self.assertEqual(utils.getCertList(self._client_ca_crt), [])
     # Creation
-    _, crt0 = self._getCAKeyPair()
+    key0, crt0 = self._getCAKeyPair()
     crt0_pem = utils.dump_certificate(crt0)
-    _, crt1 = self._getCAKeyPair()
+    key1, crt1 = self._getCAKeyPair()
     crt1_pem = utils.dump_certificate(crt1)
+    crl0_pem = self._getCRL(key0, crt0).public_bytes(
+      serialization.Encoding.PEM,
+    )
+    crl1_pem = self._getCRL(key1, crt1).public_bytes(
+      serialization.Encoding.PEM,
+    )
+    # Store CRLs in the same directory, to detect cross-talk
+    utils.saveCRLList(self._client_ca_dir, [crl0_pem, crl1_pem])
+    # Sanity check
+    self.assertItemsEqual(
+      utils.getCRLList(self._client_ca_dir),
+      [crl0_pem, crl1_pem],
+    )
+    # On with the test for the CA side
     utils.saveCertList(self._client_ca_dir, [crt0_pem])
     self.assertTrue(os.path.exists(self._client_ca_dir))
     self.assertTrue(os.path.isdir(self._client_ca_dir))
-    crt0_name, = os.listdir(self._client_ca_dir)
+    crt0_name, = _listCAFiles()
     self.assertItemsEqual(utils.getCertList(self._client_ca_dir), [crt0_pem])
     utils.saveCertList(self._client_ca_crt, [crt0_pem])
     self.assertTrue(os.path.exists(self._client_ca_crt))
     self.assertTrue(os.path.isfile(self._client_ca_crt))
     self.assertItemsEqual(utils.getCertList(self._client_ca_crt), [crt0_pem])
-    # Invalid file gets deleted
-    dummy_file_path = os.path.join(self._client_ca_dir, 'not_a_pem')
-    with open(dummy_file_path, 'wb') as dummy:
+    # Invalid file gets deleted only if it has expected extension (.ca.pem)
+    kept_file_path = os.path.join(self._client_ca_dir, 'not_a_ca.pem')
+    deleted_file_path = os.path.join(self._client_ca_dir, 'foo.ca.pem')
+    with open(kept_file_path, 'wb'), open(deleted_file_path, 'wb'):
       pass
-    self.assertTrue(os.path.exists(dummy_file_path))
+    self.assertTrue(os.path.exists(kept_file_path))
+    self.assertTrue(os.path.exists(deleted_file_path))
     utils.saveCertList(self._client_ca_dir, [crt0_pem])
-    self.assertFalse(os.path.exists(dummy_file_path))
+    self.assertTrue(os.path.exists(kept_file_path))
+    self.assertFalse(os.path.exists(deleted_file_path))
+    os.unlink(kept_file_path)
     # Storing and loading multiple certificates
     utils.saveCertList(self._client_ca_dir, [crt0_pem, crt1_pem])
-    crta, crtb = os.listdir(self._client_ca_dir)
+    crta, crtb = _listCAFiles()
     crt1_name, = [x for x in (crta, crtb) if x != crt0_name]
     self.assertItemsEqual(
       utils.getCertList(self._client_ca_dir),
       [crt0_pem, crt1_pem],
     )
     utils.saveCertList(self._client_ca_crt, [crt0_pem, crt1_pem])
     self.assertItemsEqual(
       utils.getCertList(self._client_ca_crt),
       [crt0_pem, crt1_pem],
     )
     # Removing a previously-stored certificate
     utils.saveCertList(self._client_ca_dir, [crt1_pem])
-    crta, = os.listdir(self._client_ca_dir)
+    crta, = _listCAFiles()
     self.assertEqual(crta, crt1_name)
     self.assertItemsEqual(utils.getCertList(self._client_ca_dir), [crt1_pem])
     utils.saveCertList(self._client_ca_crt, [crt1_pem])
     self.assertItemsEqual(utils.getCertList(self._client_ca_crt), [crt1_pem])
+    # The CRLs are still present
+    self.assertItemsEqual(
+      utils.getCRLList(self._client_ca_dir),
+      [crl0_pem, crl1_pem],
+    )
 
   def testHttpSSLRenewal(self):
     """
     Test that caucased https certificate renewal is functional.
     """
     # http server is started without backups by default, so deadline is ssl
     # renewal deadline. So fake expiration and verify the certificate presented
@@ -3007,15 +3358,18 @@
         for x in utils.getCertList(self._client_ca_crt)
       ],
       None,
     ).extensions.get_extension_for_class(
       x509.CRLDistributionPoints,
     ).value
     uri, = distribution_point.full_name
-    self.assertEqual(uri.value, self._caucase_url + u'/cas/crl')
+    self.assertRegexpMatches(
+      uri.value,
+      u'^' + re.escape(self._caucase_url) + u'/cas/crl/[0-9]+$',
+    )
 
   def testHttpNetlocIPv4(self):
     """
     Test that it is possible to use a literal IPv4 as netloc.
     """
     self._testHttpCustomNetLoc(netloc='127.0.0.1')
 
@@ -3123,28 +3477,222 @@
       user_certificate_policies.value,
       x509.CertificatePolicies([
         pre_monkey_CAUCASE_POLICY_INFORMATION_AUTO_SIGNED,
       ]),
     )
     self.assertFalse(user_certificate_policies.critical)
 
+  def test_databaseUpgradeFrom_0_9_8_with_revoked(self):
+    """
+    Test database upgrade from 0.9.8 with some revoked certificates.
+    """
+    self._test_databaseUpgradeFrom_0_9_8(has_revoked=True)
+
+  def test_databaseUpgradeFrom_0_9_8_no_revoked(self):
+    """
+    Test database upgrade from 0.9.8 without any revoked certificate.
+    """
+    self._test_databaseUpgradeFrom_0_9_8(has_revoked=False)
+
+  def _test_databaseUpgradeFrom_0_9_8(self, has_revoked):
+    """
+    Up to version 0.9.8, caucase managed (and issued) a single CRL, which
+    prevent proper CA renewal. Test that it is possible to upgrade from that
+    version.
+    """
+    self._stopServer()
+    os.unlink(self._server_db)
+    os.close(os.open(
+      self._server_db,
+      os.O_CREAT | os.O_RDONLY,
+      0o600,
+    ))
+    db = sqlite3.connect(self._server_db)
+    with db:
+      c = db.cursor()
+      c.executescript('''
+        CREATE TABLE IF NOT EXISTS casca (
+          expiration_date INTEGER,
+          key TEXT,
+          crt TEXT
+        );
+        CREATE TABLE IF NOT EXISTS cascrt (
+          id INTEGER PRIMARY KEY,
+          key_id TEXT,
+          expiration_date INTEGER,
+          csr TEXT,
+          crt TEXT
+        );
+        CREATE TABLE IF NOT EXISTS casrevoked (
+          serial TEXT PRIMARY KEY,
+          revocation_date INTEGER,
+          expiration_date INTEGER
+        );
+        CREATE TABLE IF NOT EXISTS cascrl (
+          expiration_date INTEGER,
+          crl TEXT
+        );
+        CREATE TABLE IF NOT EXISTS cascounter (
+          name TEXT PRIMARY KEY,
+          value INTEGER
+        );
+        CREATE TABLE IF NOT EXISTS casconfig_once (
+          name TEXT PRIMARY KEY,
+          value TEXT
+        );
+      ''')
+      now = datetime.datetime.utcnow().replace(microsecond=0)
+      ca_lifetime = datetime.timedelta(390)
+      old_ca_expiration_date = now + datetime.timedelta(100)
+      old_ca_key, old_ca_crt = self._getCAKeyPair(
+        not_before=old_ca_expiration_date - ca_lifetime,
+        not_after=old_ca_expiration_date,
+      )
+      ca_expiration_date = now + datetime.timedelta(300)
+      ca_key, ca_crt = self._getCAKeyPair(
+        not_before=ca_expiration_date - ca_lifetime,
+        not_after=ca_expiration_date,
+      )
+      c.execute(
+        'INSERT INTO casca (expiration_date, key, crt) VALUES (?, ?, ?)',
+        (
+          utils.datetime2timestamp(old_ca_expiration_date),
+          utils.dump_privatekey(old_ca_key),
+          utils.dump_certificate(old_ca_crt),
+        ),
+      )
+      c.execute(
+        'INSERT INTO casca (expiration_date, key, crt) VALUES (?, ?, ?)',
+        (
+          utils.datetime2timestamp(ca_expiration_date),
+          utils.dump_privatekey(ca_key),
+          utils.dump_certificate(ca_crt),
+        ),
+      )
+      crl_number = 5
+      c.execute(
+        'INSERT INTO cascounter (name, value) VALUES (?, ?)',
+        (
+          'crl_number',
+          crl_number,
+        ),
+      )
+      if has_revoked:
+        revoked_list = [
+          (
+            4321,
+            now - datetime.timedelta(11),
+          ),
+          (
+            1234,
+            now - datetime.timedelta(10),
+          ),
+        ]
+        for (serial, revocation_date) in revoked_list:
+          c.execute(
+            'INSERT INTO casrevoked '
+            '(serial, revocation_date, expiration_date) '
+            'VALUES (?, ?, ?)',
+            (
+              serial,
+              utils.datetime2timestamp(revocation_date),
+              utils.datetime2timestamp(now + datetime.timedelta(5)),
+            ),
+          )
+      else:
+        revoked_list = []
+      crl_pem = x509.CertificateRevocationListBuilder(
+        issuer_name=ca_crt.issuer,
+        last_update=now,
+        next_update=now + datetime.timedelta(31),
+        extensions=[
+          Extension(
+            x509.CRLNumber(crl_number),
+            critical=False,
+          ),
+          # Note: AuthorityKeyIdentifier is absent, consistently with
+          # caucase version 0.9.8 .
+        ],
+        revoked_certificates=[
+          x509.RevokedCertificateBuilder(
+            serial_number=serial,
+            revocation_date=revocation_date,
+          ).build(_cryptography_backend)
+          for (serial, revocation_date) in revoked_list
+        ],
+      ).sign(
+        private_key=ca_key,
+        algorithm=hashes.SHA256(),
+        backend=_cryptography_backend,
+      ).public_bytes(serialization.Encoding.PEM)
+      with open(self._client_crl, 'wb') as crl_file:
+        # Excercise the client's ability to update the CRL from a file which
+        # lacks AuthorityKeyIdentifier extension.
+        crl_file.write(crl_pem)
+      # Sanity check
+      self.assertRaises(
+        x509.extensions.ExtensionNotFound,
+        utils.getAuthorityKeyIdentifier,
+        utils.load_crl(crl_pem, [ca_crt]),
+      )
+      c.execute(
+        'INSERT INTO cascrl (expiration_date, crl) VALUES (?, ?)',
+        (
+          utils.datetime2timestamp(now + datetime.timedelta(15, 0)),
+          crl_pem,
+        ),
+      )
+    db.close()
+    ca_crt_list = [old_ca_crt, ca_crt]
+    self._startServer()
+    self._runClient()
+    self.assertItemsEqual(
+      [
+        utils.load_ca_certificate(x)
+        for x in utils.getCertList(self._client_ca_crt)
+      ],
+      ca_crt_list,
+    )
+    crl_pem_list = utils.getCRLList(self._client_crl)
+    self.assertEqual(len(crl_pem_list), 2)
+    for crl_pem in crl_pem_list:
+      crl = utils.load_crl(crl_pem, ca_crt_list)
+      # "now" is the (rough) CRL generation time, current time should be later
+      # (by at least one second) although this is not being tested, and the
+      # re-generated CRL time should be "now" to justify the crl_number being
+      # unchanged.
+      self.assertEqual(crl.last_update, now)
+      self.assertEqual(
+        crl.extensions.get_extension_for_class(
+          x509.CRLNumber,
+        ).value.crl_number,
+        crl_number,
+      )
+      self.assertItemsEqual(
+        revoked_list,
+        [
+          (x.serial_number, x.revocation_date)
+          for x in crl
+        ],
+      )
+
 for property_id, property_value in CaucaseTest.__dict__.iteritems():
   if property_id.startswith('test') and callable(property_value):
     setattr(CaucaseTest, property_id, print_buffer_on_error(property_value))
 
 # pylint: disable=no-member
 if getattr(CaucaseTest, 'assertItemsEqual', None) is None: # pragma: no cover
   # Because python3 decided it should be named differently, and 2to3 cannot
   # pick it up, and this code must remain python2-compatible... Yay !
   CaucaseTest.assertItemsEqual = CaucaseTest.assertCountEqual
 # pylint: enable=no-member
 
-_caucase_root = os.path.normpath(
-  os.path.join(os.path.dirname(__file__), os.path.pardir),
-)
+_caucase_root = os.path.dirname(__file__)
+while not os.path.exists(os.path.join(_caucase_root, '.git')):
+  _caucase_root = os.path.normpath(os.path.join(_caucase_root, os.path.pardir))
 _caucase_sh_path = find_executable(
   'caucase.sh',
   path=os.path.join(
     _caucase_root, 'shell',
   ) + os.path.pathsep + os.getenv('PATH', ''),
 )
 def _runCaucaseSh(*args):
@@ -3154,15 +3702,14 @@
       command,
       stdin=devnull,
       stdout=subprocess.PIPE,
       stderr=subprocess.STDOUT,
       close_fds=True,
       env={
         'CAUCASE_PYTHON': sys.executable,
-        'PYTHONPATH': _caucase_root,
       },
     )
     stdout, _ = process.communicate()
     status = process.wait()
   return status, command, stdout
 @unittest.skipIf(
   _caucase_sh_path is None or _runCaucaseSh('--help')[0],
@@ -3180,15 +3727,15 @@
       'Process %r exited with status %s, dumping output:\n%s' % (
         command,
         status,
         stdout.decode('ascii'),
       )
     )
 
-  def test_test(self):
+  def test_shell_test(self):
     """
     Run caucase.sh's embedded testsuite.
     """
     self._run('--test', os.getenv(
       'CAUCASE_NETLOC',
       'localhost:8000',
     ))
```

### Comparing `caucase-0.9.8/caucase/ca.py` & `caucase-0.9.9/caucase/ca.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,24 +44,22 @@
 __all__ = ('CertificateAuthority', 'UserCertificateAuthority', 'Extension')
 
 _cryptography_backend = default_backend()
 _AUTO_SIGNED_NO = 0
 _AUTO_SIGNED_YES = 1
 _AUTO_SIGNED_PASSTHROUGH = 2
 _SUBJECT_OID_DICT = {
-  # pylint: disable=bad-whitespace
   'C' : x509.oid.NameOID.COUNTRY_NAME,
   'O' : x509.oid.NameOID.ORGANIZATION_NAME,
   'OU': x509.oid.NameOID.ORGANIZATIONAL_UNIT_NAME,
   'ST': x509.oid.NameOID.STATE_OR_PROVINCE_NAME,
   'CN': x509.oid.NameOID.COMMON_NAME,
   'L' : x509.oid.NameOID.LOCALITY_NAME,
   'SN': x509.oid.NameOID.SURNAME,
   'GN': x509.oid.NameOID.GIVEN_NAME,
-  # pylint: enable=bad-whitespace
 }
 _BACKUP_MAGIC = b'caucase\0'
 _CONFIG_NAME_AUTO_SIGN_CSR_AMOUNT = 'auto_sign_csr_amount'
 
 DEFAULT_BACKUP_SYMETRIC_CIPHER = 'aes256_cbc_pkcs7_hmac_10M_sha256'
 
 def Extension(value, critical):
@@ -149,14 +147,15 @@
       (a message is printed when retrieving the certificate)
       This mark is propagated during certificate renewal.
 
     lock_auto_sign_csr_amount (bool)
       When given with a true value, auto_sign_csr_amount is stored and the
       value given on later instanciation will be ignored.
     """
+    self._current_crl_dict = {}
     self._storage = storage
     self._ca_renewal_lock = threading.Lock()
     if lock_auto_sign_csr_amount:
       storage.setConfigOnce(
         _CONFIG_NAME_AUTO_SIGN_CSR_AMOUNT,
         auto_sign_csr_amount,
       )
@@ -196,25 +195,48 @@
   def digest_list(self):
     """
     Read-only access to digest_list ctor parameter.
     """
     return list(self._digest_list)
 
   def _loadCAKeyPairList(self):
+    digest = self._digest_list[0]
     ca_key_pair_list = []
+    ca_certificate_chain = []
+    previous_crt_pem = None
+    previous_key = None
     for pem_key_pair in self._storage.getCAKeyPairList():
       utils.validateCertAndKey(
         pem_key_pair['crt_pem'],
         pem_key_pair['key_pem'],
       )
+      crt_pem = pem_key_pair['crt_pem']
+      crt = utils.load_ca_certificate(pem_key_pair['crt_pem'])
+      key = utils.load_privatekey(pem_key_pair['key_pem'])
       ca_key_pair_list.append({
-        'crt': utils.load_ca_certificate(pem_key_pair['crt_pem']),
-        'key': utils.load_privatekey(pem_key_pair['key_pem']),
+        'crt': crt,
+        'key': key,
+        'authority_key_identifier': utils.getAuthorityKeyIdentifier(crt),
       })
+      if previous_key is not None:
+        ca_certificate_chain.append(utils.wrap(
+          {
+            'old_pem': utils.toUnicode(previous_crt_pem),
+            'new_pem': utils.toUnicode(crt_pem),
+          },
+          previous_key,
+          digest,
+        ))
+      previous_crt_pem = crt_pem
+      previous_key = key
+    self._current_crl_dict.clear()
     self._ca_key_pairs_list = ca_key_pair_list
+    self._ca_certificate_chain = tuple(
+      ca_certificate_chain
+    )
 
   def getCertificateSigningRequest(self, csr_id):
     """
     Retrieve a PEM-encoded certificate signing request.
 
     csr_id (int)
       As returned when the CSR was stored.
@@ -319,29 +341,33 @@
         Extension(
           x509.SubjectKeyIdentifier.from_public_key(
             public_key,
           ),
           critical=False, # "MUST mark this extension as non-critical"
         ),
         Extension(
-          x509.AuthorityKeyIdentifier.from_issuer_subject_key_identifier(
-            ca_crt.extensions.get_extension_for_class(
-              x509.SubjectKeyIdentifier,
-            ).value,
-          ),
+          ca_crt.extensions.get_extension_for_class(
+            x509.AuthorityKeyIdentifier,
+          ).value,
           critical=False, # "MUST mark this extension as non-critical"
         ),
       ],
     )
     if self._crl_base_url:
       builder = builder.add_extension(
         x509.CRLDistributionPoints([
           x509.DistributionPoint(
             full_name=[
-              x509.UniformResourceIdentifier(self._crl_base_url),
+              x509.UniformResourceIdentifier(
+                self._crl_base_url + (
+                  '/%i' % (
+                    utils.getAuthorityKeyIdentifier(ca_crt),
+                  )
+                ),
+              ),
             ],
             relative_name=None,
             crl_issuer=None,
             reasons=None,
           ),
         ]),
         critical=False, # "SHOULD be non-critical"
@@ -357,25 +383,23 @@
       if key_usage.key_agreement:
         encipher_only = key_usage.encipher_only
         decipher_only = key_usage.decipher_only
       else:
         encipher_only = decipher_only = False
       builder = builder.add_extension(
         x509.KeyUsage(
-          # pylint: disable=bad-whitespace
           digital_signature =key_usage.digital_signature,
           content_commitment=key_usage.content_commitment,
           key_encipherment  =key_usage.key_encipherment,
           data_encipherment =key_usage.data_encipherment,
           key_agreement     =key_usage.key_agreement,
           key_cert_sign     =False,
           crl_sign          =False,
           encipher_only     =encipher_only,
           decipher_only     =decipher_only,
-          # pylint: enable=bad-whitespace
         ),
         # "SHOULD mark this extension critical"
         critical=key_usage_extension.critical,
       )
     try:
       extended_key_usage = template_csr.extensions.get_extension_for_class(
         x509.ExtendedKeyUsage,
@@ -505,25 +529,23 @@
                 ca=True,
                 path_length=0,
               ),
               critical=True, # "MUST mark the extension as critical"
             ),
             Extension(
               x509.KeyUsage(
-                # pylint: disable=bad-whitespace
                 digital_signature =False,
                 content_commitment=False,
                 key_encipherment  =False,
                 data_encipherment =False,
                 key_agreement     =False,
                 key_cert_sign     =True,
                 crl_sign          =True,
                 encipher_only     =False,
                 decipher_only     =False,
-                # pylint: enable=bad-whitespace
               ),
               critical=True, # "SHOULD mark this extension critical"
             ),
           ] + self._ca_extension_list
         public_key = private_key.public_key()
         now = datetime.datetime.utcnow()
         crt_builder = x509.CertificateBuilder(
@@ -594,17 +616,23 @@
       # No CA cert is valid for more than one certificate life time, so just
       # pick the newest one.
       key_pair = self._ca_key_pairs_list[-1]
     return key_pair
 
   def getCACertificate(self):
     """
-    Return current CA certificate, PEM-encoded.
+    Return oldest still-valid CA certificate, PEM-encoded.
     """
-    return utils.dump_certificate(self._getCurrentCAKeypair()['crt'])
+    self._renewCAIfNeeded()
+    # XXX: _loadCAKeyPairList seems a bit too expensive for such simple operation.
+    # So do out-of-storage self._ca_key_pairs_list pruning only.
+    now = datetime.datetime.utcnow()
+    while self._ca_key_pairs_list[0]['crt'].not_valid_after <= now:
+      self._ca_key_pairs_list.pop(0)
+    return utils.dump_certificate(self._ca_key_pairs_list[0]['crt'])
 
   def getCACertificateList(self):
     """
     Return the current list of CA certificates as X509 obbjects.
     """
     self._renewCAIfNeeded()
     return [x['crt'] for x in self._ca_key_pairs_list]
@@ -632,52 +660,42 @@
     an ancestor certificate.
 
     Note: the chain may contain expired CA certificates. CA user should skip
     these, and consider their signature invalid for CA chain validation
     purposes.
     """
     self._renewCAIfNeeded()
-    result = []
-    iter_key_pair = iter(self._ca_key_pairs_list)
-    first_key_pair = next(iter_key_pair)
-    previous_crt_pem = utils.dump_certificate(first_key_pair['crt'])
-    previous_key = first_key_pair['key']
-    for key_pair in iter_key_pair:
-      current_crt_pem = utils.dump_certificate(key_pair['crt'])
-      result.append(utils.wrap(
-        {
-          'old_pem': utils.toUnicode(previous_crt_pem),
-          'new_pem': utils.toUnicode(current_crt_pem),
-        },
-        previous_key,
-        self.digest_list[0],
-      ))
-      previous_key = key_pair['key']
-      previous_crt_pem = current_crt_pem
-    return result
+    return self._ca_certificate_chain
 
   def revoke(self, crt_pem):
     """
     Revoke certificate.
 
     crt_pem (str)
       PEM-encoded certificat to revoke.
     """
     crt = utils.load_certificate(
       crt_pem,
       self.getCACertificateList(),
-      x509.load_pem_x509_crl(
-        self.getCertificateRevocationList(),
-        _cryptography_backend,
-      ),
+      crl_list=[
+        x509.load_pem_x509_crl(x, _cryptography_backend)
+        for x in self.getCertificateRevocationListDict().itervalues()
+      ],
     )
     self._storage.revoke(
       serial=crt.serial_number,
-      expiration_date=utils.datetime2timestamp(crt.not_valid_after),
+      expiration_date=utils.datetime2timestamp(
+        # https://tools.ietf.org/html/rfc5280#section-3.3
+        # An entry MUST NOT be removed
+        # from the CRL until it appears on one regularly scheduled CRL issued
+        # beyond the revoked certificate's validity period.
+        crt.not_valid_after + self._crl_life_time,
+      ),
     )
+    self._current_crl_dict.clear()
 
   def revokeSerial(self, serial):
     """
     Revoke a certificate by its serial only.
 
     Revocation will expire when the latest CA certificate of this instance
     expires, meaning it will stay longer in the revocation list than when
@@ -686,35 +704,38 @@
     Also, there cannot be any check on the validity of the serial, typos
     are accepted verbatim.
 
     Using this method is hence not recomended.
     """
     self._storage.revoke(
       serial=serial,
-      expiration_date=utils.datetime2timestamp(max(
-        x.not_valid_after for x in self.getCACertificateList()
-      )),
+      expiration_date=utils.datetime2timestamp(
+        max(
+          x.not_valid_after for x in self.getCACertificateList()
+        ) + self._crl_life_time,
+      ),
     )
+    self._current_crl_dict.clear()
 
   def renew(self, crt_pem, csr_pem):
     """
     Renew certificate.
 
     crt_pem (str)
       PEM-encoded certificate to renew.
     csr_pem (str)
       PEM-encoded certificate signing request.
     """
     crt = utils.load_certificate(
       crt_pem,
       self.getCACertificateList(),
-      x509.load_pem_x509_crl(
-        self.getCertificateRevocationList(),
-        _cryptography_backend,
-      ),
+      crl_list=[
+        x509.load_pem_x509_crl(x, _cryptography_backend)
+        for x in self.getCertificateRevocationListDict().itervalues()
+      ],
     )
     return self._createCertificate(
       csr_id=self.appendCertificateSigningRequest(
         csr_pem,
         override_limits=True,
       ),
       auto_signed=_AUTO_SIGNED_PASSTHROUGH,
@@ -727,54 +748,90 @@
       ).sign(
         private_key=self._ca_key_pairs_list[-1]['key'],
         algorithm=self._default_digest_class(),
         backend=_cryptography_backend,
       ),
     )
 
-  def getCertificateRevocationList(self):
+  def getCertificateRevocationListDict(self):
     """
-    Return PEM-encoded certificate revocation list.
+    Return PEM-encoded certificate revocation lists for all CAs.
     """
-    crl_pem = self._storage.getCertificateRevocationList()
-    if crl_pem is None:
-      ca_key_pair = self._getCurrentCAKeypair()
-      now = datetime.datetime.utcnow()
-      crl = x509.CertificateRevocationListBuilder(
-        issuer_name=ca_key_pair['crt'].issuer,
-        last_update=now,
-        next_update=now + self._crl_life_time,
-        extensions=[
-          Extension(
-            x509.CRLNumber(
-              self._storage.getNextCertificateRevocationListNumber(),
+    now = datetime.datetime.utcnow()
+    result = {}
+    crl_pem_dict = self._current_crl_dict
+    self._renewCAIfNeeded()
+    storage = self._storage
+    crl_number, last_update = storage.getCurrentCRLNumberAndLastUpdate()
+    has_renewed = last_update is None
+    last_update = (
+      None
+      if last_update is None else
+      utils.timestamp2datetime(last_update)
+    )
+    revoked_certificate_list = None
+    for ca_key_pair in self._ca_key_pairs_list:
+      authority_key_identifier = ca_key_pair['authority_key_identifier']
+      try:
+        crl_pem, crl_expiration_date = crl_pem_dict[authority_key_identifier]
+      except KeyError:
+        crl_pem = None
+      if crl_pem is None or crl_expiration_date < now:
+        if not has_renewed and crl_pem is not None:
+          # CRL expired, generate a new serial
+          last_update = None
+          has_renewed = True
+        if (
+          last_update is None or
+          last_update + self._crl_renew_time < now
+        ):
+          # We cannot use the existing CRL (or maybe none exist), generate a
+          # new one.
+          last_update = now
+          crl_number = storage.getNextCertificateRevocationListNumber()
+          storage.storeCRLLastUpdate(
+            last_update=utils.datetime2timestamp(last_update),
+          )
+        if revoked_certificate_list is None:
+          revoked_certificate_list = [
+            x509.RevokedCertificateBuilder(
+              serial_number=x['serial'],
+              revocation_date=utils.timestamp2datetime(x['revocation_date']),
+            ).build(_cryptography_backend)
+            for x in storage.getRevocationList()
+          ]
+        ca_crt = ca_key_pair['crt']
+        crl_pem = x509.CertificateRevocationListBuilder(
+          issuer_name=ca_crt.issuer,
+          last_update=last_update,
+          next_update=last_update + self._crl_life_time,
+          extensions=[
+            Extension(
+              x509.CRLNumber(crl_number),
+              critical=False, # "MUST mark this extension as non-critical"
             ),
-            critical=False, # "MUST mark this extension as non-critical"
-          ),
-        ],
-        revoked_certificates=[
-          x509.RevokedCertificateBuilder(
-            serial_number=x['serial'],
-            revocation_date=datetime.datetime.fromtimestamp(
-              x['revocation_date'],
+            Extension(
+              ca_crt.extensions.get_extension_for_class(
+                x509.AuthorityKeyIdentifier,
+              ).value,
+              critical=False, # No mention in RFC5280 5.2.1
             ),
-          ).build(_cryptography_backend)
-          for x in self._storage.getRevocationList()
-        ],
-      ).sign(
-        private_key=ca_key_pair['key'],
-        algorithm=self._default_digest_class(),
-        backend=_cryptography_backend,
-      )
-      crl_pem = crl.public_bytes(serialization.Encoding.PEM)
-      self._storage.storeCertificateRevocationList(
-        crl_pem,
-        expiration_date=utils.datetime2timestamp(now + self._crl_renew_time),
-      )
-    return crl_pem
+          ],
+          revoked_certificates=revoked_certificate_list,
+        ).sign(
+          private_key=ca_key_pair['key'],
+          algorithm=self._default_digest_class(),
+          backend=_cryptography_backend,
+        ).public_bytes(serialization.Encoding.PEM)
+        crl_pem_dict[authority_key_identifier] = (
+          crl_pem,
+          last_update + self._crl_renew_time,
+        )
+      result[authority_key_identifier] = crl_pem
+    return result
 
 class UserCertificateAuthority(CertificateAuthority):
   """
   Backup-able CertificateAuthority.
 
   See backup schema in documentation.
   """
@@ -787,18 +844,18 @@
 
   def doBackup(self, write):
     """
     Backup the entire storage to given path, enciphering it using all stored
     certificates.
     """
     ca_cert_list = self.getCACertificateList()
-    crl = x509.load_pem_x509_crl(
-      self.getCertificateRevocationList(),
-      _cryptography_backend,
-    )
+    crl_list = [
+      x509.load_pem_x509_crl(x, _cryptography_backend)
+      for x in self.getCertificateRevocationListDict().itervalues()
+    ]
     signing_key = os.urandom(32)
     symetric_key = os.urandom(32)
     iv = os.urandom(16)
     encryptor = Cipher(
       algorithms.AES(symetric_key),
       modes.CBC(iv),
       backend=_cryptography_backend,
@@ -809,15 +866,15 @@
       backend=_cryptography_backend,
     )
     symetric_cipher_name = DEFAULT_BACKUP_SYMETRIC_CIPHER
     HMAC_PAYLOAD_SIZE = self.__backup_format_dict[symetric_cipher_name]
     key_list = []
     for crt_pem in self._storage.iterCertificates():
       try:
-        crt = utils.load_certificate(crt_pem, ca_cert_list, crl)
+        crt = utils.load_certificate(crt_pem, ca_cert_list, crl_list)
       except CertificateVerificationError:
         continue
       public_key = crt.public_key()
       key_list.append({
         'id': utils.toUnicode(hexlify(
           x509.SubjectKeyIdentifier.from_public_key(public_key).digest,
         )),
```

### Comparing `caucase-0.9.8/caucase/exceptions.py` & `caucase-0.9.9/caucase/exceptions.py`

 * *Files identical despite different names*

### Comparing `caucase-0.9.8/caucase/http.py` & `caucase-0.9.9/caucase/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,18 @@
   # up calling X509_STORE_add_crl, which either adds the CRL to its list of
   # files or rejects the file. So either memory usage with increase until
   # context gets renewed, or we get stuck with an old CRL. So expect wsgi
   # application to implement these checks on its own when accessing client's
   # certificate.
   #ssl_context.verify_flags = ssl.VERIFY_CRL_CHECK_LEAF
   ssl_context.load_verify_locations(
-    cadata=utils.toUnicode(cau.getCACertificate()),
+    cadata=utils.toUnicode(b'\n'.join(
+      utils.dump_certificate(x)
+      for x in cau.getCACertificateList()
+    )),
   )
   http_cas_certificate_list = http_cas.getCACertificateList()
   threshold_delta = datetime.timedelta(threshold, 0)
   exists = os.path.exists(server_key_path)
   if exists:
     try:
       old_crt_pem = utils.getLeafCertificate(server_key_path)
@@ -359,25 +362,23 @@
               oid=x509.oid.NameOID.ORGANIZATIONAL_UNIT_NAME,
               value=hostname_dnsname,
             ),
           ]),
           extensions=[
             Extension(
               x509.KeyUsage(
-                # pylint: disable=bad-whitespace
                 digital_signature =True,
                 content_commitment=False,
                 key_encipherment  =True,
                 data_encipherment =False,
                 key_agreement     =False,
                 key_cert_sign     =False,
                 crl_sign          =False,
                 encipher_only     =False,
                 decipher_only     =False,
-                # pylint: enable=bad-whitespace
               ),
               critical=True,
             ),
             Extension(
               x509.SubjectAlternativeName([
                 x509.DNSName(hostname_dnsname)
                 if hostname_ip_address is None else
@@ -804,15 +805,15 @@
       sock=https.socket,
       server_side=True,
     )
   if args.backup_directory:
     backup_period = datetime.timedelta(args.backup_period, 0)
     try:
       next_backup = max(
-        datetime.datetime.utcfromtimestamp(os.stat(x).st_ctime)
+        utils.timestamp2datetime(os.stat(x).st_ctime)
         for x in glob.iglob(
           os.path.join(args.backup_directory, '*' + BACKUP_SUFFIX),
         )
       ) + backup_period
     except ValueError:
       next_backup = datetime.datetime.utcnow()
     next_deadline = min(
@@ -1008,27 +1009,27 @@
           },
         ),
       )
   if args.import_ca:
     import_ca_dict = defaultdict(
       (lambda: {'crt': None, 'key': None, 'from': []}),
     )
-    for import_ca in args.import_ca:
-      with open(import_ca, 'rb') as ca_file:
+    password = b''
+    for import_ca_path in args.import_ca:
+      with open(import_ca_path, 'rb') as ca_file:
         ca_data = ca_file.read()
       for index, component in enumerate(pem.parse(ca_data)):
-        name = '%r, block %i' % (import_ca, index)
+        name = '%r, block %i' % (import_ca_path, index)
         if isinstance(component, pem.Certificate):
           component_name = 'crt'
           component_value = x509.load_pem_x509_certificate(
             component.as_bytes(),
             _cryptography_backend,
           )
         elif isinstance(component, pem.Key):
-          password = None
           while True:
             component_name = 'key'
             try:
               component_value = serialization.load_pem_private_key(
                 component.as_bytes(),
                 password,
                 _cryptography_backend,
@@ -1109,51 +1110,79 @@
     if not imported:
       raise ValueError('No CA certificate imported')
     print('Imported %i CA certificates' % imported, file=stdout)
   if args.import_crl:
     db = SQLite3Storage(db_path, table_prefix='cas')
     trusted_ca_crt_set = [
       utils.load_ca_certificate(x['crt_pem'])
-      for x in db.getCAKeyPairList()
+      for x in db.getCAKeyPairList(prune=False)
     ]
     latest_ca_not_after = max(
       x.not_valid_after
       for x in trusted_ca_crt_set
     )
     already_revoked_count = revoked_count = 0
+    crl_number = crl_last_update = None
     for import_crl in args.import_crl:
       with open(import_crl, 'rb') as crl_file:
-        crl_data = crl_file.read()
-      for revoked in utils.load_crl(crl_data, trusted_ca_crt_set):
+        crl = utils.load_crl(crl_file.read(), trusted_ca_crt_set)
+      current_crl_number = crl.extensions.get_extension_for_class(
+        x509.CRLNumber,
+      ).value.crl_number
+      if crl_number is None:
+        crl_number = current_crl_number
+        crl_last_update = crl.last_update
+      else:
+        crl_number = max(crl_number, current_crl_number)
+        crl_last_update = max(crl_last_update, crl.last_update)
+      for revoked in crl:
         try:
           db.revoke(
             revoked.serial_number,
             latest_ca_not_after,
           )
         except exceptions.Found:
           already_revoked_count += 1
         else:
           revoked_count += 1
+    db.storeCRLLastUpdate(utils.datetime2timestamp(crl_last_update))
+    db.storeCRLNumber(crl_number)
+    print(
+      'Set CRL number to %i and last update to %s' % (
+        crl_number,
+        crl_last_update.isoformat(' '),
+      ),
+      file=stdout,
+    )
     print(
       'Revoked %i certificates (%i were already revoked)' % (
         revoked_count,
         already_revoked_count,
       ),
       file=stdout,
     )
   if args.export_ca is not None:
-    encryption_algorithm = serialization.BestAvailableEncryption(
-      getBytePass('CA export passphrase: ')
-    )
+    if os.path.exists(args.export_ca):
+      parser.error('file exists: %r' % (args.export_ca, ))
+    while True:
+      passphrase = getBytePass(
+        'CA export passphrase: ',
+      )
+      if getBytePass(
+        '             (again): ',
+      ) == passphrase:
+        break
+      print('Error: Input does not match, retrying')
+    encryption_algorithm = serialization.BestAvailableEncryption(passphrase)
     with open(args.export_ca, 'wb') as export_ca_file:
       write = export_ca_file.write
       for key_pair in SQLite3Storage(
         db_path,
         table_prefix='cas',
-      ).getCAKeyPairList():
+      ).getCAKeyPairList(prune=False):
         write(
           key_pair['crt_pem'] + serialization.load_pem_private_key(
             key_pair['key_pem'],
             None,
             _cryptography_backend,
           ).private_bytes(
             encoding=serialization.Encoding.PEM,
```

### Comparing `caucase-0.9.8/caucase/__init__.py` & `caucase-0.9.9/caucase/__init__.py`

 * *Files identical despite different names*

### Comparing `caucase-0.9.8/caucase/http_wsgirequesthandler.py` & `caucase-0.9.9/caucase/http_wsgirequesthandler.py`

 * *Files identical despite different names*

### Comparing `caucase-0.9.8/caucase/storage.py` & `caucase-0.9.9/caucase/storage.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,32 +23,35 @@
 """
 from __future__ import absolute_import
 from random import getrandbits
 import os
 import sqlite3
 from threading import local
 from time import time
+from cryptography import x509
+from cryptography.hazmat.backends import default_backend
 from .exceptions import NoStorage, NotFound, Found
-from .utils import toBytes, toUnicode
+from .utils import toBytes, toUnicode, datetime2timestamp
 
 __all__ = ('SQLite3Storage', )
 
+_cryptography_backend = default_backend()
 DAY_IN_SECONDS = 60 * 60 * 24
 
 class NoReentryConnection(sqlite3.Connection):
   """
   Refuse to start an already started transaction.
 
   Allows detecting code bugs which would lead to non-atomic updates (partial
   outer transaction getting committed by an inner transaction).
   """
   __entered = False
 
   def __enter__(self):
-    if self.__entered:
+    if self.__entered: # pragma: no cover
       raise Exception('Subtransactions are not supported')
     self.__entered = True
     return super(NoReentryConnection, self).__enter__()
 
   def __exit__(self, exc_type, exc_value, traceback):
     self.__entered = False
     return super(NoReentryConnection, self).__exit__(exc_type, exc_value, traceback)
@@ -109,15 +112,16 @@
     self._crt_keep_time = crt_keep_time * DAY_IN_SECONDS
     self._crt_read_keep_time = crt_read_keep_time * DAY_IN_SECONDS
     with db:
       # Note about revoked.serial: certificate serials exceed the 63 bits
       # sqlite can accept as integers, so store these as text. Use a trivial
       # string serialisation: not very space efficient, but this should not be
       # a limiting issue for our use-cases anyway.
-      db.cursor().executescript('''
+      c = db.cursor()
+      c.executescript('''
         CREATE TABLE IF NOT EXISTS %(prefix)sca (
           expiration_date INTEGER,
           key TEXT,
           crt TEXT
         );
         CREATE TABLE IF NOT EXISTS %(prefix)scrt (
           id INTEGER PRIMARY KEY,
@@ -127,136 +131,180 @@
           crt TEXT
         );
         CREATE TABLE IF NOT EXISTS %(prefix)srevoked (
           serial TEXT PRIMARY KEY,
           revocation_date INTEGER,
           expiration_date INTEGER
         );
-        CREATE TABLE IF NOT EXISTS %(prefix)scrl (
-          expiration_date INTEGER,
-          crl TEXT
-        );
         CREATE TABLE IF NOT EXISTS %(prefix)scounter (
           name TEXT PRIMARY KEY,
           value INTEGER
         );
         CREATE TABLE IF NOT EXISTS %(prefix)sconfig_once (
           name TEXT PRIMARY KEY,
           value TEXT
-        )
+        );
+        CREATE TABLE IF NOT EXISTS %(prefix)sconfig (
+          name TEXT PRIMARY KEY,
+          value TEXT
+        );
       ''' % {
         'prefix': table_prefix,
         'key_id_constraint': 'UNIQUE' if enforce_unique_key_id else '',
       })
+      try:
+        crl_row = self._executeSingleRow(
+          'SELECT crl FROM %(prefix)scrl '
+          'ORDER BY expiration_date DESC LIMIT 1',
+        )
+      except sqlite3.OperationalError as exc:
+        # XXX: no error codes in sqlite and only a generic error class ?
+        if not exc.args[0].startswith('no such table: '): # pragma: no cover
+          raise
+        crl_row = None
+      if crl_row is not None:
+        self._setConfig(
+          'crl_last_update',
+          str(datetime2timestamp(x509.load_pem_x509_crl(
+            toBytes(crl_row['crl']),
+            _cryptography_backend,
+          ).last_update)),
+        )
+        self._execute(c, 'DROP TABLE IF EXISTS %(prefix)scrl')
+
+  def _execute(self, cursor, sql, parameters=()):
+    return cursor.execute(
+      sql % {
+        'prefix': self._table_prefix,
+      },
+      parameters,
+    )
 
   def _incrementCounter(self, name, increment=1, initial=0):
     """
     Increment counter with <name> by <increment> and return resulting value.
     If <name> is not found, it is created with <initial>, and then incremented.
     Does not commit.
     """
     row = self._executeSingleRow(
-      'SELECT value FROM %scounter WHERE name = ? LIMIT 2' % (
-        self._table_prefix,
-      ),
+      'SELECT value FROM %(prefix)scounter WHERE name = ? LIMIT 2',
       (name, ),
     )
     if row is None:
       value = initial
     else:
       value = row['value']
     value += increment
-    self._db.cursor().execute(
-      'INSERT OR REPLACE INTO %scounter (name, value) VALUES (?, ?)' % (
-        self._table_prefix,
-      ),
+    self._execute(
+      self._db.cursor(),
+      'INSERT OR REPLACE INTO %(prefix)scounter (name, value) VALUES (?, ?)',
       (name, value),
     )
     return value
 
   def _executeSingleRow(self, sql, parameters=()):
     """
     Execute <sql>, raise if it produces more than 1 row, and return it.
     """
-    result_list = self._db.cursor().execute(sql, parameters).fetchall()
+    result_list = self._execute(self._db.cursor(), sql, parameters).fetchall()
     if result_list:
       result, = result_list
       return result
     return None
 
   def getConfigOnce(self, name, default):
     """
     Retrieve the value of <name> from config-once list, or <default> if not
     stored.
     """
     with self._db:
       result = self._executeSingleRow(
-        'SELECT value FROM %sconfig_once WHERE name = ?' % (
-          self._table_prefix,
-        ),
+        'SELECT value FROM %(prefix)sconfig_once WHERE name = ?',
         (name, ),
       )
     if result is None:
       return default
     return result['value']
 
   def setConfigOnce(self, name, value):
     """
     Store <value> as <name> in config-once list, if it was not already stored.
     If it was already stored, do nothing.
     """
     try:
       with self._db as db:
-        db.cursor().execute(
-          'INSERT INTO %sconfig_once (name, value) VALUES (?, ?)' % (
-            self._table_prefix,
-          ),
+        self._execute(
+          db.cursor(),
+          'INSERT INTO %(prefix)sconfig_once (name, value) VALUES (?, ?)',
           (name, value),
         )
     except sqlite3.IntegrityError:
       pass
 
-  def getCAKeyPairList(self):
+  def _getConfig(self, name, default):
+    """
+    Retrieve the value of <name> from config list, or <default> if not
+    stored.
+    """
+    result = self._executeSingleRow(
+      'SELECT value FROM %(prefix)sconfig WHERE name = ?',
+      (name, ),
+    )
+    if result is None:
+      return default
+    return result['value']
+
+  def _setConfig(self, name, value):
+    """
+    Store <value> as <name> in config list, possibly overwriting an existing
+    entry.
+    """
+    self._execute(
+      self._db.cursor(),
+      'INSERT OR REPLACE INTO %(prefix)sconfig (name, value) VALUES (?, ?)',
+      (name, value),
+    )
+
+  def getCAKeyPairList(self, prune=True):
     """
     Return the chronologically sorted (oldest in [0], newest in [-1])
     certificate authority key pairs.
     """
     with self._db as db:
       c = db.cursor()
-      c.execute(
-        'DELETE FROM %sca WHERE expiration_date < ?' % (
-          self._table_prefix,
-        ),
-        (time(), ),
-      )
+      if prune:
+        self._execute(
+          c,
+          'DELETE FROM %(prefix)sca WHERE expiration_date < ?',
+          (time(), ),
+        )
       return [
         {
           'crt_pem': toBytes(x['crt']),
           'key_pem': toBytes(x['key']),
         }
-        for x in db.cursor().execute(
-          'SELECT key, crt FROM %sca ORDER BY expiration_date ASC' % (
-            self._table_prefix,
-          ),
+        for x in self._execute(
+          c,
+          'SELECT key, crt FROM %(prefix)sca ORDER BY expiration_date ASC',
         ).fetchall()
       ]
 
   def appendCAKeyPair(self, expiration_timestamp, key_pair):
     """
     Store a certificate authority key pair.
     expiration_timestamp (int)
       Unix GMT timestamp of CA certificate "valid until" date.
-    key_pair (dict with 'key' and 'crt' items)
+    key_pair (dict with 'key_pem' and 'crt_pem' items)
       CA key pair to store, as bytes.
     """
     with self._db as db:
-      db.cursor().execute(
-        'INSERT INTO %sca (expiration_date, key, crt) VALUES (?, ?, ?)' % (
-          self._table_prefix,
-        ),
+      self._execute(
+        db.cursor(),
+        'INSERT INTO %(prefix)sca '
+        '(expiration_date, key, crt) VALUES (?, ?, ?)',
         (
           expiration_timestamp,
           key_pair['key_pem'],
           key_pair['crt_pem'],
         ),
       )
 
@@ -269,66 +317,59 @@
     """
     Store acertificate signing request and generate a unique ID for it.
     Note: ID uniqueness is only guaranteed among pending CSR, and may be reused
     after the original CSR has been discarded (by being rejected or signed).
     """
     with self._db as db:
       known_csr = self._executeSingleRow(
-        'SELECT id FROM %scrt WHERE csr = ? LIMIT 2' % (
-          self._table_prefix,
-        ),
+        'SELECT id FROM %(prefix)scrt WHERE csr = ? LIMIT 2',
         (csr_pem, ),
       )
       if known_csr is not None:
         return known_csr['id'], None
       if override_limits:
         # Ignore max pending count
         # Do not increment the number of auto-signed certificates, but do not
         # automatically sign either.
         requested_count = None
       else:
         if self._executeSingleRow(
-          'SELECT COUNT(*) FROM %scrt WHERE crt IS NULL' % (
-            self._table_prefix,
-          )
+          'SELECT COUNT(*) FROM %(prefix)scrt WHERE crt IS NULL',
         )[0] >= self._max_csr_amount:
           raise NoStorage
         requested_count = self._incrementCounter('received_csr')
       csr_id = getrandbits(63)
       c = db.cursor()
-      c.execute(
-        'INSERT INTO %scrt (id, key_id, csr) VALUES (?, ?, ?)' % (
-          self._table_prefix,
-        ),
+      self._execute(
+        c,
+        'INSERT INTO %(prefix)scrt (id, key_id, csr) VALUES (?, ?, ?)',
         (
           csr_id,
           key_id,
           csr_pem,
         ),
       )
-      c.execute(
-        'DELETE FROM %scrt WHERE expiration_date < ?' % (
-          self._table_prefix,
-        ),
+      self._execute(
+        c,
+        'DELETE FROM %(prefix)scrt WHERE expiration_date < ?',
         (time(), ),
       )
       return csr_id, requested_count
 
   def deletePendingCertificateSigningRequest(self, csr_id):
     """
     Forget about a pending CSR. Does nothing if the CSR was already signed
     (it will be automatically garbage-collected later).
     Raises NotFound if there is no matching CSR.
     """
     with self._db as db:
       c = db.cursor()
-      c.execute(
-        'DELETE FROM %scrt WHERE id = ? AND crt IS NULL' % (
-          self._table_prefix,
-        ),
+      self._execute(
+        c,
+        'DELETE FROM %(prefix)scrt WHERE id = ? AND crt IS NULL',
         (csr_id, ),
       )
       if c.rowcount == 1:
         return
       raise NotFound
 
   def getCertificateSigningRequest(self, csr_id):
@@ -338,17 +379,15 @@
     csr_id (int)
       Desired CSR id, as given when the CSR was stored.
 
     Raises NotFound if there is no matching CSR.
     """
     with self._db:
       result = self._executeSingleRow(
-        'SELECT csr FROM %scrt WHERE id = ?' % (
-          self._table_prefix,
-        ),
+        'SELECT csr FROM %(prefix)scrt WHERE id = ?',
         (csr_id, ),
       )
       if result is None:
         raise NotFound
       return toBytes(result['csr'])
 
   def getCertificateSigningRequestList(self):
@@ -363,35 +402,33 @@
           'id': str(x['id']),
           # XXX: because only call chain will end up serialising this value in
           # json, and for some reason python3 json module refuses bytes.
           # So rather than byte-ify (consistently with all PEM-encoded values)
           # to then have to unicode-ify, just unicode-ify here.
           'csr': toUnicode(x['csr']),
         }
-        for x in db.cursor().execute(
-          'SELECT id, csr FROM %scrt WHERE crt IS NULL' % (
-            self._table_prefix,
-          ),
+        for x in self._execute(
+          db.cursor(),
+          'SELECT id, csr FROM %(prefix)scrt WHERE crt IS NULL',
         ).fetchall()
       ]
 
   def storeCertificate(self, csr_id, crt):
     """
     Store certificate for pre-existing CSR.
 
     Raises NotFound if there is no matching CSR, or if a certificate was
     already stored.
     """
     with self._db as db:
       c = db.cursor()
-      c.execute(
-        'UPDATE %scrt SET crt=?, expiration_date = ? '
-        'WHERE id = ? AND crt IS NULL' % (
-          self._table_prefix,
-        ),
+      self._execute(
+        c,
+        'UPDATE %(prefix)scrt SET crt=?, expiration_date = ? '
+        'WHERE id = ? AND crt IS NULL',
         (
           crt,
           int(time() + self._crt_keep_time),
           csr_id,
         ),
       )
       if c.rowcount == 0:
@@ -405,28 +442,25 @@
       Desired certificate id, which is the same as corresponding CSR's id.
 
     Raises NotFound if there is no matching CRT or if no certificate was issued
     for it.
     """
     with self._db as db:
       row = self._executeSingleRow(
-        'SELECT crt, expiration_date FROM %scrt '
-        'WHERE id = ? AND crt IS NOT NULL' % (
-          self._table_prefix,
-        ),
+        'SELECT crt, expiration_date FROM %(prefix)scrt '
+        'WHERE id = ? AND crt IS NOT NULL',
         (crt_id, ),
       )
       if row is None:
         raise NotFound
       new_expiration_date = int(time() + self._crt_read_keep_time)
       if row['expiration_date'] > new_expiration_date:
-        db.cursor().execute(
-          'UPDATE %scrt SET expiration_date = ? WHERE id = ?' % (
-            self._table_prefix,
-          ),
+        self._execute(
+          db.cursor(),
+          'UPDATE %(prefix)scrt SET expiration_date = ? WHERE id = ?',
           (
             new_expiration_date,
             crt_id,
           )
         )
       return toBytes(row['crt'])
 
@@ -435,32 +469,31 @@
     Return the certificate corresponding to given key_id.
 
     Raises NotFound if there is no matching CRT or if no certificate was issued
     for it.
     """
     with self._db:
       row = self._executeSingleRow(
-        'SELECT crt FROM %scrt WHERE key_id = ? AND crt IS NOT NULL' % (
-          self._table_prefix,
-        ),
+        'SELECT crt FROM %(prefix)scrt WHERE key_id = ? AND crt IS NOT NULL',
         (key_id, ),
       )
       if row is None:
         raise NotFound
       return toBytes(row['crt'])
 
   def iterCertificates(self):
     """
     Iterator over stored certificates.
     """
     with self._db as db:
       c = db.cursor()
-      c.execute('SELECT crt FROM %scrt WHERE crt IS NOT NULL' % (
-        self._table_prefix,
-      ))
+      self._execute(
+        c,
+        'SELECT crt FROM %(prefix)scrt WHERE crt IS NOT NULL',
+      )
       while True:
         row = c.fetchone()
         if row is None:
           break
         yield toBytes(row['crt'])
 
   def revoke(self, serial, expiration_date):
@@ -472,73 +505,73 @@
       Serial of the certificate to revoke.
     expiration_date (int)
       Unix timestamp at which the certificate expires, allowing to remove this
       entry from the CRL.
     """
     with self._db as db:
       c = db.cursor()
-      c.execute('DELETE FROM %scrl' % (
-        self._table_prefix,
-      ))
       try:
-        c.execute(
-          'INSERT INTO %srevoked '
+        self._execute(
+          c,
+          'INSERT INTO %(prefix)srevoked '
           '(serial, revocation_date, expiration_date) '
-          'VALUES (?, ?, ?)' % (
-            self._table_prefix,
-          ),
+          'VALUES (?, ?, ?)',
           (
             str(serial),
             int(time()),
             expiration_date,
-          )
+          ),
         )
       except sqlite3.IntegrityError:
         raise Found
+      self._incrementCounter('crl_number')
 
-  def getCertificateRevocationList(self):
+  def getNextCertificateRevocationListNumber(self):
     """
-    Get PEM-encoded current Certificate Revocation List.
-
-    Returns None if there is no CRL.
+    Get next CRL sequence number.
     """
     with self._db:
-      row = self._executeSingleRow(
-        'SELECT crl FROM %scrl '
-        'WHERE expiration_date > ? ORDER BY expiration_date DESC LIMIT 1' % (
-          self._table_prefix,
-        ),
-        (time(), )
-      )
-      if row is not None:
-        return toBytes(row['crl'])
-    return None
+      return self._incrementCounter('crl_number')
 
-  def getNextCertificateRevocationListNumber(self):
+  def storeCRLLastUpdate(self, last_update):
     """
     Get next CRL sequence number.
     """
-    return self._incrementCounter('crl_number')
+    with self._db:
+      self._setConfig('crl_last_update', str(last_update))
 
-  def storeCertificateRevocationList(self, crl, expiration_date):
+  def storeCRLNumber(self, crl_number):
     """
-    Store Certificate Revocation List.
+    Set the current CRL sequence number.
+    Use only when importing an existing CA.
     """
     with self._db as db:
-      c = db.cursor()
-      c.execute('DELETE FROM %scrl' % (
-        self._table_prefix,
-      ))
-      c.execute(
-        'INSERT INTO %scrl (expiration_date, crl) VALUES (?, ?)' % (
-          self._table_prefix,
+      self._execute(
+        db.cursor(),
+        'INSERT OR REPLACE INTO %(prefix)scounter (name, value) VALUES (?, ?)',
+        (
+          'crl_number',
+          crl_number,
         ),
+      )
+
+  def getCurrentCRLNumberAndLastUpdate(self):
+    """
+    Get the current CRL sequence number.
+    """
+    with self._db:
+      last_update = self._getConfig('crl_last_update', None)
+      return (
+        # Note: does not increment the counter, but may set it to the default
+        # value.
+        self._incrementCounter('crl_number', increment=0),
         (
-          int(expiration_date),
-          crl,
+          last_update
+          if last_update is None else
+          int(last_update, 10)
         ),
       )
 
   def getRevocationList(self):
     """
     Get the list of all revoked certificates.
 
@@ -546,29 +579,27 @@
     - revocation_date (int)
       Unix timestamp of certificate revocation.
     - serial (int)
       Revoked certificate's serial.
     """
     with self._db as db:
       c = db.cursor()
-      c.execute(
-        'DELETE FROM %srevoked WHERE expiration_date < ?' % (
-          self._table_prefix,
-        ),
+      self._execute(
+        c,
+        'DELETE FROM %(prefix)srevoked WHERE expiration_date < ?',
         (time(), ),
       )
       return [
         {
           'revocation_date': int(x['revocation_date']),
           'serial': int(x['serial']),
         }
-        for x in c.execute(
-          'SELECT revocation_date, serial FROM %srevoked' % (
-            self._table_prefix,
-          ),
+        for x in self._execute(
+          c,
+          'SELECT revocation_date, serial FROM %(prefix)srevoked',
         )
       ]
 
   def dumpIterator(self):
     """
     Backs the *entire* dabase up. This is not limited to tables managed by this
     class (so not limited to table_prefix).
```

### Comparing `caucase-0.9.8/caucase/wsgi.py` & `caucase-0.9.9/caucase/wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 from urllib import quote, urlencode
 from urlparse import parse_qs
 from wsgiref.util import application_uri, request_uri
 import jwt
 from . import utils
 from . import exceptions
 
-# pylint: disable=import-error
+# pylint: disable=import-error,no-name-in-module
 if sys.version_info >= (3, ): # pragma: no cover
   from html import escape
 else: # pragma: no cover
   from cgi import escape
-# pylint: enable=import-error
+# pylint: enable=import-error,no-name-in-module
 
 __all__ = ('Application', 'CORSTokenManager')
 
 # TODO: l10n
 CORS_FORM_TEMPLATE = b'''\
 <html>
 <head>
@@ -168,17 +168,24 @@
   """
   status = _getStatus(httplib.REQUEST_ENTITY_TOO_LARGE)
 
 class InsufficientStorage(ApplicationError):
   """
   No storage slot available (not necessarily out of disk space)
   """
-  # httplib lacks the textual description for 507, although it has the
-  # constant...
+  # python2.7's httplib lacks the textual description for 507, although it
+  # has the constant.
+  # And modern pylint on python3 complain that
+  # http.client.INSUFFICIENT_STORAGE, an enum item, is not suitable for %i
+  # (spoiler: it is suitable).
+  # Also, older pylint (last version suppoting 2.7 ?) does not support
+  # bad-string-format-type but does not detect anything wrong here.
+  # pylint: disable=bad-string-format-type
   status = '%i Insufficient Storage' % (httplib.INSUFFICIENT_STORAGE, )
+  # pylint: enable=bad-string-format-type
 
 STATUS_OK = _getStatus(httplib.OK)
 STATUS_CREATED = _getStatus(httplib.CREATED)
 STATUS_NO_CONTENT = _getStatus(httplib.NO_CONTENT)
 STATUS_FOUND = _getStatus(httplib.FOUND)
 MAX_BODY_LENGTH = 10 * 1024 * 1024 # 10 MB
 
@@ -346,18 +353,32 @@
     #   (default: False)
 
     caucase_routing_dict = {
       'crl': {
         'method': {
           'GET': {
             'do': self.getCertificateRevocationList,
-            'descriptor': [{
-              'name': 'getCertificateRevocationList',
-              'title': 'Retrieve latest certificate revocation list.',
-            }],
+            'subpath': SUBPATH_OPTIONAL,
+            'descriptor': [
+              {
+                'name': 'getCertificateRevocationListList',
+                'title': (
+                  'Retrieve latest certificate revocation list for all valid '
+                  'authorities.'
+                ),
+              },
+              {
+                'name': 'getCertificateRevocationList',
+                'title': (
+                  'Retrieve latest certificate revocation list for given '
+                  'decimal representation of the authority identifier.'
+                ),
+                'subpath': '{+authority_key_id}',
+              },
+            ],
           },
         },
       },
       'csr': {
         'method': {
           'GET': {
             'do': self.getCSR,
@@ -525,15 +546,15 @@
         while path_item_list:
           context = path_entry_dict.get('context', context)
           try:
             path_entry_dict = path_entry_dict['routing'][path_item_list[0]]
           except KeyError:
             break
           del path_item_list[0]
-        # If this raises, it means the outing dict is inconsistent.
+        # If this raises, it means the routing dict is inconsistent.
         method_dict = path_entry_dict['method']
         request_method = environ['REQUEST_METHOD']
         try:
           action_dict = method_dict[request_method]
         except KeyError:
           if request_method == 'OPTIONS':
             status = STATUS_NO_CONTENT
@@ -627,16 +648,22 @@
     """
     Read the entire request body.
 
     Raises BadRequest if request Content-Length cannot be parsed.
     Raises TooLarge if Content-Length if over MAX_BODY_LENGTH.
     If Content-Length is not set, reads at most MAX_BODY_LENGTH bytes.
     """
+    content_length = environ.get('CONTENT_LENGTH')
+    if not content_length:
+      result = environ['wsgi.input'].read(MAX_BODY_LENGTH)
+      if environ['wsgi.input'].read(1):
+        raise TooLarge(b'Content-Length limit exceeded')
+      return result
     try:
-      length = int(environ.get('CONTENT_LENGTH') or MAX_BODY_LENGTH)
+      length = int(content_length, 10)
     except ValueError:
       raise BadRequest(b'Invalid Content-Length')
     if length > MAX_BODY_LENGTH:
       raise TooLarge(b'Content-Length limit exceeded')
     return environ['wsgi.input'].read(length)
 
   def _authenticate(self, environ, header_list):
@@ -647,18 +674,18 @@
     On success, appends a "Cache-Control" header.
     """
     try:
       ca_list = self._cau.getCACertificateList()
       utils.load_certificate(
         environ.get('SSL_CLIENT_CERT', b''),
         trusted_cert_list=ca_list,
-        crl=utils.load_crl(
-          self._cau.getCertificateRevocationList(),
-          ca_list,
-        ),
+        crl_list=[
+          utils.load_crl(x, ca_list)
+          for x in self._cau.getCertificateRevocationListDict().itervalues()
+        ],
       )
     except (exceptions.CertificateVerificationError, ValueError):
       raise SSLUnauthorized
     header_list.append(('Cache-Control', 'private'))
 
   def _readJSON(self, environ):
     """
@@ -683,16 +710,16 @@
       To decide cookie's scope (path).
     value (string)
       Cookie's raw value.
 
     Returns a Morsel instance.
     """
     cookie = SimpleCookie({self._cors_cookie_id: value})[self._cors_cookie_id]
-    cookie['path'] = environ.get('SCRIPT_NAME') or '/',
-    cookie['expires'] = A_YEAR_IN_SECONDS
+    cookie['path'] = environ.get('SCRIPT_NAME') or '/'
+    cookie['max-age'] = A_YEAR_IN_SECONDS
     # No "secure" flag: cookie is not secret, and is protected against
     # tampering on client side.
     # No "httponly" flag: cookie is protected against tampering on client side,
     # and this allows a GUI to list allowed origins and let user delete some
     # (which may not prevent a hostile client from restoring its access for
     # the validity period of their entry - a year by default).
     return cookie
@@ -872,18 +899,19 @@
             assert name not in hal_section_dict, name
             hal_section_dict[name] = descriptor_dict
     return self._returnFile(
       json.dumps(hal).encode('utf-8'),
       'application/hal+json',
     )
 
-  def getCORSForm(self, context, environ): # pylint: disable=unused-argument
+  def getCORSForm(self, context, environ):
     """
     Handle GET /cors .
     """
+    _ = context # Silence pylint
     if environ['wsgi.url_scheme'] != 'https':
       return (
         STATUS_FOUND,
         [
           ('Location', self._https_url),
         ],
         [],
@@ -906,18 +934,19 @@
         # Standard, apparently not widespread yet
         ('Content-Security-Policy', "frame-ancestors 'none'"),
         # BBB
         ('X-Frame-Options', 'DENY'),
       ],
     )
 
-  def postCORSForm(self, context, environ): # pylint: disable=unused-argument
+  def postCORSForm(self, context, environ):
     """
     Handle POST /cors .
     """
+    _ = context # Silence pylint
     if environ['wsgi.url_scheme'] != 'https':
       raise NotFound
     if environ.get('CONTENT_TYPE') != 'application/x-www-form-urlencoded':
       raise BadRequest(b'Unhandled Content-Type')
     try:
       form_dict = parse_qs(
         self._read(environ).decode('ascii'),
@@ -950,26 +979,33 @@
             json.dumps(origin_control_dict),
           ).OutputString(),
         ),
       ],
       [],
     )
 
-  def getCertificateRevocationList(
-    self,
-    context,
-    environ,
-  ): # pylint: disable=unused-argument
+  def getCertificateRevocationList(self, context, environ, subpath):
     """
-    Handle GET /{context}/crl .
+    Handle GET /{context}/crl and GET /{context}/crl/{authority_key_id} .
     """
-    return self._returnFile(
-      context.getCertificateRevocationList(),
-      'application/pkix-crl',
-    )
+    _ = environ # Silence pylint
+    crl_dict = context.getCertificateRevocationListDict()
+    if subpath:
+      try:
+        authority_key_id, = subpath
+        authority_key_id = int(authority_key_id, 10)
+      except ValueError:
+        raise NotFound
+      try:
+        crl = crl_dict[authority_key_id]
+      except KeyError:
+        raise NotFound
+    else:
+      crl = b'\n'.join(crl_dict.itervalues())
+    return self._returnFile(crl, 'application/pkix-crl')
 
   def getCSR(self, context, environ, subpath):
     """
     Handle GET /{context}/csr/{csr_id} and GET /{context}/csr.
     """
     if subpath:
       return self._returnFile(
@@ -1005,49 +1041,39 @@
     self._authenticate(environ, header_list)
     try:
       context.deletePendingCertificateSigningRequest(csr_id)
     except exceptions.NotFound:
       raise NotFound
     return (STATUS_NO_CONTENT, header_list, [])
 
-  def getCACertificate(
-    self,
-    context,
-    environ,
-  ): # pylint: disable=unused-argument
+  def getCACertificate(self, context, environ):
     """
     Handle GET /{context}/crt/ca.crt.pem urls.
     """
+    _ = environ # Silence pylint
     return self._returnFile(
       context.getCACertificate(),
       'application/x-x509-ca-cert',
     )
 
-  def getCACertificateChain(
-    self,
-    context,
-    environ,
-  ): # pylint: disable=unused-argument
+  def getCACertificateChain(self, context, environ):
     """
     Handle GET /{context}/crt/ca.crt.json urls.
     """
+    _ = environ # Silence pylint
     return self._returnFile(
       json.dumps(context.getValidCACertificateChain()).encode('utf-8'),
       'application/json',
     )
 
-  def getCertificate(
-    self,
-    context,
-    environ,
-    subpath,
-  ): # pylint: disable=unused-argument
+  def getCertificate(self, context, environ, subpath):
     """
     Handle GET /{context}/crt/{crt_id} urls.
     """
+    _ = environ # Silence pylint
     return self._returnFile(
       context.getCertificate(self._getCSRID(subpath)),
       'application/pkix-cert',
     )
 
   def revokeCertificate(self, context, environ):
     """
```

### Comparing `caucase-0.9.8/caucase/utils.py` & `caucase-0.9.9/caucase/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 # See https://www.nexedi.com/licensing for rationale and options.
 """
 Caucase - Certificate Authority for Users, Certificate Authority for SErvices
 
 Small-ish functions needed in many places.
 """
 from __future__ import absolute_import, print_function
-from binascii import a2b_base64, b2a_base64
+from binascii import a2b_base64, b2a_base64, hexlify
 import calendar
 import codecs
 from collections import defaultdict
 import datetime
 import email
 import json
 import os
+import sys
 import threading
 import traceback
 import time
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization, hashes
 from cryptography.hazmat.primitives.asymmetric import rsa
@@ -82,15 +83,14 @@
 CAUCASE_LEGACY_OID_TOP = '2.25.285541874270823339875695650038637483517'
 CAUCASE_LEGACY_OID_AUTO_SIGNED = CAUCASE_LEGACY_OID_TOP + '.0'
 CAUCASE_LEGACY_OID_RESERVED = CAUCASE_LEGACY_OID_TOP + '.999'
 _CAUCASE_LEGACY_OID_AUTO_SIGNED = x509.oid.ObjectIdentifier(
   CAUCASE_LEGACY_OID_AUTO_SIGNED,
 )
 
-
 def isCertificateAutoSigned(crt):
   """
   Checks whether given certificate was automatically signed by caucase.
 
   Allows ensuring no rogue certificate could be emitted before legitimate owner
   could take control of their instance: in such case, "first" certificate would
   not appear as auto-signed.
@@ -120,110 +120,144 @@
       entry,
     )
   return result
 
 def getCertList(crt_path):
   """
   Return a list of certificates.
-  Raises if there is anything else than a certificate.
   """
-  if not os.path.exists(crt_path):
+  return _getPEMListFromPath(crt_path, pem.Certificate)
+
+def getCRLList(crl_path):
+  """
+  Return a list of Certificate Revocation Lists.
+  """
+  return _getPEMListFromPath(crl_path, pem.CertificateRevocationList)
+
+def _getPEMListFromPath(path, pem_type):
+  if not os.path.exists(path):
     return []
-  if os.path.isdir(crt_path):
-    file_list = [os.path.join(crt_path, x) for x in os.listdir(crt_path)]
-  else:
-    file_list = [crt_path]
-  result = []
-  for file_name in file_list:
-    type_dict = _getPEMTypeDict(file_name)
-    crt_list = type_dict.pop(pem.Certificate)
-    if type_dict:
-      raise ValueError('%s contains more than just certificates' % (file_name, ))
-    result.extend(x.as_bytes() for x in crt_list)
-  return result
+  return [
+    pem_object.as_bytes()
+    for file_name in (
+      [os.path.join(path, x) for x in os.listdir(path)]
+      if os.path.isdir(path) else
+      [path]
+    )
+    for pem_object in _getPEMTypeDict(file_name).get(pem_type, ())
+  ]
 
 def saveCertList(crt_path, cert_pem_list):
   """
-  Store given list of PEm-encoded certificates in given path.
+  Store given list of PEM-encoded certificates in given path.
 
   crt_path (str)
   May point to a directory a file, or nothing.
   If it does not exist, and this value contains an extension, a file is
   created, otherwise a directory is.
   If it is a file, all certificates are written in it.
   If it is a folder, each certificate is stored in a separate file.
 
   cert_pem_list (list of bytes)
   """
-  if os.path.exists(crt_path):
-    if os.path.isfile(crt_path):
-      saveCertListTo = _saveCertListToFile
-    elif os.path.isdir(crt_path):
-      saveCertListTo = _saveCertListToDirectory
+  _savePEMList(crt_path, cert_pem_list, load_ca_certificate, '.ca.pem')
+
+def saveCRLList(crl_path, crl_pem_list):
+  """
+  Store given list of PEM-encoded Certificate Revocation Lists in given path.
+
+  crl_path (str)
+  May point to a directory a file, or nothing.
+  If it does not exist, and this value contains an extension, a file is
+  created, otherwise a directory is.
+  If it is a file, all CRLs are written in it.
+  If it is a folder, each CRL is stored in a separate file.
+
+  crl_pem_list (list of bytes)
+  """
+  _savePEMList(
+    crl_path,
+    crl_pem_list,
+    lambda x: x509.load_pem_x509_crl(x, _cryptography_backend),
+    '.crl.pem',
+  )
+
+def _savePEMList(path, pem_list, pem_loader, extension):
+  if os.path.exists(path):
+    if os.path.isfile(path):
+      savePEMList = _savePEMListToFile
+    elif os.path.isdir(path):
+      savePEMList = _savePEMListToDirectory
     else:
       raise TypeError('%s exist and is neither a directory nor a file' % (
-        crt_path,
+        path,
       ))
   else:
-    saveCertListTo = (
-      _saveCertListToFile
-      if os.path.splitext(crt_path)[1] else
-      _saveCertListToDirectory
+    savePEMList = (
+      _savePEMListToFile
+      if os.path.splitext(path)[1] else
+      _savePEMListToDirectory
     )
-  saveCertListTo(crt_path, cert_pem_list)
+  savePEMList(path, pem_list, pem_loader, extension)
 
-def _saveCertListToFile(ca_crt_path, cert_pem_list):
-  with open(ca_crt_path, 'wb') as ca_crt_file:
-    ca_crt_file.write(b''.join(cert_pem_list))
-
-def _saveCertListToDirectory(crt_dir, cert_pem_list):
-  if not os.path.exists(crt_dir):
-    os.mkdir(crt_dir)
-  ca_cert_dict = {
-    '%x.pem' % (load_ca_certificate(x).serial_number, ): x
-    for x in cert_pem_list
+def _savePEMListToFile(file_path, pem_list, pem_loader, extension):
+  _ = pem_loader # Silence pylint
+  _ = extension # Silence pylint
+  with open(file_path, 'wb') as pem_file:
+    for pem_chunk in pem_list:
+      pem_file.write(pem_chunk)
+
+def _savePEMListToDirectory(dir_path, pem_list, pem_loader, extension):
+  if not os.path.exists(dir_path):
+    os.mkdir(dir_path)
+  pem_dict = {
+    hexlify(
+      pem_loader(x).extensions.get_extension_for_class(
+        x509.AuthorityKeyIdentifier,
+      ).value.key_identifier,
+    ).decode('ascii') + extension: x
+    for x in pem_list
   }
-  for cert_filename in os.listdir(crt_dir):
-    ca_crt_path = os.path.join(crt_dir, cert_filename)
-    if not os.path.isfile(ca_crt_path):
-      # Not a file and not a symlink to a file, ignore
+  for filename in os.listdir(dir_path):
+    filepath = os.path.join(dir_path, filename)
+    if not filepath.endswith(extension) or not os.path.isfile(filepath):
+      # Not a managed file name and not a symlink to a file, ignore
       continue
-    if not os.path.islink(ca_crt_path) and cert_filename in ca_cert_dict:
+    if not os.path.islink(filepath) and filename in pem_dict:
       try:
         # pylint: disable=unbalanced-tuple-unpacking
-        cert, = getCertList(ca_crt_path)
+        file_pem_item, = _getPEMTypeDict(filepath).itervalues()
         # pylint: enable=unbalanced-tuple-unpacking
       # pylint: disable=broad-except
       except Exception:
       # pylint: enable=broad-except
-        # Inconsistent content (multiple certificates, not CA certificates,
-        # ...): overwrite file
+        # File contains multiple PEM items: overwrite
         pass
       else:
-        if cert == ca_cert_dict[cert_filename]:
+        if file_pem_item == pem_dict[filename]:
           # Already consistent, do not edit.
-          del ca_cert_dict[cert_filename]
+          del pem_dict[filename]
     else:
       # Unknown file (ex: expired certificate), or a symlink to a file: delete
-      os.unlink(ca_crt_path)
-  for cert_filename, cert_pem in ca_cert_dict.items():
-    ca_crt_path = os.path.join(crt_dir, cert_filename)
-    with open(ca_crt_path, 'wb') as ca_crt_file:
-      ca_crt_file.write(cert_pem)
+      os.unlink(filepath)
+  for filename, pem_item in pem_dict.iteritems():
+    filepath = os.path.join(dir_path, filename)
+    with open(filepath, 'wb') as pem_file:
+      pem_file.write(pem_item)
 
 def getCert(crt_path):
   """
   Return a certificate from a file which may also contain a key.
   Raises if there is more or less than one certificate.
   """
   type_dict = _getPEMTypeDict(crt_path)
   crt, = type_dict.get(pem.Certificate)
   return crt.as_bytes()
 
-def getCertKeyAndCACert(crt_path, crl):
+def getCertKeyAndCACert(crt_path, crl_list):
   """
   Return a certificate with its private key and the certificate which signed
   it.
   Raises if there is anything else than two certificates and one key, or if
   their relationship cannot be validated.
   """
   type_dict = _getPEMTypeDict(crt_path)
@@ -237,15 +271,15 @@
     (crt_b, crt_a),
   ):
     try:
       validateCertAndKey(crt, key)
     except ValueError:
       continue
     # key and crt match, check signatures
-    load_certificate(crt, [load_ca_certificate(ca_crt)], crl)
+    load_certificate(crt, [load_ca_certificate(ca_crt)], crl_list)
     return crt, key, ca_crt
   # Latest error comes from validateCertAndKey
   raise # pylint: disable=misplaced-bare-raise
 
 def getLeafCertificate(crt_path):
   """
   Return a regular (non-CA) certificate from a file which may contain a CA
@@ -333,33 +367,38 @@
     cert_pem,
     _cryptography_backend,
   ).public_key().public_numbers() != load_privatekey(
     key_pem,
   ).public_key().public_numbers():
     raise ValueError('Mismatch between private key and certificate')
 
-def _verifyCertificateChain(cert, trusted_cert_list, crl):
+def _verifyCertificateChain(cert, trusted_cert_list, crl_list):
   """
   Verifies whether certificate has been signed by any of the trusted
   certificates, is not revoked and is whithin its validity period.
 
   Raises CertificateVerificationError if validation fails.
   """
   # Note: this function (validating a certificate without an SSL connection)
   # does not seem to have many equivalents at all in python. OpenSSL module
   # seems to be a rare implementation of it, so we keep using this module.
   # BUT it MUST NOT be used anywhere outside this function (hence the
   # bad-style local import). Use "cryptography".
+  # Also, older pylint (last version suppoting 2.7 ?) does not support
+  # import-outside-toplevel but does not detect anything wrong here.
+  # pylint: disable=import-outside-toplevel
   from OpenSSL import crypto
+  # pylint: enable=import-outside-toplevel
   store = crypto.X509Store()
   assert trusted_cert_list
   for trusted_cert in trusted_cert_list:
     store.add_cert(crypto.X509.from_cryptography(trusted_cert))
-  if crl is not None:
-    store.add_crl(crypto.CRL.from_cryptography(crl))
+  if crl_list:
+    for crl in crl_list:
+      store.add_crl(crypto.CRL.from_cryptography(crl))
     store.set_flags(crypto.X509StoreFlags.CRL_CHECK)
   try:
     crypto.X509StoreContext(
       store,
       crypto.X509.from_cryptography(cert),
     ).verify_certificate()
   except (
@@ -452,23 +491,23 @@
   Raises CertificateVerificationError if loaded certificate is not self-signed
   or is otherwise invalid.
   """
   crt = x509.load_pem_x509_certificate(data, _cryptography_backend)
   _verifyCertificateChain(crt, [crt], None)
   return crt
 
-def load_certificate(data, trusted_cert_list, crl):
+def load_certificate(data, trusted_cert_list, crl_list):
   """
   Load a certificate from PEM-encoded data.
 
   Raises CertificateVerificationError if loaded certificate is not signed by
   any of trusted certificates, is revoked or is otherwise invalid.
   """
   crt = x509.load_pem_x509_certificate(data, _cryptography_backend)
-  _verifyCertificateChain(crt, trusted_cert_list, crl)
+  _verifyCertificateChain(crt, trusted_cert_list, crl_list)
   return crt
 
 def dump_certificate(data):
   """
   Serialise a certificate as PEM-encoded data.
   """
   return data.public_bytes(encoding=serialization.Encoding.PEM)
@@ -530,21 +569,47 @@
   """
   crl = x509.load_pem_x509_crl(data, _cryptography_backend)
   for cert in trusted_cert_list:
     if crl.is_signature_valid(cert.public_key()):
       return crl
   raise cryptography.exceptions.InvalidSignature
 
+def _getAuthorityKeyIdentifier(cert):
+  return cert.extensions.get_extension_for_class(
+    x509.AuthorityKeyIdentifier,
+  ).value.key_identifier
+
+if sys.version_info < (3, ): # pragma: no cover
+  def getAuthorityKeyIdentifier(cert):
+    """
+    Returns the authority key identifier of given certificate.
+    """
+    return int(_getAuthorityKeyIdentifier(cert).encode('hex'), 16)
+else: # pragma: no cover
+  def getAuthorityKeyIdentifier(cert):
+    """
+    Returns the authority key identifier of given certificate.
+    """
+    # pylint: disable=no-member
+    return int.from_bytes(_getAuthorityKeyIdentifier(cert), 'big')
+    # pylint: enable=no-member
+
 EPOCH = datetime.datetime(1970, 1, 1)
 def datetime2timestamp(value):
   """
   Convert given datetime into a unix timestamp.
   """
   return int((value - EPOCH).total_seconds())
 
+def timestamp2datetime(value):
+  """
+  Convert given unix timestamp into a datetime.
+  """
+  return EPOCH + datetime.timedelta(0, value)
+
 def timestamp2IMFfixdate(value):
   """
   Convert a timestamp into an IMF-fixdate string following RFC7231.
   """
   return email.utils.formatdate(
     value,
     localtime=False,
```

### Comparing `caucase-0.9.8/caucase/client.py` & `caucase-0.9.9/caucase/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,37 +21,51 @@
 """
 Caucase - Certificate Authority for Users, Certificate Authority for SErvices
 """
 from __future__ import absolute_import
 import datetime
 import httplib
 import json
-import os
 import ssl
 from urlparse import urlparse
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 import cryptography.exceptions
+import pem
 from . import utils
 from . import version
 
 __all__ = (
   'CaucaseError',
+  'CaucaseHTTPError',
+  'CaucaseSSLError',
   'CaucaseClient',
   'HTTPSOnlyCaucaseClient',
 )
 
 _cryptography_backend = default_backend()
 
 class CaucaseError(Exception):
   """
+  Base error for errors when communicating with a caucase server.
+  """
+  pass
+
+class CaucaseHTTPError(CaucaseError):
+  """
   Raised when server responds with an HTTP error status.
   """
   pass
 
+class CaucaseSSLError(CaucaseError):
+  """
+  Raised when there is an SSL error while communicating with the server.
+  """
+  pass
+
 class CaucaseClient(object):
   """
   Caucase HTTP(S) client.
 
   Expose caucase REST API as pythonic methods.
   """
   HTTPConnection = httplib.HTTPConnection
@@ -100,33 +114,46 @@
   def updateCRLFile(cls, url, crl_path, ca_list):
     """
     Bootstrap anf maintain a CRL file up-to-date.
 
     url (str)
       URL to caucase, ending in eithr /cas or /cau.
     crl_path (str)
-      Path to the CRL file, which may not exist.
+      Path to the CRL file or directory, which may not exist.
+      If it does not exist, it is created. If there is an extension, a file is
+      created, otherwise a directory is.
     ca_list (list of cryptography.x509.Certificate instances)
       One of these CA certificates must have signed the CRL for it to be
       accepted.
 
     Return whether an update happened.
     """
-    if os.path.exists(crl_path):
-      with open(crl_path, 'rb') as crl_file:
-        my_crl = utils.load_crl(crl_file.read(), ca_list)
+    def _asCRLDict(crl_list):
+      return {
+        utils.getAuthorityKeyIdentifier(utils.load_crl(x, ca_list)): x
+        for x in crl_list
+      }
+    local_crl_list = utils.getCRLList(crl_path)
+    try:
+      local_crl_dict = _asCRLDict(crl_list=local_crl_list)
+    except x509.extensions.ExtensionNotFound:
+      # BBB: caucased used to issue CRLs without the AuthorityKeyIdentifier
+      # extension. In such case, local CRLs need to be replaced.
+      local_crl_list = []
+      local_crl_dict = {}
+      updated = True
     else:
-      my_crl = None
-    latest_crl_pem = cls(ca_url=url).getCertificateRevocationList()
-    latest_crl = utils.load_crl(latest_crl_pem, ca_list)
-    if my_crl is None or latest_crl.signature != my_crl.signature:
-      with open(crl_path, 'wb') as crl_file:
-        crl_file.write(latest_crl_pem)
-      return True
-    return False
+      updated = len(local_crl_list) != len(local_crl_dict)
+    server_crl_list = cls(ca_url=url).getCertificateRevocationListList()
+    for ca_key_id, crl_pem in _asCRLDict(crl_list=server_crl_list).iteritems():
+      updated |= local_crl_dict.pop(ca_key_id, None) != crl_pem
+    updated |= bool(local_crl_dict)
+    if updated:
+      utils.saveCRLList(crl_path, server_crl_list)
+    return updated
 
   def __init__(
     self,
     ca_url,
     ca_crt_pem_list=None,
     user_key=None,
     http_ca_crt_pem_list=None,
@@ -167,35 +194,56 @@
       context=ssl_context,
     )
 
   def _request(self, connection, method, url, body=None, headers=None):
     path = self._path + url
     headers = headers or {}
     headers.setdefault('User-Agent', 'caucase ' + version.__version__)
-    connection.request(method, path, body, headers)
-    response = connection.getresponse()
-    response_body = response.read()
+    try:
+      connection.request(method, path, body, headers)
+      response = connection.getresponse()
+      response_body = response.read()
+    except ssl.SSLError as exc:
+      raise CaucaseSSLError(exc.errno, exc.strerror)
     if response.status >= 400:
-      raise CaucaseError(response.status, response.getheaders(), response_body)
+      raise CaucaseHTTPError(
+        response.status,
+        response.getheaders(),
+        response_body,
+      )
     assert response.status < 300 # caucase does not redirect
     if response.status == 201:
       return response.getheader('Location')
     return response_body
 
   def _http(self, method, url, body=None, headers=None):
     return self._request(self._http_connection, method, url, body, headers)
 
   def _https(self, method, url, body=None, headers=None):
     return self._request(self._https_connection, method, url, body, headers)
 
-  def getCertificateRevocationList(self):
+  def getCertificateRevocationList(self, authority_key_identifier):
+    """
+    [ANONYMOUS] Retrieve latest CRL for given integer authority key
+    identifier.
+    """
+    return self._http(
+      'GET',
+      '/crl/%i' % (authority_key_identifier, ),
+    )
+
+  def getCertificateRevocationListList(self):
     """
-    [ANONYMOUS] Retrieve latest CRL.
+    [ANONYMOUS] Retrieve the latest CRLs for each CA certificate.
     """
-    return self._http('GET', '/crl')
+    return [
+      x.as_bytes()
+      for x in pem.parse(self._http('GET', '/crl'))
+      if isinstance(x, pem.CertificateRevocationList)
+    ]
 
   def getCertificateSigningRequest(self, csr_id):
     """
     [ANONYMOUS] Retrieve an CSR by its identifier.
     """
     return self._http('GET', '/csr/%i' % (csr_id, ))
```

