# 404 Website Blocker

A Chrome Manifest V3 extension that redirects every normal HTTP/HTTPS top-level navigation to a 404-style page, while allowing `google.com` and its subdomains.

## Install locally

1. Open `chrome://extensions`.
2. Turn on **Developer mode**.
3. Click **Load unpacked**.
4. Select this repository folder.
5. Visit a website such as `https://example.com`; it should show the 404 page.
6. Visit `https://www.google.com`; Google should load normally.

## Notes

Chrome's declarative network request API performs the redirect before the normal page is displayed. The allow rule has higher priority than the catch-all redirect, so `google.com` is left untouched.
