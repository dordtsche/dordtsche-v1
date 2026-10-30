# Agent Log

## [2026-10-30 10:22:00 CET] - Update @tanstack/react-start to Patch CVE-2026-102989

- **Problem:** Vercel deployment failed because `@tanstack/react-start@1.168.32` contained a known cross-site scripting (XSS) vulnerability (`CVE-2026-102989`), requiring version `1.168.60` or later.
- **Solution:** Updated `@tanstack/react-start` to `1.169.4` along with aligned peer packages `@tanstack/react-router` (`1.170.46`) and `@tanstack/router-plugin` (`1.168.48`) in [package.json](file:///c:/Users/pc/dev/work-dev/dordtsche-v1/package.json) and [bun.lock](file:///c:/Users/pc/dev/work-dev/dordtsche-v1/bun.lock) using Bun.
- **Date & Time:** 2026-10-30 10:22:00 CET.

## [2026-09-21 20:05:00 CET] - Implement Frontend Access Lock via hotpax

- **Problem:** The client/owner of the site has not paid the developer, requiring the frontend to be locked with an access restriction screen.
- **Solution:** Integrated `LockGate` from `hotpax` into [__root.tsx](file:///c:/Users/pc/dev/work-dev/dordtsche-v1/src/routes/__root.tsx) with `hasPaid={false}`, passing site branding, support email, and an `errorCode="PAY_PENDING"`, securely locking the frontend when unpaid while preserving clean unblock capability once resolved.
- **Date & Time:** 2026-09-21 20:05:00 CET.
