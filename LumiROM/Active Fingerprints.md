# Integrity Verification

These checksums can be used to verify that archived files have not been modified, corrupted, or tampered with.

---

## Archive Fingerprints

| Artifact | File Name | SHA256 |
|-----------|-----------|---------|
| LumiROM v8.6.2 Stable | `LumiROM_8.6.2-12052026_a32.zip` | `dbdee40afecf25d2bdb0622e2a04a7b292821aa3f1c732f26cfc67ab7ff56433` |
| LumiVENDOR OneUI 8.5 | `LumiVENDOR_OneUi8.5-new-a32.zip` | `6791a3ebe42e6413b086b2fbfa93009ed80bd11a7c05c4936d2dd32b678d3ec0` |

---

## Verification

### Windows

```cmd
certutil -hashfile "filename.zip" SHA256
```

### Linux

```bash
sha256sum filename.zip
```

### Android (Termux)

```bash
sha256sum filename.zip
```

If the generated SHA256 value matches the corresponding fingerprint listed above, the file can be considered identical to the archived copy.
