# Website update notes

## Implemented in this package
- Rebuilt the landing page with a responsive editorial layout and mobile navigation.
- Kept the supplied hero video and changed it to `preload="metadata"` to reduce initial video download priority.
- Added a locally stored text-based Black Eagle wordmark SVG so the header branding displays even if the former external logo host is unavailable.
- Replaced the wave-shaped philosophy treatment with a square-edged image-and-copy layout.
- Added experience sections for wildlife, mountain adventures and coastal holidays.
- Reworked itinerary cards and a readable day-by-day detail modal with large image placement.
- Added a six-image gallery preview and a full gallery toggle.
- Converted supplied photos to WebP, reduced their dimensions for web display, and removed duplicate image content from the public gallery.
- Copied the eight supplied itinerary PDFs into `public/itineraries`.
- Added responsive mobile and reduced-motion CSS.

## Important content limitations
- The supplied archive contains 80 image files, with repeated/duplicate content; the public gallery uses 41 unique images from the supplied set.
- The supplied images mainly show wildlife and inland landscapes. No clearly identifiable Zanzibar beach or mountain-climbing photographs were present, so the experience cards currently use the closest supplied landscape/water images. Replace those two images with owner-approved authentic beach and climbing photographs before publication.
- The owner's original logo file was not present in either ZIP. `public/brand/black-eagle-mark.svg` is a local temporary wordmark, not a recreation of the official logo artwork. Replace it with the official logo asset when supplied.
- Itinerary PDFs are included for reference, but their text and every itinerary day have not been fully reconciled against the current itinerary data in this pass. Verify every day, accommodation, price, and destination with the owner before launch.
- The current enquiry form opens a prefilled email in the visitor's email app. It does not automatically send an email or create phone notifications. The existing server supports SMTP configuration, which must be configured and connected to the form for automatic notifications.
- Browser image saving cannot be completely blocked. The site uses optimized display copies; screenshots and other copying methods remain possible.

## Run and test
- Requires Node.js and npm.
- Run `npm install`, then `npm run build`.
- This package could not be dependency-installed or production-built in the current environment because package installation timed out; run the build locally before deployment.

## Premium footer refinement (2026-10-18)
- Reworked the footer into a premium multi-column layout with brand statement, location, curated navigation, enquiry contact, and a clear safari call-to-action.
- Added responsive tablet/mobile layouts and subtle hover states.
- Kept contact details consistent with the existing website configuration; no unverified social accounts or phone numbers were invented.

## Admin dashboard status
- A secure, working admin dashboard is not yet configured in this package. It requires a real authentication provider and protected persistent storage/rules for bookings, enquiries, itinerary updates, and media uploads. A front-end-only login would not secure customer data, so this is intentionally not represented as completed.

## Build verification
- Production build could not be verified in this environment because dependencies are not installed (`vite: not found`). Run `npm install` and `npm run build` in the project directory before deploying.
