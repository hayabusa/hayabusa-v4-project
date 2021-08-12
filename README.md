# hayabusa-v4-project
Hayabusa v4 Project

# Why
The web deserves **better interoperability** between clients and Image CDNs. The Image CDN community is in a similar place as the industrial revolution before standardization. Untold amounts of human effort are exhausted globally every day on **rebuilding, learning and teaching different CDN APIs**.

**This should not be the case**. The CDN community and Browser community should come together to standardize namings and structures for common use cases and parameters. We should set a path for **existing solutions to converge**.

The first step is to stop using in-house half-baked solutions and move to cloud-based dedicated solutions.

# Architecture Design

## Facade API
Currently we support the following systems through Facade APIs:
- CyberAgent's Hayabusa v1
- CyberAgent's Hayabusa v3
- CyberAgent's Stat Image Server 

## Edge
For the Edge Facade API we currently support the following Edge computing CDNs:
- Cloudflare Workers

## Image Processing
For the image processing we currently support the following Image Processing Providers:
- Cloudinary

We're open to add support for different architectures. Any PR is welcome!
# Usage

Run on local

# For Cloudflare
Specify your `account ID` and `zone ID` using environment variables.
```
CF_ACCOUNT_ID=XXXXX CF_ZONE_ID=XXXXX wrangler dev
```

# Development

Formatting
```
npm run format
```

Lint
```
npm run lint
```

Test
```
npm run test
```

> Note: Husky executes `format`, `lint` and `test` before `git commit`.
