# Black Eagle Tours & Safaris

Updated responsive React/Vite website.

## Run locally
1. Install Node.js 20 or newer.
2. Run `npm install`.
3. Run `npm run dev` for development or `npm run build` for production.

## Content notes
- The supplied hero video is retained and now uses `preload=metadata` to reduce initial loading.
- Uploaded photographs are converted to WebP for faster delivery and stored in `public/images/gallery`.
- The original supplied itinerary PDFs are available in `public/itineraries`.
- Contact form opens the visitor's email app with a drafted enquiry; it does not send a message automatically or guarantee phone notifications. Configure a server-side email provider for automatic notifications.
- Browser image copying cannot be fully prevented; the site uses display-optimized images and discourages casual copying.
- The original archive contained 80 image files (some duplicates), not 94 distinct images. The gallery manifest uses unique image content.
