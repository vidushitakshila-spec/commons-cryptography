# commons-cryptography
1. Problem statement: Developers write bespoke, insecure cryptographic code (e.g., ECB mode, weak IVs, hardcoded secrets) for encryption needs.

2. Concepts and terminology: AES-GCM-256, Initialization Vector (IV), Salt, PBKDF2, Authenticated Encryption.

3. Available technologies / algorithms: JCA (Java Cryptography Architecture), Bouncy Castle, AES/GCM/NoPadding.

4. When to use what: Use for all symmetric/asymmetric cryptographic operations, file encryption, and payload signing across backend services.

5. Java APIs and dependencies: javax.crypto.*, Bouncy Castle Provider.

6. AWS equivalents: AWS KMS (Key Management Service).

7. Architecture patterns: Envelope Encryption, Secure Factory Pattern, Cryptographic Agile wrappers.

8. Security considerations: Never reuse IVs with AES-GCM; ensure secure memory zeroing for sensitive byte arrays where applicable.

9. Implementation examples: Utility service handling AES-GCM encryption with authenticated tag verification and randomized 12-byte IV generation.

10. References and further reading: NIST SP 800-38D (Recommendation for Block Cipher Modes of Operation: GCM).
