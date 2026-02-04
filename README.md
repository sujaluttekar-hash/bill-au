# spp.py

## Secrets & configuration

Do not commit real credentials. Provide them at runtime using environment variables or local files that are excluded from git.

### Required environment variables

Set these as needed for your workflows:

```
STAYVISTA_USERNAME=your-email@example.com
STAYVISTA_PASSWORD=your-password
EMAIL=your-email@example.com
PASSWORD=your-password
X_AUTH_TOKEN=your-api-token
GOOGLE_OAUTH_CLIENT_ID=your-google-client-id
GOOGLE_OAUTH_CLIENT_SECRET=your-google-client-secret
GOOGLE_OAUTH_CLIENT_SECRETS=/absolute/path/to/oauth.json
```

### OAuth client secrets file

1. Copy `oauth.template.json` to `oauth.json`.
2. Replace the placeholder values with your real OAuth client values.
3. Keep `oauth.json` untracked (it is ignored by `.gitignore`).

### Example `.env`

Use `.env.example` as a starting point and load it with your preferred tooling.
