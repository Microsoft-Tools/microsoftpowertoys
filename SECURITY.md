# Security Policy

## 🔒 Supported Versions

We provide security updates for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| 2.x.x   | ✅ |
| 1.x.x   | ✅ |
| < 1.0   | ❌ |

## 🛡️ Security Considerations

### What We Secure

- **Offline Installation Process**: Ensuring integrity of PowerToys binaries
- **Administrator Privileges**: Safe handling of elevated permissions
- **Registry Modifications**: Secure system integration
- **File System Access**: Safe deployment to system directories
- **Network Communications**: When downloading components (optional)

### What We Don't Secure

This assistant is a deployment tool and does **not**:
- Modify PowerToys security features
- Handle PowerToys runtime security
- Provide antivirus or anti-malware protection
- Secure end-user PowerToys configurations

## 🚨 Reporting a Vulnerability

If you discover a security vulnerability, please report it privately:

### 📧 Contact Methods

**Primary**: Create a private security advisory on GitHub
1. Go to the "Security" tab in this repository
2. Click "Report a vulnerability"
3. Fill out the advisory details

**Alternative**: Email security concerns to:
- **Email**: `security@microsoft-tools.github.io`
- **Subject**: `[SECURITY] PowerToys Assistant - [Brief Description]`

### 📋 What to Include

Please provide:

1. **Vulnerability Type**: Buffer overflow, privilege escalation, etc.
2. **Impact Assessment**: What systems/data could be affected
3. **Reproduction Steps**: Detailed steps to reproduce the issue
4. **Environment Details**: Windows version, PowerShell version, etc.  
5. **Proof of Concept**: Code samples or screenshots (if safe to share)
6. **Suggested Fix**: If you have ideas for remediation

### ⏰ Response Timeline

- **Initial Response**: Within 48 hours
- **Assessment Complete**: Within 1 week
- **Fix Development**: 2-4 weeks (depending on complexity)
- **Public Disclosure**: After fix is released

### 🏆 Recognition

Security researchers will be credited in:
- Security advisory acknowledgments
- Release notes
- Special recognition in `SECURITY.md`

## 🔍 Security Best Practices

### For Users

- **Always run as Administrator**: Required for system-level installation
- **Verify File Integrity**: Check hashes of downloaded components
- **Use Antivirus**: Scan all files before execution  
- **Backup System**: Create restore point before installation
- **Keep Updated**: Use latest version of the assistant

### For Contributors

- **Code Review**: All PRs require security review
- **Input Validation**: Sanitize all user inputs
- **Privilege Minimization**: Use least privilege necessary
- **Secure Defaults**: Safe configurations by default
- **Error Handling**: Don't expose sensitive information in errors

## 🛠️ Security Features

### Built-in Protections

- **Hash Verification**: Validates integrity of downloaded files
- **Digital Signature Checks**: Verifies Microsoft-signed binaries
- **Safe Path Handling**: Prevents directory traversal attacks
- **Input Sanitization**: Cleans user-provided paths and parameters
- **Administrative Validation**: Confirms elevated privileges before proceeding

### Audit Trail

The assistant logs:
- Installation steps and outcomes
- File modifications and registry changes
- Error conditions and warnings
- Administrative actions taken

Logs are stored in: `%TEMP%\PowerToysAssistant\logs\`

## 🔐 Cryptographic Details

### File Integrity

- **Algorithm**: SHA-256 hashing
- **Verification**: Against known good hashes
- **Sources**: Official Microsoft distribution channels

### Secure Downloads (When Used)

- **Protocol**: HTTPS only
- **Certificate Validation**: Full chain verification
- **Retry Logic**: Secure failure handling

## 📚 Additional Resources

- [Microsoft Security Response Center](https://msrc.microsoft.com/)
- [PowerToys Official Security Policy](https://github.com/microsoft/PowerToys/security/policy)
- [Windows Security Best Practices](https://docs.microsoft.com/en-us/windows/security/)

---

**We take security seriously and appreciate your help in keeping our users safe!** 🙏 