# Instagram Live Feed Widget — paellasymas

**Widget service:** Elfsight Instagram Feed  
**Handle:** @paellasymas  
**Status:** Embed code integrated · Widget ID pending activation  
**Last updated:** 2026-05-21 · feat(v4.3)

---

## Setup Instructions (5 minutes)

### Step 1 — Create Elfsight Account

1. Go to [https://elfsight.com/instagram-feed-instashow/](https://elfsight.com/instagram-feed-instashow/)
2. Click **Create Widget for Free**
3. Sign up with email (no credit card required)
4. Account email to use: create a FORGE Digital shared account (e.g., `forge.widgets@gmail.com`)

### Step 2 — Connect @paellasymas Instagram Account

> **Important:** Instagram requires the account owner to authorize OAuth access. Chef Janet must log into Instagram during this step.

1. In the Elfsight dashboard, click **Add New Widget → Instagram Feed**
2. Click **Connect Instagram Account**
3. Log in as @paellasymas (Chef Janet's credentials)
4. Authorize Elfsight to read the public feed
5. Select @paellasymas as the feed source

### Step 3 — Configure Widget Appearance

Match the paellasymas brand palette:

| Setting | Value |
|---|---|
| Layout | Grid |
| Columns (desktop) | 4 |
| Columns (tablet) | 3 |
| Columns (mobile) | 2 |
| Posts to show | 12 |
| Image size | Square |
| Hover effect | Overlay with like/comment count |
| Background | Transparent (matches `--carbon-mid: #2A2A2A`) |
| Link behavior | Open in new tab |

### Step 4 — Get Widget ID and Activate

1. Click **Save** in the Elfsight editor
2. Click **Get Code** — you will see an embed snippet like:
   ```html
   <script src="https://static.elfsight.com/platform/platform.js" async></script>
   <div class="elfsight-app-xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"></div>
   ```
3. Copy the Widget ID: `xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx`

### Step 5 — Activate in index.html

In `index.html`, find line:
```html
<div class="elfsight-app-WIDGET_ID_PAELLASYMAS" data-elfsight-app-lazy></div>
```

Replace `WIDGET_ID_PAELLASYMAS` with your actual Widget ID:
```html
<div class="elfsight-app-xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx" data-elfsight-app-lazy></div>
```

Commit with:
```bash
git add index.html
git commit -m "feat(v4.3.1): activate Elfsight widget ID · @paellasymas live feed"
git push origin main
```

---

## Free Tier Constraints

| Constraint | Free Tier | Basic ($5/mo) |
|---|---|---|
| Monthly views | 200 | Unlimited |
| Widgets per account | 1 | 3 |
| Elfsight branding | Logo on hover | Removed |
| Feed refresh rate | Every 24 hours | Every 24 hours |
| Posts displayed | Up to 12 | Up to 12 |
| Support | Community | Priority |

**200 views/month** = ~6-7 unique visitors/day viewing the Instagram section. For a low-traffic portfolio site this is acceptable for launch. Upgrade to Basic ($5/mo) when traffic exceeds this threshold.

---

## Upgrade Path

1. Log into [https://dash.elfsight.com](https://dash.elfsight.com)
2. Click **Upgrade** on the paellasymas widget
3. Select **Basic** plan ($5/month or $48/year)
4. No code changes required — widget ID stays the same

---

## Maintenance

- **Feed refresh:** Automatic every 24 hours. New posts on @paellasymas appear on the site within 24h.
- **Account re-auth:** If Instagram changes API permissions, Elfsight will email the account holder to re-authorize. This typically happens every 60-90 days.
- **Widget customization:** Log into [https://dash.elfsight.com](https://dash.elfsight.com) → select widget → edit settings → Save. Changes apply live without code updates.

---

## Technical Notes

- The Elfsight platform script (`platform.js`) is loaded `async` — no render-blocking impact.
- Widget uses `data-elfsight-app-lazy` attribute for lazy loading — loads only when section scrolls into view.
- The `WIDGET_ID_PAELLASYMAS` placeholder renders nothing until replaced with a real ID — the section header and CTA button remain visible as fallback.
- All existing CSS classes (`ig-header`, `ig-grid`, `ig-cta-btn`) are preserved for potential future use.

---

## Why Elfsight (vs alternatives)

| Service | Free Tier | Auth Required | HTTPS | Watermark |
|---|---|---|---|---|
| **Elfsight** | 200 views/mo | Owner OAuth | ✓ | Logo on hover |
| Behold | 1,200 views/mo | Owner OAuth | ✓ | Logo on hover |
| LightWidget | Unlimited | Owner OAuth | ✗ (paid) | None |
| EmbedSocial | 1 source | Owner OAuth | ✓ | Branding |
| SociableKit | 7-day trial | Owner OAuth | ✓ | Branding |

**Key constraint across ALL services:** Instagram's Graph API (since Oct 2020) requires the account owner to authorize OAuth access. There is no legitimate service that can display a private or public Instagram feed without the account owner's authorization. This is a Meta/Instagram platform policy, not a service limitation.

---

*FORGE Digital · dispatch 2026-05-21 · feat(v4.3)*
