# SwiftWoo Free

A Next.js storefront for WordPress and WooCommerce.

## Setup

1. Use Node.js 22 or newer and run `npm ci`.
2. Configure WordPress, WooCommerce, WPGraphQL, and JWT Authentication.
3. Copy `.env.example` to `.env.local` and configure your own backend URLs and credentials.
4. Run `npm run dev`.
5. Run `npm run build -- --webpack` and `npm start` for a production build.

## Deployment

Import this repository into a compatible Next.js / Node.js hosting account. Set environment variables in the host settings before building. NEXT_PUBLIC_* values are public and may be embedded at build time. Keep WooCommerce, JWT, payment, connection and revalidation secrets server-side. Never commit your .env.local file. Configure your own domain, HTTPS, backend reachability and permitted image host. Test authentication, cart, taxes, shipping and payments before launch. Hosting deployment has not been certified by this source snapshot.

## Release status

This is a development preview, not a production-readiness certification. Known review items include order ownership enforcement, customer identity at checkout, password recovery, input validation, shipping/tax behavior and an existing lint baseline. Use a test backend until these are resolved.

## License and attribution

GPL-3.0; see LICENSE. Derived from wpacademy/nextjs-woocommerce-frontend. This repository contains the Free frontend only. SwiftWoo Pro source and Core plugin are distributed separately.
