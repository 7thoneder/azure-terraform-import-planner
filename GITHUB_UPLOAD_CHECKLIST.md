# GitHub Upload Checklist

Upload the contents of this folder to your GitHub repository.

## Files And Folders To Commit

- `.gitignore`
- `README.md`
- `package.json`
- `desktop/`
- `docs/`
- `GITHUB_UPLOAD_CHECKLIST.md`

## Do Not Commit

The `.gitignore` excludes generated and local files such as:

- `node_modules/`
- `outputs/`
- `work/`
- `dist/`
- `.wrangler/`
- `.vinext/`
- Electron package output
- local editor and OS files

## First-Time Setup

```bash
pnpm install
```

## Run The App During Development

```bash
pnpm run desktop
```

## Package The Windows Desktop App

```bash
pnpm run desktop:package
```

## Azure Setup Reminder

The Azure App Registration must have:

```text
Allow public client flows: Yes
```

Users loading remote Terraform state from Azure Storage need:

```text
Storage Blob Data Reader
```
