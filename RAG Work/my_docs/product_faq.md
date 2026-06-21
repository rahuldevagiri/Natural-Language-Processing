# CloudSync Pro — Frequently Asked Questions

## What is CloudSync Pro?

CloudSync Pro is a file synchronization and backup service for teams. It
automatically syncs folders across devices, keeps a 30-day version history
for every file, and lets you share folders with external collaborators
through secure, expiring links.

## Pricing

CloudSync Pro is offered in three tiers:

- **Starter** — $8/user/month. Includes 100GB of storage per user and
  7-day version history.
- **Business** — $15/user/month. Includes 1TB of storage per user, 30-day
  version history, and admin controls for team-wide sharing policies.
- **Enterprise** — custom pricing. Includes unlimited storage, 90-day
  version history, single sign-on (SSO), and a dedicated support contact.

All plans include a 14-day free trial with no credit card required.

## How does file syncing work?

CloudSync Pro uses a delta-sync algorithm: instead of re-uploading an entire
file when it changes, it only uploads the modified blocks. This makes
syncing large files (such as design files or video projects) significantly
faster than full re-uploads. Sync conflicts — for example, when two people
edit the same file offline — are resolved by keeping both versions and
appending the editor's name and timestamp to the conflicting copy.

## Troubleshooting: Sync Stuck or Paused

If sync appears stuck, first check the CloudSync Pro menu-bar icon for a
status message. Common causes and fixes:

1. **"Sync paused — low disk space."** Free up at least 5GB on the local
   drive and sync will resume automatically.
2. **"Sync paused — network unstable."** CloudSync Pro automatically retries
   every 60 seconds. You can force a retry by clicking "Sync Now" in the
   menu.
3. **A single file won't sync.** This is usually caused by an unsupported
   character in the filename (such as `:` or `*`) or a file size over the
   5GB single-file limit on the Starter plan (50GB on Business and
   Enterprise).

If none of these resolve the issue, generate a diagnostic report from
Settings → Help → Export Diagnostics and send it to support@cloudsyncpro.com.

## Security

All files are encrypted in transit using TLS 1.3 and at rest using AES-256.
Enterprise customers can enable customer-managed encryption keys (CMEK) for
an additional layer of control. CloudSync Pro is SOC 2 Type II certified and
undergoes annual third-party penetration testing.

## Canceling a Subscription

You can cancel anytime from Settings → Billing → Cancel Plan. Your data
remains accessible in a read-only state for 30 days after cancellation,
after which it is permanently deleted unless you export it first.
