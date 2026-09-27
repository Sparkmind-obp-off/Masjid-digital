# TECHNICAL ARCHITECTURE

## Recommended
- Frontend: React/Next.js atau equivalent.
- Backend: lightweight serverless endpoints.
- Database: Cloudflare D1 atau relational free-tier equivalent.
- Storage: object storage untuk galeri bila diperlukan.
- Auth: secure admin authentication.
- Hosting: Cloudflare Pages/Workers atau equivalent.

## Flow
Browser → Web App → API → Database
                         └→ Object Storage

## Requirements
- Environment variables untuk secrets.
- Server-side authorization.
- Input validation.
- Rate limiting where appropriate.
- Audit logging.
- No secrets in frontend bundle.
