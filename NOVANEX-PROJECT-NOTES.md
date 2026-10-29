# Novanex Global Bank — project notes

Novanex Global Bank is a separately identified banking-style software prototype. It is not affiliated with or endorsed by any real financial institution and must not collect real banking credentials or process real funds.

## Requested scope
- Premium navy, gold, and white visual identity with original logo and copy
- Customer registration and account dashboard
- Separate protected administrator dashboard
- Transaction history and simulated transfers using clearly labelled demo data
- Notification preferences and email alerts when a verified mail provider is configured

## Security requirements before deployment
- Keep all secrets in environment variables; never commit credentials, recovery phrases, API keys, or production customer data.
- Rotate any credential or recovery phrase that has appeared in a public repository. Deleting a file does not remove it from prior Git history.
- Audit authentication, authorization, session handling, rate limits, validation, database access, and email flows before exposing the app publicly.
- Use synthetic demo accounts and non-real balances. Do not connect to real banking rails until a properly licensed and reviewed integration exists.
- Configure production environment variables in Vercel; do not place secret values in source files.

## Source preservation
This working branch is based on `Flamzyberry/riyadnational` for review. The `master` branch is unchanged. This branch is not yet a separate GitHub repository and is not ready for production deployment.
