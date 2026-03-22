# NÍKĒ — Free, Deniable, Steganographic Communications

**For journalists, dissidents, activists, and anyone living under authoritarian surveillance.**

Free. Open source. No account. No server required. No traces.

---

## What It Does

NÍKĒ hides encrypted messages inside normal-looking text. A guard reads the message and sees physics equations. The recipient reads the same message and extracts the real communication.

Three steganographic channels:

- **Channel 1 — Zero-Width Unicode:** Invisible characters between letters. Fast. Stripped by aggressive scrapers.
- - **Channel 2 — Whitespace:** Data encoded in space/tab patterns. Survives most filters.
  - - **Channel 3 — Linguistic:** Data encoded in word choice. Survives DPI, AI content scanning, printing, and retyping. Use this in high-threat environments.
   
    - All channels use AES-256-GCM encryption with PBKDF2 key derivation (100,000 iterations).
   
    - **Deniability:** A different passphrase produces different innocent output. Mathematically impossible to prove another message exists.
   
    - ---

    ## How to Use

    ### Offline (no internet required)
    Download `nike_offline.html` and open it in any browser. Works on a USB drive. Leaves no traces when the tab is closed.

    ### Online via Tor
    ```
    kn5pskbnjemjv6cgh5vre7zpvfrpq5puigjkfsqrl53vqzfuhvnht4id.onion
    ```
    Accessible from Iran, Russia, China, and North Korea via [Tor Browser](https://torproject.org) — free to download.

    ### Online clearnet
    ```
    https://smarthub.my/comms
    ```

    ---

    ## Threat Model

    Built for users whose devices may be physically inspected and whose network traffic is monitored by a state-level adversary.

    Channel 3 (linguistic steganography) produces output that looks like normal academic or personal writing. No file attachments. No unusual characters. No metadata. Sends through any channel — email, SMS, forum post, comment section.

    ---

    ## Keys

    The Keys tab generates an ECDH P-256 keypair for end-to-end encrypted communication. The private key can be:
    - Downloaded as a `.txt` file
    - - Saved as a QR code photograph
      - - Stored on an encrypted USB drive
       
        - Never share the private key. Never store it in cloud services.
       
        - ---

        ## Distribution

        If you are an organization working with people in repressive environments — journalists, dissidents, human rights workers — please share or mirror this tool. No permission needed. MIT license.

        ---

        ## Technical Details

        - Encryption: AES-256-GCM
        - - Key derivation: PBKDF2-SHA256, 100,000 iterations
          - - Key exchange: ECDH P-256
            - - Steganography: Zero-width Unicode / whitespace / synonym substitution
              - - Size: ~23KB, single HTML file, zero dependencies (offline mode)
                - - Runs entirely in the browser — no server, no logs, no telemetry
                 
                  - ---

                  ## Cover

                  The clearnet host is a legitimate mathematical physics research wiki (RTSG framework, 177+ pages, cited by researchers). A government blocking `smarthub.my` blocks real academic content — the political cost is high.

                  ---

                  ## Author

                  Jean-Paul Niko · [smarthub.my](https://smarthub.my) · 2026

                  MIT License — free to use, copy, modify, distribute.
