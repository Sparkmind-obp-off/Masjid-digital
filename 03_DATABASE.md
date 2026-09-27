# DATABASE MODEL

## mosques
id, name, slug, address, description, phone, whatsapp, created_at, updated_at

## events
id, title, description, speaker, location, starts_at, ends_at, status, created_at, updated_at

## announcements
id, title, body, published_at, status, created_at, updated_at

## gallery
id, title, image_url, caption, published_at

## transactions
id, type(income|expense), category, amount, description, transaction_date, created_at, created_by

## admins
id, email, role, created_at, updated_at

## audit_logs
id, actor_id, action, entity, entity_id, metadata, created_at

## Security
- Admin-only writes.
- Public reads only for published content.
- Financial records private by default.
- Secrets only in environment variables.
