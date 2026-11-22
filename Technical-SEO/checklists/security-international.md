# Checklist: Security and Internationalization

## Security and status codes

- [ ] Important pages use HTTPS and HTTP URLs redirect consistently to the preferred HTTPS URL
- [ ] TLS certificates are valid for the domains in use
- [ ] Pages do not load critical resources over insecure connections
- [ ] Security issues shown in webmaster tools are reviewed when access is available
- [ ] Important URLs return the expected status; errors are not disguised as successful pages
- [ ] Redirects use an appropriate destination and status code; temporary and permanent changes are distinguished
- [ ] Removed URLs return an appropriate not-found or gone response, or redirect to a genuinely equivalent replacement
- [ ] Redirect loops and long chains are absent from important paths

## Internationalization (when applicable)

- [ ] Language and regional versions are clearly identified and have equivalent content where expected
- [ ] `hreflang` values use valid language/region codes and point to canonical, indexable URLs
- [ ] Alternate-language references are reciprocal and include the page itself
- [ ] `x-default` is used when an appropriate fallback page exists
- [ ] Language targeting, page content, navigation, and destination URLs agree
- [ ] Canonical and hreflang signals do not conflict

**Related fix guides:** `fixes/security-international/`
